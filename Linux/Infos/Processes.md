pid (processid), ppid (parentID), pgid (group id)  

  

setuid-programms -> run with predetermined user rights (not user who starts the process)

  

poss Status: running, sleeping, stopped, zombie

  

priority: niceness -> higehst prio (-20) lowest(19) default(10)

set prio -> nice -n 5 command args (5 is increment or decrement to default / old val)

set prio while running -> renice +5 -p <PID>

  

Kill processes:

default kill -15 (SIGTERM) terminates the program

hardkill: kill -9 (SIGKILL) terminates the program without letting it respond

syntax: kill -<signalNr/type> <PID>

  

killall kills all processes with given name:

rather give command name than pid

killall -15 bash equivalent to: killall bash

  

pkill: pkill is similar to kill but uses name instead of pid.

  
  

# ProcessMonitoring

  

ps, pstree, top, fg etx

  
  

ram operations ->

free    Brief summary of memory usage  

vmstat  Detailed virtual memory statistics and block I/O, dynamically updated   -> vmstat [options] [delay] [count]

pmap    Process memory map

  

info-file => /proc/meminfo, /proc/sys/vm