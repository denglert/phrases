# Geometry & trigonometry



## Complementary angle (arccos sin x)

```q
q)x:0.25
q)acos sin x
1.320796
q)x+acos sin x / should be 0.5*pi, approximately
1.570796
q)2*x+acos sin x
3.141593
```


## Rotation matrix for angle x (in radians) counter-clockwise

```q
q)x:0.25
q)((cos x;neg sin x);(sin x;cos x))
0.9689124 -0.247404
0.247404  0.9689124
```


## Degrees from radians

```q
q)x:0.5
q)57.295779513082323*x
28.64789
```


## Radians from degrees

```q
q)x:0.5
q)z:57.295779513082323*x
q)z
28.64789
q)0.017453292519943295*z
0.5
```


## Area of triangle with sides x

Heron’s rule.

```q
```q
q)hr:{sqrt (prd (sum x%2)-0,x)}
q)hr x
6f
```

