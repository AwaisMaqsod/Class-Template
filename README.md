//Class-Template
//Class Template for addition of two number with integer and long data member, C++ Oop.
#include<iostream>
using namespace std;
template <class T>
class Addition
{
	public:
		T add( T,T);// T is data type arguments 
};
template<class T>
T Addition<T>::add(T t1 ,T t2){// t1 and t2 is arguments
	T sum;
	sum=t1+t2;
	return sum;
	
} 
int main(){
Addition<int>obj1;
Addition<long>obj2;
int A=10,B=20,c;//int values for add funtion as a permeters 
int X=110,Y=220,z;//long values for add funtion as a permeters  
c=obj1.add(A,B);
cout<<": Sum of intger values : "<<c<<endl;

z=obj2.add(X,Y);
cout<<": Sum of long values : "<<z<<endl;

	return 0;
}
