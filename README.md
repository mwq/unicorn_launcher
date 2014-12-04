unicorn_launcher
===============

Supervisor for unicorn. Process supervisors as runit works by keeping track of pids. This does not work that great with unicorn's live restart mechanism. By letting runit monitor this supervisor instead, USR2 signals can be sent with runit and result in a working live reload.

Stolen from https://github.com/discourse/discourse/blob/master/config/unicorn_launcher
