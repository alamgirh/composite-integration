# Composite Numerical Integration (CNI)

Newton-Cotes formulas are not accurate for a large integral domain. The main idea of the CNI is to divide integral domain into subdomains and use simple integration rule for each subdomain. 

Using the C++ code (composite.cpp), I computed composite numerical integration over a quadrilateral region. We described the composite numerical integration over an arbitrary quadrilateral region in our following paper: 

Md. Shafiqul Islam and M. Alamgir Hossain (2009)- Numerical Integrations over an Arbitrary Quadrilateral Region, Applied Mathematics and Computations Volume 210, Issue 2, 15 April 2009, Pages 515-524.

## Run
Example 2 of Islam and Hossain (2009) can run in a terminal with the following instructions: 

$ g++ composite.cpp<br>
$ ./a.out

Enter the order of Gauss Legendre Quadrature rule: 3

|	$C_k$            |	$X_k$              | $Y_k$              |
|:-----------------|:--------------------|:-------------------|	
|0.154320987654321 |	-0.874596669241483 |  0.674596669241483 |
|0.151284361822039 |	-0.443649167310371 |	0.330947501931112 |
|0.034784464623228 |	-0.012701665379258 |	-0.012701665379258|
|0.342542798671788 |	-0.830947501931112 |	-0.056350832689629|
|0.395061728395062 |	-0.250000000000000 |	-0.250000000000000|
|0.151284361822039 |	0.330947501931112  |	-0.443649167310371|
|0.273857510685414 |	-0.787298334620741 |	-0.787298334620741|
|0.342542798671788 |	-0.056350832689629 |	-0.830947501931112|
|0.154320987654321 |	0.674596669241483  |	-0.874596669241483|

Enter the value of n (between 1 and 50) then discretise T into $4\times n^2$ triangle:10

|$4\times n^2$|		Result           |
|:-------|:--------------------|
|4 x 1^2 |  14.991195582852475 |
|4 x 2^2 |  19.267674833364271 |
|4 x 3^2 | 	20.238201270672942 |
|4 x 4^2 |	20.562029516588154 |
|4 x 5^2 |	20.693999549518534 |
|4 x 6^2 |  20.755006700820118 |
|4 x 7^2 |  20.785863805737211 |
|4 x 8^2 |  20.802577184929046 |
|4 x 9^2 |  20.812134862867111 |
|4 x 10^2|	20.817848407116379 |

