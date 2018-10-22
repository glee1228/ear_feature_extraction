## How To Extract Ear feature points

* #### Paper Title :

  ##### A novel geometric feature extraction method for ear recognition

* #### Link : https://www.sciencedirect.com/science/article/pii/S0957417416304341#tbl0002

![Figure 1:](https://ars.els-cdn.com/content/image/1-s2.0-S0957417416304341-gr1.jpg)



![Figure 4:](https://ars.els-cdn.com/content/image/1-s2.0-S0957417416304341-gr4.jpg)

```
* Input: Binary edge image of an ear image, segment length T.

* Output:Umax, Lmax, Llb, uls, urs and lls.

1  Search maximum EHL by computing the longest distance between ear edge points and obtain Umax, Lmax.
2  Select T points on either side of Umax to determine the segments uls and urs.
3  Similarly, Select T points on left side of Lmax to obtain lls.
```



| Abbreviation | Full name                                                    |
| ------------ | ------------------------------------------------------------ |
| *Uls*        | The upper left segment of the outer helix                    |
| *urs*        | The upper right segment of the outer helix                   |
| *lls*        | The lower left segment of the outer helix                    |
| *T*          | The number of pixels of *uls, urs* or *lls*                  |
| *U*max       | The upper point of the maximum ear height line               |
| *U*min       | The upper point of the minimum ear height line               |
| *L*max       | The lower point of the maximum ear height line               |
| *L*min       | The lower point of the minimum ear height line               |
| *C*max       | The middle point of the maximum ear height line              |
| *U*lb        | The left end point of the segment *uls*                      |
| *U*rb        | The right end point of the segment *urs*                     |
| *L*lb        | The left end point of the segment *lls*                      |
| *I*lh        | The intersection point on the left outer helix which is the closest to *C*max |
| *CI*         | The line segment between *C*max and *I*lh                    |

![Figure 5:](https://ars.els-cdn.com/content/image/1-s2.0-S0957417416304341-gr5.jpg)

```
* Input:Umax, Lmax, Llb, Ulb and Urb.

* Output: FVi (i = 1, 2, …, 6).

1  Take the distance from Umax to Lmax (the length of maximum EHL) as FV1.
2  Search the minimum EHL between upper region (uls and urs) and lower region (lls) and obtain Umin and Lmin. The distance from Umin to Lmin is denoted as FV2.
3  Take the summation and ratio of FV1 and FV2 to obtain FV3 and FV4, respectively.
4  Find the middle point Cmax of maximum EHL, compute the shortest distance from Cmax to the left outer helix region and get line segment CI. Then ratio of both FV1 and FV2 to the length of CI are taken as FV5 and FV6, respectively.
```





