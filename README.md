# rsyncD
My init script version to start rsync as a daemon

There is only two observations to run this script:

1. Be sure that the file "/etc/rsyncd.conf" exists with at least these lines on in

	log file = /var/log/rsyncd.log

	pid file = /var/run/rsyncd.pid

	lock file = /var/run/rsyncd.lock

2. Be sure that the user who will start the process have permission to write in /var/log and /var/run

That's it!
