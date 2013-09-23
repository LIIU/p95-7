p95-7
=====
#include <iostream>
using namespace std;
double p (double x,double y)
{
double t;
if(y==0) 
{
t=1.0;

}
else if(y==1)
{
t=x;

}
else
{
t=x*p(x,y-1);

}
return t;
}
void main()
{
double x,y;
cin>>x>>y; 
cout<<p(x,y)<<endl;
}
