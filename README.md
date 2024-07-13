# conversion_in_international_tim_frame
It is a problem in hackerrank 


#include<bits/stdc++.h>
using namespace std ;
using  ll = long long  ;
int main()
{
     string s , y;
     cin>>s;
     string x = " ";
     if(s[8]=='A')
     {
         if(s[0]=='1'&&s[1]=='2')
         {
             s[0]='0';
             s[1]='0';
         }
     }

      if(s[8]=='P'&&s[0]!='1')

     {
        
             x=x+s[0]+s[1];
             int a = stoi(x) + 12;
             y = to_string(a);
             s[0]=y[0];
             s[1]=y[1];
         
     }

      if (s[0]=='1'&&s[1]=='0'&&s[8]=='P')
     {
          s[0]='2';
          s[1]='1';

       }
      if (s[0]=='1'&&s[1]=='1'&&s[8]=='P')
     {
         s[0]='2';
         s[1]='3';
       }
     
  

  for(int i = 0 ; i<8;++i)
  {
       cout<<s[i];
  }

}
