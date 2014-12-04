unicorn_launcher
===============

Supervisor for unicorn. Process supervisors as runit works by keeping track pids, which does not work that great with unicorn's live restart mechanism. By letting runit monitor this supervisor, we can send USR2 signals with runit and still get a working live restart.

Unshamely stolen from https://github.com/discourse/discourse/blob/master/config/unicorn_launcher
