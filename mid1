#include <iostream>
#include <cstdlib>
#include <iomanip>
using namespace std;

double milesToKm(double miles);
bool val(double tol, double miles);
double m(double *mil, double *func);

int main(int argc, char *argv[])
{
    double miles = 1.0, con[10];
    float tol;
    const double mil[] = {0.1,0.2,0.3,0.4,0.5,0.6,0.7,0.8,0.9,1.0}, func[]={0.070595, 0.127778, 0.193219, 0.256047, 0.320338, 0.377179, 0.437968, 0.502869, 0.566453, 0.627338};

    if (argc > 1) {
        miles = atof(argv[1]); 
        cout << miles << " miles = ";
        cout << milesToKm(miles) << " Km" << endl;
        cout << endl;
    }

    if (argc > 2) {
        miles = atof(argv[1]);
        tol = atof(argv[2]);
        cout << miles << " " << tol << endl;

        cout << "Unit test of milesToKm() function..." << endl;
        cout << "Tolerance: " << tol << endl;

        cout << "       Miles   Function" << endl;
        cout << "       -----   --------" << endl;
        for(int i=0; i<10; i++) {
            cout << i+1;
            cout << setw(9) << mil[i];
            //for(int i=0; i<10; i++)
            cout << setw(13) << milesToKm(mil[i]);
            //double dif = func[i] - tol;
            // con[i] = mil[i]*dif;
            //cout << con[i];
            if(mil[i]*func[i]-milesToKm(mil[i]) > tol || mil[i]*func[i]-milesToKm(mil[i]) < (-tol))
                cout << "    <--- bad value" << endl;
            else
                cout << endl;
            //        if (val == false)
            //            cout << "<--- bad value" << endl;
            //        else
            //            cout << endl;
        }
    }

    return 0;
}

double milesToKm(double miles)
{
    return (miles * 0.62137);
}

bool val(double tol, double miles)
{
    //    if (val <= miles-tol && val >= miles+tol)
    return true;
    return false;
}
double m(double *mil, double *func) {
    /*  double con[10];
        for(int i=0; i<10; i++) {
        double dif = func[i] - tol;
        con[i] = mil[i]*dif;
        }
        return *con;*/
    //    for(int i=0; i<10; i++)
    //return (mil[]*func[]);
}
