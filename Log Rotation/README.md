# Log rotation implementation in bash
All successful applications should have some form of logging. This keeps track of application states,
errors, warnings, and etc. Logs can be kept for security, for debugging, performance monitoring, or
any number of reasons. Log files are often split into multiple files. One scheme of managing this is to have a log file for each
day.

In order to keep these files accurate, the engineers will schedule a nightly process to rotate the logs.
This rotation will increment the number in each file, and archive (or in our case, delete) any files older
than a specified number of days. A new, empty, log file should also be created. Logs can have any name, but will always follow the pattern logtype.number.log where the number is the current age of the file.
