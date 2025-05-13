Build and run each Dockerfile individually.

For `db`, we should be able to see some messages confirming that the data set
was loaded successfully (some `INSERT` lines in the container output).

For `web` and `words`, we should be able to see some message looking like
"server started successfully".

That's all we care about for now!

Bonus question: make sure that each container stops correctly when hitting Ctrl-C.

???
