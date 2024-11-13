# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

First I would run the code several times with different lists the of the size 100 then with larger sized lists of 1000000 and time them each one. After that I would compare the times between the lists of 100 and lists of 1000000 and find the asymptotic growth. I would also run it on the same computer. The difference in times are expected to be proportional to each other. As a list is increased by a factor of x the time should also increase by a factor of x if the time is truely linear.

The algorithm X couldn't be $O(n)$ since the algorithm is comparision based it is like a binary tree. According to the slides the there is only two decisions that it is sorted or not so the number of leaves is at least n! and the height is at least log(n!) and the worst case of comparisions is log(n!). That makes the complexity $Omega(nlogn)$ according to Stirlings approximation.

Looked at the slides for a refresher on the Theroretical bounds. “I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”
