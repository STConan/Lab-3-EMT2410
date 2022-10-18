////////////////////////////////////////////////////////////////////////////////////////////////////////////////
//Title                : Lab 3 "Functions"                                                                    //
//Author               : Wellington Verduga Macias                                                            //
//Version and Date     : V0.1 10/07/2022                                                                      //
//Copyright disclaimer :                                                                                      //
////////////////////////////////////////////////////////////////////////////////////////////////////////////////

#include <iostream>
using namespace std;

float ArrayUserNumbers[5]; //Set up array for User's numbers

void RequestForUserNumbers();
float FindMaxNumber(float Array[5]);
float FindMinNumber(float Array[5]);
void DisplayMaxOrMin(float, float);

int main()
{    
    RequestForUserNumbers();
    
    float UserMin = FindMinNumber(ArrayUserNumbers);

    float UserMax = FindMaxNumber(ArrayUserNumbers);

    DisplayMaxOrMin(UserMin, UserMax);
    
    return 0;
}

void RequestForUserNumbers() //Function to request for User to input the 5 numbers
{
    cout << "The program requires you to give it 5 decimal numbers.\n"; //Informing the user about what is needed from them
    for (int i=0; i < 5; i++) //Loop for User to input the 5 numbers
    {
        cout << "Please, input your decimal numbers:\n";//Instruction for User
        cin >> ArrayUserNumbers[i];//Taking User's Input
    }
}

float FindMinNumber(float UserNumbers[5])//Function to find the minimum number
{
    float Min = UserNumbers[0];
    for(int i=1; i<5; i++)//Iteration to check every number in the array
    {
        if (UserNumbers[i] < Min) //Compares the current number in the array against the number already stored in UserMin
        {
            Min = UserNumbers[i]; //If statement is true, replaces UserMin for the number in the array
        }
    }
    return Min;
}

float FindMaxNumber(float UserNumbers[5])//Function to find the minimum number
{
    float Max = UserNumbers[0];
    for(int i=1; i<5; i++)//Iteration to check every number in the array
    {
        if (UserNumbers[i] > Max) //Compares the current number in the array against the number already stored in UserMax
        {
            Max = UserNumbers[i]; //If statement is true, replaces UserMin for the number in the array
        }
    }
    return Max;   
}

void DisplayMaxOrMin(float min, float max)//Function to display the values wanted
{
    char UserInput;
    cout << "Press 9 for the max number or 0 for the min number from the numbers given by you.\n";
    cin >> UserInput;
    switch(UserInput)
    {
        case '0':
            cout << "The min number in your array is " << min << ".\n";
            break;
        case '9':
            cout << "The max number in your array is " << max << ".\n";
            break;
        default:
            cout << "Please pick either 0 or 9 only.\n";
            break;
    }
}
