#4100053008 王冠傑
#TheFunction(x)=1-exp(-x)
par(mfrow = c(1,2))
Inverse_Function=function(x)
{
y=-log(1-x)
return(y)
}
Derivative_Function=function(x)
{
y=exp(-x)
return(y)
}
x1=runif(10000)# 0~1
y1=Inverse_Function(x1)
hist(y1,breaks=50,col="blueviolet")
x2=seq(0.05,10,0.01)
y2=Derivative_Function(x2)
plot(x2,y2,"l")
