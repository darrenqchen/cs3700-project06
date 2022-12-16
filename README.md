Describe your high-level approach
- Elected a leader in the beginning because it was going to do leader selection regardless
- Made everything work in the main "run" function that just called helper functions based on the command made
- I don't really know how else to explain my high-level approach because it is basically the RAFT protocol
- For the append entries I just sent the whole log even though it might be a bit slower but it is a bit easier to deal with and passes the needed tests


The challenges you faced
- The main challenge I faced is the timing out one, I had to comment that out which resulted in many cases not passing because electing a new leader while the client is sending messages doesn't sync well even though I understood the concept I would say
- 

A list of properties/features of your design that you think is good
- I really liked how I took out all the code and made it into helper functions that were fairly easy to understand to the reviewer
- Overral the way I handled the commands is pretty good especially because I believe the ordering I made with them seems to make the most sense

An overview of how you tested your code.
- The main way I tested my code was by running the certain tests but if i needed a big check I would just send it to the autograder