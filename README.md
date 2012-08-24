/*
 * Permission to use and edit this software is freely granted,
 * provided that this statement is retained.
 *
 * Developed by Dr. Nikolas Askitis
 * Website: www.naskitis.com
 * Email:   askitisn@gmail.com
 *
 * Please visit www.naskitis.com for more information.   If you have
 * any questions regarding my work, do not hesitate to ask.
 *
 * Enjoy!
 *
 */

The copy-based burst sort algorithm is one of the fastest in-memory sorting 
algorithms for variable-length strings, as detailed in the computing
literature. I have written my own implementation of the copy-based burst sort 
in C using my knowledge of cache-conscious string data structures. This 
implementation may not be as fast or as memory-efficient as the original  
used by the authors, but given the results shown on my
website (www.naskitis.com), I am confident that it will serve as a good
baseline for your experiments :)

My implementation of the copy-based burst sort algorithm is a little 
different from how its explained in literature. First, the strings that 
are stored in containers are length-encoded --- the original algorithm simply 
stored null-terminated strings. Second, containers are not sized to fit into 
the L2 cache of a typical CPU, as is the intention of the burst sort algorithm. 
Instead, much like my implementation of the array burst trie and HAT-trie, 
containers are burst once they store more than a given number of strings,
which, in my opinion, is a simpler and more optimal approach. 


Feel free to improve the code, and if you can spare the time, please do write 
the code in other languages such as Java and C++.   If you decide to do this, 
please create a sub-directory within this repository for the language that you 
wish to implement it in.  For example: burst-sort-c++/  or  burst-sort-java/ 

If you have any questions regarding my work, feel free to ask.  

Cheers, 
Dr. Nikolas Askitis. 
