# EX-SMS-Gateway
Send SMS From Queue of your web server


EX SMS Gateway is powerful tool to send sms from your phone connection using API.

EX SMS Gateway required Send SMS permission to Send SMS from your sim card on all (API)http requests. If the app does not have Send SMS permission, then it will not work properly.

SMS & Data rates may apply: Depending on your cellphone plan, your carrier may charge standard message rates and data charges to send text messages.

Request URL Json Example:

http://example.com/get_queue_sms

Return: {"id":"786","phone":"+923133336426","text":"Hey Mian"}


Response URL Example:


http://example.com/sms_sent_status_update?sms_id={id}

Return: successed


Schedule Cron Every Minute Example (Linux Style):

*/1 * * * *

Permission Required:

SEND_SMS: Allows an application to send SMS messages.

INTERNET: Allows applications to open network sockets.

SCHEDULE_EXACT_ALARM: Allows applications to use exact alarm APIs.

ACCESS_NOTIFICATION_POLICY: Marker permission for applications that wish to access notification policy. This permission is not supported on managed profiles.

WAKE_LOCK: Allows using PowerManager WakeLocks to keep processor from sleeping or screen from dimming.

FOREGROUND_SERVICE: Allows a regular application to use Service.startForeground.

REQUEST_IGNORE_BATTERY_OPTIMIZATIONS: Permission an application must hold in order to use Settings.ACTION_REQUEST_IGNORE_BATTERY_OPTIMIZATIONS.
