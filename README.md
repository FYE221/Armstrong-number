
#include<iostream.h>
#include<conio.h>
#include<math.h>
class arms
{
 int x,t;
 public:
 void get_x();
 void display();
 void check();
};

 void arms::get_x()
 {
  cin>>x;
 }
 void arms::check()
 {
 int i,p,q,r,s;
  for(i=100; i<=999; i++)
  {
   p=x%10;
   q=x/10;
   r=q%10;
   s=q/10;
   t=pow(p,3)+pow(r,3)+pow(s,3);
  }
 }
 void arms::display()
 {
  if(t==x)
  {
   cout<<"It's a Armstrong number"<<endl;
  }
  else
  {
   cout<<"Its not Armstrong number"<<endl;
  }
 }

 void main()
 {
  clrscr();
  arms m;
  cout<<"Enter the number which you want to check for Armstrong"<<endl;
  m.get_x();
  m.check();
  m.display();
  getch();
 }
