#include <iostream>
#include <string>


using namespace std;

int main()
{    const double Vat = 0.12;

    string name, printer, phone, table, choice;
  long double Amount,cost, balance,priceofprinter=755,priceofphone=690,priceoftable=395;
   double quantity,ID;
    cout << "*WELCOME TO DAKWA'S CORP. \n";
    cout << "\n";
    cout << "-SELLING ITEMS \n";
    cout << "ITEMS TO BE SOLD: \n";

    string item1, item2, item3;
    item1 = "table";
    item2 = "printer";
    item3 = "phone";

    cout << "1. table \n";
    cout << "2. printer \n";
    cout << "3. phone \n";


    cout << "\n";
    cout << "-KINDLY INPUT YOUR NAME \n";
    cin >> name;

    cout << "\n";
    cout << "KINDLY INPUT YOUR ID \n";
    cin >> ID;

    cout << "\n";
    cout << "-WHAT ITEM WOULD YOU WANT TO BUY? \n";
       cin>>choice;
    cout << "\n";
     if(choice==item1)
      {

          cout << "HOW MANY WOULD YOU WANT TO BUY?" << endl;
          cin>>quantity;
          cout << "HOW MUCH WOULD YOU WANT TO PURCHASE THE ITEM?" << endl;
          cin>>Amount;
          cost=priceofprinter*quantity+Vat;
          cout << "\n";

         if(Amount>cost)
      {
          balance=Amount-cost;
       }

       else{

        cout<<" INSUFFICIENT BALANCE TO PURCHASE ITEM "<<endl;
       }

        cout << "\n";
        cout<<"**********RECEIPT OF DAKWA CORP**********"<<endl;

     cout<<"BUYER'S NAME:"<<name<<endl;
     cout<<"BUYER'S ID:"<<ID<<endl;
     cout<<"ITEMS BOUGHT:"<<"printer"<<endl;
     cout<<"NUMBER OF ITEMS BOUGHT:"<<quantity<<endl;
     cout<<"VAT:"<<Vat<<endl;
     cout<<"COST TOTAL:$"<<cost<<endl;
     cout<<"SUM TOTAL:$"<<Amount<<endl;
     cout<<"BALANCE:$ "<<balance<<endl;

       }

      else if (choice==item2)
      {

          cout << "HOW MANY WOULD YOU WANT TO BUY?" << endl;
          cin>>quantity;
          cout << "HOW MUCH WOULD YOU WANT TO PURCHASE THE ITEM?" << endl;
          cin>>Amount;
          cost=priceofphone*quantity+Vat;
          cout << "\n";

         if(Amount>cost)
      {
          balance=Amount-cost;
       }

       else{

        cout<<" INSUFFICIENT BALANCE TO PURCHASE ITEM"<<endl;
       }

        cout << "\n";
        cout<<"**********RECEIPT OF DAKWA CORP**********"<<endl;

     cout<<"BUYER'S NAME:"<<name<<endl;
     cout<<"BUYER'S ID:"<<ID<<endl;
     cout<<"ITEMS SOLD:"<<"phone"<<endl;
     cout<<"NUMBER OF ITEMS:"<<quantity<<endl;
     cout<<"VAT:"<<Vat<<endl;
     cout<<"COST TOTAL:$"<<cost<<endl;
     cout<<"SUM TOTAL:$"<<Amount<<endl;
     cout<<"BALANCE:$ "<<balance<<endl;

      }
        else if (choice==item3)
        {

          cout << "HOW MANY WOULD YOU WANT TO BUY?" << endl;
          cin>>quantity;
          cout << "HOW MUCH WOULD YOU WANT TO PURCHASE THE ITEM?" << endl;
          cin>>Amount;
          cost=priceoftable*quantity+Vat;
          cout << "\n";

         if(Amount>cost)
      {
          balance=Amount-cost;
       }

       else{

        cout<<"INSUFFICIENT BALANCE TO PURCHASE ITEM"<<endl;
       }

        cout << "\n";
        cout<<"**********RECEIPT OF TEKHOUSE LIMITED**********"<<endl;

     cout<<"BUYER'S NAME:"<<name<<endl;
     cout<<"BUYER'S ID:"<<ID<<endl;
     cout<<"ITEMS BOUGHT:"<<"table"<<endl;
     cout<<"NUMBER OF ITEMS BOUGHT:"<<quantity<<endl;
     cout<<"VAT AMOUNT:"<<Vat<<endl;
     cout<<"COST TOTAL:$"<<cost<<endl;
     cout<<"SUM TOTAL:$"<<Amount<<endl;
     cout<<"BALANCE:$ "<<balance<<endl;

        }

        else {
            cout << "Sorry...This product is unknown \n";

        }
        cout << "\n";
        cout << "THANK YOU FOR YOUR CO-OPERATION \n";
    return 0;
}