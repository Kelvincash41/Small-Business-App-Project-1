// Small-Business-App-Project-1
#include <iostream>
#include <fstream>

 using namespace std;
int main() 
{
  int Coupon_number = 11098765;
  char ask_for_code;
  int Code;
  bool isvalid = false;

  while (isvalid == false )
  {
    //Ask customer for Coupon Code
    cout << "Answer the following questions\n";
    cout << "with either Y for Yes or ";
    cout << "N for No.\n";
    cout << "Do you have a coupon code? ";
    cin >> ask_for_code;

    if (ask_for_code == 'Y' || ask_for_code == 'y')
    {
      cout << "Enter the coupon code: ";
      cin>> Code; 
    } 
 

  if (Code == Coupon_number)
  {
    cout << "You qualify for another order\n";
    isvalid = true;
  }
  else
    cout << " Code is invalid\n";
}



      ofstream outputFile;
      

      // Open an output file.
      outputFile.open("Numbers.txt"); 

      // Write the numbers to the file.
      outputFile << Coupon_number << endl;
      outputFile << Code << endl;
      outputFile << ask_for_code << endl;
      cout << "The numbers were saved to a file.\n";

      // Close the file
      outputFile.close();
      cout << "Done.\n"; 
return 0;
}



