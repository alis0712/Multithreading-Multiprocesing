Good day!

The first project in this respository is a producer and consumer problem made in UNIX. 
The aim of this project is to solve a producer and consumer problem using pthreads. Pthreads allows
developers to create threads which results in parallel programming opportunities which allows for
multiple computations to be done simultaneously on different threads. My program is comprised of
three major functions which are the Main, the producer and consumer functions. The main function
derives the entire program with calls to the producer and consumer functions along the way. The
program will throw errors if the necessary parameters are not entered which are time to sleep, number
of producers, and the number of consumers. The producer and consumer functions work exactly as
intended and rely on external “insert_item” and “remove_item” functions to handle the actual
operations of insertion and deletion of buffer elements. The code makes use of pthreads for
simultaneous production and consumption and handles synchronization issues via two mutex locks and
two semaphores. The two mutex locks, “in and out” ensure that the item is being produced or
consumed, inserted into the buffer or removed from it respectively and is not tampered with until the
operation is fully completed. The two semaphores, “full” and “empty” protect against buffer overhead.
This interprets more specifically to preventing production with a full buffer and prevents consumption
with an empty buffer. 

The second project is implementing the Least Recently Used Algorithm made in UNIX. 
Operating systems that use paging for memory management, page replacement algorithms are needed
to decide which page is needed to be replaced when new page comes in. Whenever a new page is
referred and not present in memory, a page fault error occurs and Operating system replaces one of the
existing pages with a newly needed page. There are different page replacement algorithms and the goal
for each algorithm is to reduce the number of page faults. LRU (Least Recently Used) algorithm is a
greedy algorithm where the page to be replaced is least recently used. The idea is based on locality of
reference, the least recently used page is not likely. 
