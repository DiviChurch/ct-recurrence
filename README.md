CT Recurrence
===========

The CT Recurrence class gets future recurring dates based on given arguments. It also considers excluded dates. It is used for events in the [Church Content](https://github.com/churchthemes/church-theme-content) plugin (and Pro add-on) and [Church Theme Framework](https://github.com/churchthemes/church-theme-framework).

Version 2.0 adopted the use of [php-rrule](https://github.com/rlanvin/php-rrule) (MIT) for more sophisticted patterns. Earlier versions used more simplistic, proprietary calculations. get_dates(), calc_next_future_date() and their arguments are backwards-compatible.

Be aware that version 2.0 requires PHP 5.3+ (a php-rrule requirement). ```get_dates()``` will return empty and ```calc_next_future_date()``` false when PHP version is too old. You can use the ```php_is_old()``` method to detect old version and show an admin notice to update.

See example usage at bottom of [ct-recurrence.php](https://github.com/churchthemes/ct-recurrence/blob/master/ct-recurrence.php).
