# Assignment_BTech2026_-2201920130161---
IT-C (06/02/2025)

#include <bits/stdc++.h> 
#include<iostream>

using namespace std;

class GrandFather

{

   

    public:

    string gname;

    GrandFather(string s):gname(s)

    {

 

    }

};

class Father:public GrandFather

{

   

    public:

    string fname;

    Father(string s,string f):fname(s),GrandFather(f){}

};

class Son:public Father

{

   

    public:

    string name;

    Son(string a,string b,string c):name(a),Father(b,c)

    {

 

    }

    void print()

    {

        cout<<"sonname: "<<name<<endl;

        cout<<"fathername: "<<fname<<endl;

        cout<<"grandfather: "<<gname<<endl;

    }

};

int main() {

    Son a("Saurabh","Ramesh","Suresh");

    a.print();



    return 0;
}
