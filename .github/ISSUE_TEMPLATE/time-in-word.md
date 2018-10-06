---
name: Time In word
about: code in c++

---

#include<iostream>
#include<iterator>
#include<vector>
#include<bits/stdc++.h>

using namespace std;

int main()
{
    int h,m,i,j;
    string s;
    cin>>h;
    
    cin>>m;
    
    if(m>30&&h==12)
    {
    
    h=1;
}
    else if(m>30)
    {
        i=h+1;
        h=i;
    }
    
    
    
    if(h==1)
    s="one";
    if(h==2)
    s="two";
    if(h==3)
    s="three";
    if(h==4)
    s="four";
    if(h==5)
    s="five";
    if(h==6)
    s="six";
    if(h==7)
    s="seven";
    if(h==8)
    s="eight";
    if(h==9)
    s="nine";
    if(h==10)
    s="ten";
    if(h==11)
    s="eleven";
    if(h==12)
    s="twelve";
    
    
    if(m==00)
    {
        cout<<s<<" o' clock";
    }
    char numbers[100][100] = {
        "zero", 
        "one",
        "two",
        "three",
        "four",
        "five",
        "six",
        "seven",
        "eight",
        "nine",
        "ten",
        "eleven",
        "twelve",
        "thirteen",
        "fourteen",
        "fifteen",
        "sixteen",
        "seventeen",
        "eighteen",
        "nineteen",
        "twenty",
        "twenty one",
        "twenty two",
        "twenty three",
        "twenty four",
        "twenty five",
        "twenty six",
        "twenty seven",
        "twenty eight",
        "twenty nine",
        
    };
    if(m==1)
    cout<<"one minute past "<<s;
    if(m>1&&m<15||m>15&&m<30)
    {
        cout<<numbers[m]<<" minutes past "<<s;
    }
    if(m==15)
    cout<<"quarter past "<<s;
    if(m==30)
    cout<<"half past "<<s;
    
    if(m>30&&m<45||m>45&&m<60)
    cout<<numbers[60-m]<<" minutes to "<<s;
    if(m==45)
    cout<<"quarter to "<<s;
}
