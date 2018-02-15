# Log rotation implementation in bash
All successful applications should have some form of logging. This keeps track of application states,
errors, warnings, and etc. Logs can be kept for security, for debugging, performance monitoring, or
any number of reasons.
Log files are often split into multiple files. One scheme of managing this is to have a log file for each
day.
