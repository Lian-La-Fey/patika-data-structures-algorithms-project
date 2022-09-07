Proje 3
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

Root: 7

1st step:
```
    7
```

2nd step: We must add 5 to the left 'cause 5 < 7
    7
  /
5

3rd step:  We must add 1 to the left 'cause 1 < 7 and again left 'cause 1 < 5
```
        7
      /
    5
  /
1
```

3rd step:  We must add 8 to the right 'cause 8 > 7

```
        7
      /   \
    5       8
  /
1
```

4th step:  3 < 7 (left), 3 < 5 (left), 3 > 1 (right)

```
        7
      /   \
    5       8
  /           
 1
  \
    3
```

5th step:  6 < 7 (left), 6 > 5 (right)

```
        7
      /   \
    5       8
   / \       
  1   6
   \ 
    3
```
6th step:  0 < 7 (left), 0 < 5 (left), 0 < 1 (left)

```
        7
     /     \
    5        8
   /  \
  1     6
 / \               
0   3
```

7th step:  9 > 7 (right), 9 > 8 (right)

```
       7
     /   \
    5      8
   / \       \
  1   6        9
 / \
0   3
```

8th step:  4 < 7 (left), 4 < 5 (left), 4 > 1 (right), 4 > 3 (right)

```
        7
      /    \
    5        8
   / \        \
  1    6        9
 / \
0   3
      \
        4
```

9th step:  2 < 7 (left), 2 < 5 (left), 2 > 1 (right), 2 < 3 (left)

```
        7
      /   \
    5      8
   / \      \
  1    6     9
 / \
0   3
   / \
  2    4
```

[patika.dev](https://patika.dev)