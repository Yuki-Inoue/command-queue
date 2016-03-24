# command-queue

The shell command batch queueu in emacs.

# How to Use

1. `M-x list-packages`, install  `command-queue` from MELPA
2. `M-x command-queue-publish-command` is the command to enqueue the shell command. enqueued command will get executed asynchronously, each by each.
3. When a command failed, the queue execution aborts.


# Background

When working inside emacs (and doing all the work from there), I often wants to queue the shell command execution, and the commands to be executed asynchronously. For example, manipulate DB, flush, and then search. These sequence of commands are intended to e executed one after another, and if any of the step fail, then I want the entire processing to be stopped and get aborted. Writing down such shell script is sometime cumbersome. OS batch queue feature might be available, but, as said, they are OS dependent so I have to remember each batching facilities of the host OS provides.

I wanted to execute batch queue in a same manner in both Windows and Ubuntu.

So, I wrote such package.


# disclaimer

I've just made a working prototype, and I know its crappy.

And many requests/issues/PR are welcome.
