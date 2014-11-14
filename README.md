class_part
==========
#include <iostream>
using namespace std;

class part  //define class
{
private:
    int modelnumber;  //ID number of widget
    int partnumber;    //ID number of widget part
    float cost;   //cost of part
public:
    void setpart(int mn,int pn, float c)  //set data
    {
        modelnumber=mn;
        partnumber=pn;
        cost=c;
    }
    void showpart()
    {
        cout<<"Moder "  <<modelnumber;
        cout<<",part"  <<partnumber;
        cout<<",cost $"<<cost<<endl;
    }
};


int main()
{
    part part1;
    part1.setpart(6244, 373, 217.55f);  //call member function
    part1.showpart();//call member function
    return 0;
}
