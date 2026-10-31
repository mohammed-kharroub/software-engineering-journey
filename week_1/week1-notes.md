step-by-step pseudocode
    task 1
        Pick up phone book
        Open to middle of phone book
            Look at page
            If person is on page
            Call person
            Else if person is earlier in book
        Open to middle of left half of book
        Go back to line 3
            Else if person is later in book
        Open to middle of right half of book
            Go back to line 3
        Else
            Quit

    task 2  play ainon weth frinds
        open laptop
        opan steam
        opan aion 2
        opan discord
            opan l7awma served discord
            look wase frinde ther
            if lokman our anas our gharbi there 
            intre the room 
            else if no frinde there look how is online gharbi anas lokman
            if gharbi online call him
            Go back to line 9
            if anas oneline call him
            Go back to line 9
            if lokman online call him
            Go back to line 9
            else play solo 
            quit
    
    task 3  watch anime
        open laptop 
        opan stremio
        serch for anime name 
        start watching
        if anime start in en swetch in japan
        if have no arabic sub swetch to arabic 
        else watch in en 
        quite

---------------------------------------------------------------------
Linear vs. Binary Search

Both are ways to find a target value in a collection. They differ in how they look, and in what they require.

Linear search

Start at the first element and check each one in order until you find the target or run out of items.

Looking for 23 in [7, 3, 23, 9, 15]: check 7, then 3, then 23. Found.

Works on any list, sorted or not.
Time complexity: O(n). In the worst case you check every element.
Simple, with nothing to set up. 

python
def linear_search(arr, target):
    for i, value in enumerate(arr):
        if value == target:
            return i
    return -1


Binary search

Binary search requires a sorted list. Instead of checking elements one by one, it repeatedly cuts the search area in half:

Look at the middle element.
If it equals the target, you’re done.
If the target is smaller, discard the right half. If larger, discard the left half.
Repeat on the remaining half.

Looking for 23 in [3, 7, 9, 15, 23, 31, 42]:

Middle is 15. 23 > 15, so keep the right half: [23, 31, 42]
Middle is 31. 23 < 31, so keep the left half: [23]
Middle is 23. Found, in 3 steps.

python

def binary_search(arr, target):
    low, high = 0, len(arr) - 1
    while low <= high:
        mid = (low + high) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return -1
    
Time complexity: O(log n). Each step halves the problem.
Requires sorted data (and ideally random access, like an array).
Why the difference matters
List size	Linear (worst case)	Binary (worst case)
100	100 checks	~7 checks
1,000,000	1,000,000 checks	~20 checks
1,000,000,000	1,000,000,000 checks	~30 checks

Doubling the data adds just one extra step to binary search, while linear search’s work doubles.

Which to use
Linear search when the data is unsorted, small, or you’ll only search once (sorting first would cost more than just scanning).
Binary search when the data is already sorted, or you’ll search it many times, so the cost of sorting is paid back.


            
        