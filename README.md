MusicMappr FAQ
==========

1. What does it do? 

MusicMappr finds chunks of songs that are similar, and clusters them accordingly.
You can visualize these clusters and play them back at will. This is for music lovers who are
curious about the structures inherent to their favorite songs.

2. How does it work? 

MusicMappr uses a hodge-podge of HTML5 features as well as some clustering and visualization techniques from machine learning.
Using the WebAudio API, it extracts raw samples from a song. Then, it divides those samples into chunks
and performs a fourier transform on each chunk to extract frequency data (dividing the work into multiple WebWorkers to 
speed up the process). Then, MusicMappr uses the T-SNE algorithm to visualize differences between 
the high dimensional fourier features in 2-d space. Finally, it runs K-means clustering to show the clusters 
that arise from T-SNE.

3. How do I get it to work?

MusicMappr is a work in progress. Right now it is confirmed to work on Chrome and Firefox, but no other browsers.
Make sure you have the latest version of one of these browsers.

4.Where can I try it?

Go to http://fatsmcgee.github.io/musicmappr for a live demo! Not guaranteed to be the latest version.
