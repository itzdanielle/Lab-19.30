# Lab-19.30
#include <iostream>
using namespace std;

void conversion (double& inches, int& foot) {
  cout << "Input how many inches you would like to convert to meters" << endl;
  cin >> inches;
  cout << "Input how many feet you would like to convert to meters" << endl;
  cin >> foot;
}
double calculations ( double inches, int foot ){ 
  double meter = 0.3048 * (foot + inches/ 12); 
  return meter;
}
void results (double inches, int foot, double meter) { 
 cout << "Inches : " << inches << endl;
 cout << "Feet : " << foot << endl;
 cout << "Meters : " << meter << endl;
}


int main() {
  double inches;
  int foot;
  double meter;
  conversion (inches, foot);
  meter = calculations (inches, foot);
  results (inches, foot, meter);
}
