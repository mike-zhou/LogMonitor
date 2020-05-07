#Log Monitors
Check off-line or real-time logs.

##fileReceiver
Receive compressed log files uploaded from a browsesr.

##logReader
Decompress the compressed log file, populate database with log lines, then sort those lines in time ascending order

##logSender
Read log lines in ascending order from database, and send them to logDispatcher

##realTimeLogReceiver
Receive real-time logs, send them to logDispatcher and populate the database

##logDispatcher
Send log lines to each monitor.

##monitors
Receive log line from logDispatcher, and fire events to eventsViewer

##eventsViewer
Return evnets to browsers

##logViewer
Return synchronized log to browers.
