## Project 1B

## Q1: What are Channels and Kernels (according to EVA)?
A: Kernels - Kernels are the matrices that extract the features from an image. For example, a matrix that signifies a verical edge will extract all the vertical edges visible in  the image.

Channels - The resultant output when a kernel convolves over an image is a channel. It is also called as feature map. In the previous example, the result of the vertical edge kernel would be all the vertical edges present in the image visible as a separate image in itself.

![img](https://github.com/navneetteotia/EIP/blob/master/input%20and%20fm.PNG?raw=true)

## Q2: Why should we only (well mostly) use 3x3 Kernels?
A: Many different aspects come into play while choosing the size of the kernal:
1. We want the parameters to be the least to keep in the memory in check. Therefore, the dimension of the matrix has to be very small.
2. A 2X2 kernel can not extract all patterns like triangles and arcs. Whereas, a 3X3 can handle such features.

## Q3. How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)?
A: A 3X3 Convolution will have to be performed 99 times to reach 1X1 from 199X199. Following are the calculations:
  
199 X 199 | Conv(3X3) Layer1 -> 197 X 197  
197 X 197 | Conv(3X3) Layer2 -> 195 X 195  
195 X 195 | Conv(3X3) Layer3 -> 193 X 193  
193 X 193 | Conv(3X3) Layer4 -> 191 X 191  
191 X 191 | Conv(3X3) Layer5 -> 189 X 189  
189 X 189 | Conv(3X3) Layer6 -> 187 X 187  
187 X 187 | Conv(3X3) Layer7 -> 185 X 185  
185 X 185 | Conv(3X3) Layer8 -> 183 X 183  
183 X 183 | Conv(3X3) Layer9 -> 181 X 181  
181 X 181 | Conv(3X3) Layer10 -> 179 X 179  
179 X 179 | Conv(3X3) Layer11 -> 177 X 177  
177 X 177 | Conv(3X3) Layer12 -> 175 X 175  
175 X 175 | Conv(3X3) Layer13 -> 173 X 173  
173 X 173 | Conv(3X3) Layer14 -> 171 X 171  
171 X 171 | Conv(3X3) Layer15 -> 169 X 169  
169 X 169 | Conv(3X3) Layer16 -> 167 X 167  
167 X 167 | Conv(3X3) Layer17 -> 165 X 165  
165 X 165 | Conv(3X3) Layer18 -> 163 X 163  
163 X 163 | Conv(3X3) Layer19 -> 161 X 161  
161 X 161 | Conv(3X3) Layer20 -> 159 X 159  
159 X 159 | Conv(3X3) Layer21 -> 157 X 157  
157 X 157 | Conv(3X3) Layer22 -> 155 X 155  
155 X 155 | Conv(3X3) Layer23 -> 153 X 153  
153 X 153 | Conv(3X3) Layer24 -> 151 X 151  
151 X 151 | Conv(3X3) Layer25 -> 149 X 149  
149 X 149 | Conv(3X3) Layer26 -> 147 X 147  
147 X 147 | Conv(3X3) Layer27 -> 145 X 145  
145 X 145 | Conv(3X3) Layer28 -> 143 X 143  
143 X 143 | Conv(3X3) Layer29 -> 141 X 141  
141 X 141 | Conv(3X3) Layer30 -> 139 X 139  
139 X 139 | Conv(3X3) Layer31 -> 137 X 137  
137 X 137 | Conv(3X3) Layer32 -> 135 X 135  
135 X 135 | Conv(3X3) Layer33 -> 133 X 133  
133 X 133 | Conv(3X3) Layer34 -> 131 X 131  
131 X 131 | Conv(3X3) Layer35 -> 129 X 129  
129 X 129 | Conv(3X3) Layer36 -> 127 X 127  
127 X 127 | Conv(3X3) Layer37 -> 125 X 125  
125 X 125 | Conv(3X3) Layer38 -> 123 X 123  
123 X 123 | Conv(3X3) Layer39 -> 121 X 121  
121 X 121 | Conv(3X3) Layer40 -> 119 X 119  
119 X 119 | Conv(3X3) Layer41 -> 117 X 117  
117 X 117 | Conv(3X3) Layer42 -> 115 X 115  
115 X 115 | Conv(3X3) Layer43 -> 113 X 113  
113 X 113 | Conv(3X3) Layer44 -> 111 X 111  
111 X 111 | Conv(3X3) Layer45 -> 109 X 109  
109 X 109 | Conv(3X3) Layer46 -> 107 X 107  
107 X 107 | Conv(3X3) Layer47 -> 105 X 105  
105 X 105 | Conv(3X3) Layer48 -> 103 X 103  
103 X 103 | Conv(3X3) Layer49 -> 101 X 101  
101 X 101 | Conv(3X3) Layer50 -> 99 X 99  
99 X 99 | Conv(3X3) Layer51 -> 97 X 97  
97 X 97 | Conv(3X3) Layer52 -> 95 X 95  
95 X 95 | Conv(3X3) Layer53 -> 93 X 93  
93 X 93 | Conv(3X3) Layer54 -> 91 X 91  
91 X 91 | Conv(3X3) Layer55 -> 89 X 89  
89 X 89 | Conv(3X3) Layer56 -> 87 X 87  
87 X 87 | Conv(3X3) Layer57 -> 85 X 85  
85 X 85 | Conv(3X3) Layer58 -> 83 X 83  
83 X 83 | Conv(3X3) Layer59 -> 81 X 81  
81 X 81 | Conv(3X3) Layer60 -> 79 X 79  
79 X 79 | Conv(3X3) Layer61 -> 77 X 77  
77 X 77 | Conv(3X3) Layer62 -> 75 X 75  
75 X 75 | Conv(3X3) Layer63 -> 73 X 73  
73 X 73 | Conv(3X3) Layer64 -> 71 X 71  
71 X 71 | Conv(3X3) Layer65 -> 69 X 69  
69 X 69 | Conv(3X3) Layer66 -> 67 X 67  
67 X 67 | Conv(3X3) Layer67 -> 65 X 65  
65 X 65 | Conv(3X3) Layer68 -> 63 X 63  
63 X 63 | Conv(3X3) Layer69 -> 61 X 61  
61 X 61 | Conv(3X3) Layer70 -> 59 X 59  
59 X 59 | Conv(3X3) Layer71 -> 57 X 57  
57 X 57 | Conv(3X3) Layer72 -> 55 X 55  
55 X 55 | Conv(3X3) Layer73 -> 53 X 53  
53 X 53 | Conv(3X3) Layer74 -> 51 X 51  
51 X 51 | Conv(3X3) Layer75 -> 49 X 49  
49 X 49 | Conv(3X3) Layer76 -> 47 X 47  
47 X 47 | Conv(3X3) Layer77 -> 45 X 45  
45 X 45 | Conv(3X3) Layer78 -> 43 X 43  
43 X 43 | Conv(3X3) Layer79 -> 41 X 41  
41 X 41 | Conv(3X3) Layer80 -> 39 X 39  
39 X 39 | Conv(3X3) Layer81 -> 37 X 37  
37 X 37 | Conv(3X3) Layer82 -> 35 X 35  
35 X 35 | Conv(3X3) Layer83 -> 33 X 33  
33 X 33 | Conv(3X3) Layer84 -> 31 X 31  
31 X 31 | Conv(3X3) Layer85 -> 29 X 29  
29 X 29 | Conv(3X3) Layer86 -> 27 X 27  
27 X 27 | Conv(3X3) Layer87 -> 25 X 25  
25 X 25 | Conv(3X3) Layer88 -> 23 X 23  
23 X 23 | Conv(3X3) Layer89 -> 21 X 21  
21 X 21 | Conv(3X3) Layer90 -> 19 X 19  
19 X 19 | Conv(3X3) Layer91 -> 17 X 17  
17 X 17 | Conv(3X3) Layer92 -> 15 X 15  
15 X 15 | Conv(3X3) Layer93 -> 13 X 13  
13 X 13 | Conv(3X3) Layer94 -> 11 X 11  
11 X 11 | Conv(3X3) Layer95 -> 9 X 9  
9 X 9 | Conv(3X3) Layer96 -> 7 X 7  
7 X 7 | Conv(3X3) Layer97 -> 5 X 5  
5 X 5 | Conv(3X3) Layer98 -> 3 X 3  
3 X 3 | Conv(3X3) Layer99 -> 1 X 1  
