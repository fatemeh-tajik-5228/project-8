# project-8
#include <iostream>
using namespace std ;
// jadval arzesh gozare ha / do gozare 
int main () {
	string arzesh ;
	cout << "vared konid (A&B or A|B)" << "\n" ;
	cin >> arzesh ;
	
	cout << "A\tB\tresult\n" ;
	for(int a=0 ; a<=1 ; a++) {
		for(int b=0 ; b<=1 ; b++) {
			bool result ;
			if(arzesh == "A&B") result = a&&b ;
			else if(arzesh == "A|B") result = a||b ;
			else {
				cout << "namotabar" << "\n" ;
				return 1 ;
			}
			
			cout << a << "\t" << b << "\t" << result << "\n" ;
		}
	}
	return 0 ;
}
