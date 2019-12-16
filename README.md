# **Assignment 1**

In assignment number 1, we are supposed to help John by doing his two tasks: one to reduce the time of his task in which he was supposed to download 1000 images from imgur, for this purpose we have to first get the client id in order to download the image from imgur.com. The Postman app is used to create a client id. After creating the client id, we have to download images from imgur by using John's codes. By doing so, it took 13 minutes and 57 seconds but as this is I/O bound operation, so threading is  supposed to reduce the time therefore when I used my code for multithreading on the same machine it reduces walltime to 2 minutes 29 seconds.

Again, for resizing, John's code to resize 1000 images took 10.1seconds as it is CPU bound process and it is suggested to use multiprocessing to reduce the time, so I used multiprocessing which took only 5.42seconds on the same machine. 

For multithreading, I used threading module and defined a function worker and ran the code using 10 workers. The different numbers for worker are tried but with downloading 1000 images I reached the maximum downloading images. The worker 10 was found best among the other tries. For multiprocessing, I used "multiprocessing" module and used 10 pools and it ran the 10 parallel processing to perform the same task. The other pool size less than 10 and more than 10 were also used but the performance was found best with minimum time for pool 10.

For I/O bound operation multithreading and for CPU bound operation multiprocessing reduced the time significantly. Images and resized images can not be uploaded in Github due to the restriction on number of files that should be less than 100.
