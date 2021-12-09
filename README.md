# Revision

SLIDE 3, Write a code that asks the user to input 5 subject marks (0-100) and
Calculates the sum and average

  #include <iostream>
  #include <string>
  using namespace std;

  int main()
  {
      //variables
      int sub1, sub2, sub3, sub4, sub5;
      float sum, ave;

      //A code that asks the user to input 5 subject marks (0-100) and calculates the sum and average
      cout << "Enter 5 subject marks in order to calculate the sum and average:" << endl;
      cout << "\nSubject [1]: "; cin >> sub1;
      cout << "\nSubject [2]: "; cin >> sub2;
      cout << "\nSubject [3]: "; cin >> sub3;
      cout << "\nSubject [4]: "; cin >> sub4;
      cout << "\nSubject [5]: "; cin >> sub5;

      //subject mark (0-100)
      if ((sub1 >= 0 && sub1 <= 100) &&
          (sub2 >= 0 && sub2 <= 100) &&
          (sub3 >= 0 && sub3 <= 100) &&
          (sub4 >= 0 && sub4 <= 100) &&
          (sub5 >= 0 && sub5 <= 100)) {
          double sum = (sub1 + sub2 + sub3 + sub4 + sub5); //formula for sum
          double ave = (sub1 + sub2 + sub3 + sub4 + sub5) / 5; //formula for average
          cout << "\nSum = " << sum << endl;
          cout << "\nAverage = " << ave << endl;
      }
      else {
          cout << "\n\nIncorrect input." << endl;
      }
      return 0;
  }
                                                
SLIDE 5, Write the code that asks the user to input 5 subject marks (0-100) and
Calculates the sum and average making sure that program handles the fail
command
                                                
  #include <iostream>
  #include <string>
  using namespace std;

  int main()
  {
      //variables
      int sub1, sub2, sub3, sub4, sub5;
      float sum, ave;

      //A code that asks the user to input 5 subject marks (0-100) and calculates the sum and average
      cout << "Enter 5 subject marks in order to calculate the sum and average:" << endl;
      cout << "\nSubject [1]: "; cin >> sub1;
      cout << "\nSubject [2]: "; cin >> sub2;
      cout << "\nSubject [3]: "; cin >> sub3;
      cout << "\nSubject [4]: "; cin >> sub4;
      cout << "\nSubject [5]: "; cin >> sub5;

      //subject mark (0-100)
      if (!cin.fail()&&(sub1 >= 0 && sub1 <= 100) &&
          (sub2 >= 0 && sub2 <= 100) &&
          (sub3 >= 0 && sub3 <= 100) &&
          (sub4 >= 0 && sub4 <= 100) &&
          (sub5 >= 0 && sub5 <= 100)) {
          double sum = (sub1 + sub2 + sub3 + sub4 + sub5); //formula for sum
          double ave = (sub1 + sub2 + sub3 + sub4 + sub5) / 5; //formula for average
          cout << "\nSum = " << sum << endl;
          cout << "\nAverage = " << ave << endl;
      }
      else {
          cout << "\n\nIncorrect input." << endl;
      }
      return 0;
  }       

SLIDE 6, Write a code that asks the user their age (>=10), and
according to that give them a message.

  #include <iostream>
  using namespace std;

  int main()
  {
    //variable
    int age;

    cout << "Enter your age: "; cin >> age;

    //age should be greater than or equal to 10
    if (age >= 10) {
      if (age >= 10 && age <= 12) //10-12
      {
        cout << "\nPreteen age.";
      }
      if (age >= 13 && age <= 19) //13-19
      {
        cout << "\nTeen-age.";
      }
      else if (age >= 20 && age <= 29) //20-29
      {
        cout << "\nTwenties.";
      }
      if (age >= 30 && age <= 39) //30-39
      {
        cout << "\nThirties.";
      }
      if (age >= 40 && age <= 49) //40-49
      {
        cout << "\nForties.";
      }
      if (age >= 50 && age <= 59) //50-59
      {
        cout << "\nFifties";
      }
      if (age >= 60) //greater than or equal to 60
      {
        cout << "\nSixties or above.";
      }
    }
    else { //less than 10
      cout << "\nIncorrect input.";
    }
    return 0;
  }
