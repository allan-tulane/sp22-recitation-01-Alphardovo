Lab 1
Name: Haochen Chen, Maria Chen

4.Describe the worst-case input value of key for linear search? for binary search?

TODO: The worst-case for linear search is that the input value of key being searched is not in the sequence. When the key is not exist, search() need to compare all the values of the array. The worst time complexity for linear search is O(n). The worst-case for binary search is that the input value of key is exist on the edge of array, which is at the index0 or index(len-1). The worst time complexity for binary search is O(log^n). 

5.Describe the best-case input value of key for linear search? for binary search?

TODO: The best-case for linear search is that the input value of key being searched is at the first position of the array, which is at index0. The best time complexity for linear search is O(1). The best-case for binary search is that the input value of key is exist in the middle of array. That means the first time search will find that key through all array. The best time complexity for binary search is O(1).

8.Call print_results(compare_search()) and paste the results here: [(10, 0.004291534423828125, 0.0045299530029296875), (100, 0.0171661376953125, 0.0057220458984375)]

9.The theoretical worst-case running time of linear search is $O(n)$ and binary search is $O(log_2(n))$. Do these theoretical running times match your empirical results? Why or why not?
TODO: These theoretical running time matches our empirical results. Based on the timing results above, we can find that the running time of linear search grows linearly as the input size $n$ getting larger, but the running time of binary search does not grow significantly.

10.Binary search assumes the input list is already sorted. Assume it takes $\Theta(n^2)$ time to sort a list of length $n$. Suppose you know ahead of time that you will search the same list $k$ times.
What is worst-case complexity of searching a list of $n$ elements $k$ times using linear search? 

TODO: The worst-case complexity of searching a list of $n$ elements $k$ times using linear search is $k*n$.
For binary search? 

TODO: For binary search, we have to first sort the list which requires $n^2$ times. Then, searching $k$ times in the worst-case costs $k*log(n)$ times, so total time is $n^2+k*log(n)$.

For what values of $k$ is it more efficient to first sort and then use binary search versus just using linear search without sorting? 

TODO: When $k$>>$n$, $k^n$>>$n^2$, it is more efficient to first sort and then use the binary search. 