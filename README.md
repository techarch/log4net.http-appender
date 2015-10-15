Log4Net Http Appender
===

Provides async logging to an http endpoint, log entries are queued and posted in a separate thread at the set 
batch max value, to prevent overly chunky requests. 

Thread sleeps after processing for 200ms then rechecks the queue. 