The minimal answering machine db is not intended to be logged into,
it's just a place holder for when your MOO has moved.

You have to edit the Minimal-AnsMachine.db file in a text editor and 
change the following line:

msg = {"", "OurMOO has moved to 000.000.000.000 port 7007.", "Please update your world files.", ""};

to something relevant for your move. Save it, then restart the MOO server
on your old port using this db:

./restart Minimal-AnsMachine 8888

Now when people connect they'll get the answering machine message, and
then get booted. Since this runs on the minimal db, it uses very little
memory, and like the regular MOO server it can keep running until the 
system gets shut down.
