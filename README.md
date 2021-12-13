# Advance-function


//buying
#include <iostream>
using namespace std;


double sumitems(double item1, double item2) {
	double total = item1 + item2;
	return total;
}

int main() {
	double mymoney = 40.00;
	double tshirt, shoes;
	cout << "Your money is 40.00\n\n";
	cout << "How much for the tshirt?" << endl;
	cin >> tshirt;
	cout << "How much for the shoes?" << endl;
	cin >> shoes;
	if (sumitems(shoes, tshirt) <= mymoney) {
		cout << "You can afford this item" << endl;
	}
	else {
		cout << "Keep saving" << endl;
	}

	return 0;
}
                                 
                                 
                                 
 //timecheck
                                 #include <iostream>
#include <string>
using namespace std;

string time(int time) {
	if (time >= 0 && time <= 11) {
	return "Good morning";
	}
	else if (time >= 12 && time <= 17) {
		return "Good afternoon";
	}
	else if (time >= 18 && time <= 21) {
		return "Good evening";
	}
	else if (time >= 22 && time <= 24) {
		return "Good night";
	}
	else {
		return "Invalid";
	}
}

int main() {
	int userinput;
	cout << "What time is it?" << endl;
	cin >> userinput;

	cout << time(userinput) << endl;
}
