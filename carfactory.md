# car-manufacturing-factory
#include<iostream>
using namespace std;
class Assembly_line
{
protected:
	char name[50];
	char engine;
public:
	void procedure()
	{
		cout << "\t procedure is" << endl;
		cout << "\tConversion of a steel sheet into Car body shape " << endl;
		cout << "\tCarry the Body into Electric charge Tunnel " << endl;
		cout << "\tPaint Process......! " << endl;
		cout << "\tTake the Body into Cabin For Decrease the Body temprature " << endl;
		cout << "\tlaunching the Doors " << endl;
		cout << "\tBonnet/Carry cover" << endl;
		cout << "\tElectric System/Lights/AC" << endl;
		cout << "\tFront/Back/Doors/side miror" << endl;
		cout << "\tSeats Procces" << endl;

	}
	void car_name()
	{
		cout << "\t\tEnter the car name:" << endl;
		cin >> name;
	}
	void Selection()
	{
		cout << "\t\t\t\tAudi Production Factory" << endl;
		cout << "\t%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%" << endl;
		cout << "\t%%%%%%%%%                                           %%%%%%%%%" << endl;
		cout << "\t%%%%%%%%%                   Selection               %%%%%%%%%" << endl;
		cout << "\t%%%%%%%%%                                           %%%%%%%%%" << endl;
		cout << "\t%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%" << endl;
		cout << "\tPress 1 for show procedure" << endl;
		cout << "\tPress 2 for creating body shape " << endl;
		cout << "\tPress 3 to carry the Body into Electic tunnel " << endl;
		cout << "\tPress 4 for paint process  " << endl;
		cout << "\tPress 5 for Givind Body cool " << endl;
		cout << "\tPress 6 for launching Doors:" << endl;
		cout << "\tPress 7 for Giving upper shape Bonnet..." << endl;
		cout << "\tPress 8 for Installing Glass " << endl;
		cout << "\tPress 9 for Attaching the Seats " << endl;

	}
	void work()
	{
		int option;
		float lnght;
		float wdth;
		int amount;
		int Amount;
	Selection:
		Selection();
		cin >> option;
		switch (option)
		{
		case 1:
		{			cout << "___________________________________________________________" << endl;
		procedure();
		goto Selection;
		break;
		}
		case 2:
		{
				  cout << "______________________________________________________________________________" << endl;

				  cout << "enter Lenght" << endl;
				  cin >> lnght;
				  cout << "ENTER width" << endl;
				  cin >> wdth;
				  cout << "lenght and width=" << lnght << "," << wdth << endl;
				  cout << lnght << "," << wdth << " BODY IS READY" << endl;
				  goto Selection;
				  break;
		}
		case 3:
		{		cout << "________________________________________________________________" << endl;
		cout << "Set the Apply charge";
		cin >> amount;
		cout << "Apply charge amount is" << amount << endl;
		goto Selection;
		break;
		}
		case 4:
		{
				  cout << "___________________________________________________________________________" << endl;
				  int coloure = 250;
				  cout << "enter apply charge amount" << endl;
				  cin >> Amount;
				  if (Amount<coloure)
					  cout << "Red Coloure Is painted" << endl;
				  else
					  cout << "Default Colure" << endl;
				  goto Selection;
				  break;
		}
		case 5:
		{
				  cout << "______________________________________________________________________" << endl;
				  int temp;
				  cout << "Enter The Temp" << endl;
				  cin >> temp;
				  cout << "Body having Temprature" << temp << endl;
				  goto Selection;
				  break;
		}
		case 6:
		{
				  cout << "_______________________________________________________________________________________" << endl;
				  cout << "Doors Launched:" << endl;

				  goto Selection;
				  break;
		}
		case 7:
		{
				  cout << "______________________________________________________________________________________" << endl;

				  cout << "clear" << endl;

				  goto Selection;
				  break;
		}
		case 8:
		{		cout << "_______________________________________________________________________________________" << endl;
		int glass;
		int code = 92;
		int country_code;
		cout << "Enter COUNTRY code" << endl;
		cin >> country_code;
		if (country_code = code)
			cout << "Transparent Glass is Attached with Front,back,side" << endl;
		else
			cout << "Green TRANSPARENT glass is attached with sides :" << endl;
		goto Selection;
		break;
		}
		case 9:
		{
				  cout << "________________________________________________________________________" << endl;

				  cout << "seats are insatalled Succesfully:" << endl;

				  goto Selection;
				  break;
		}
		
				   break;
		}
		
		}
	}

};

//Drived class
class parts_asembly : public Assembly_line

int main()
{

	cout << "\t\t         @ @    @ @   @ @   @ @               " << endl;
	cout << "\t\t       @     @      @     @     @              " << endl;
	cout << "\t\t      @     @ @    @ @   @ @     @        " << endl;
	cout << "\t\t     @     @   @  @   @ @   @     @        " << endl;
	cout << "\t\t     @     @   @  @   @ @   @     @     " << endl;
	cout << "\t\t      @     @ @    @ @   @ @     @        " << endl;
	cout << "\t\t       @     @      @     @     @         " << endl;
	cout << "\t\t         @ @    @ @   @ @   @ @           " << endl;
	cout << "\t\t()()()()()()()()()()()()()()()()()()()()" << endl;
	return 0;
}
