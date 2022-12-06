# Single-Lane-Bridge
Single Lane Bridge Problem

Problem Statement : 

A single-lane bridge connects the two Vermont villages of North Tunbridge and South Tunbridge. Farmers in the two villages use this bridge to deliver their produce to the neighboring town. The bridge can become deadlocked if a northbound and a southbound farmer get on the bridge at the same time. (Vermont farmers are stubborn and are unable to back up.) Using semaphores and/or mutex locks, design an algorithm in pseudocode that prevents deadlock. Implement your solution using POSIX synchronization. In particular, represent northbound and southbound farmers as separate threads. Once a farmer is on the bridge, the associated thread will sleep for a random period of time, representing traveling across the bridge. Design your program so that you can create several threads representing the northbound and southbound farmers.

We have implemented a C++ program to help us understand a solution to this problem preventing deadlock and starvation.

To compile : g++ main.cpp -lpthread

To run :

    1)./a.out
        Creates random number of villagers in North and South
        Allows a villager to starve for count = 3, atmost
    2)./a.out s
        Creates random number of villagers in North and South
        Allows a villager to starve for count = s (integer), atmost
    3)./a.out m n
        Creates m (integer) & n (integer) number of North & South villagers respectively and randomly
        Allows a villager to starve for count = 3, atmost
    4)./a.out m n s
        Creates m (integer) & n (integer) number of North & South villagers respectively and randomly
        Allows a villager to starve for count = s (integer), atmost
