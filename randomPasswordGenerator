#include <iostream>
#include <string>
#include <cstdlib>
#include <time.h>
using namespace std;

int main(){
    srand(time(0));
    int passwordLength, possibleAmountOfEachChar, pT = 0;
    char c;
    bool numbersQ, smallLettersQ, bigLettersQ, specialCharsQ;
    string numbers = "0123456789", smallLetters = "abcdefghijklmnopqrstuvwxyz", bigLetters = "ABCDEFGHIJKLMNOPQRSTUVWXYZ", specialChars = "!@#$%^&*()/\\~`";
    string password = "";
    cout << "Lenght of password: "; cin >> passwordLength;
    cout << "Numbers? (y/n): "; cin >> c; numbersQ = (c == 'y'? true:false);
    cout << "SmallCars? (y/n): "; cin >> c; smallLettersQ = (c == 'y'? true:false);
    cout << "BigLetters?? (y/n): "; cin >> c; bigLettersQ = (c == 'y'? true:false);
    cout << "SpecialChars? (y/n): "; cin >> c; specialCharsQ = (c == 'y'? true:false);
    for(int i = 1; i <= passwordLength; i++){
        int random = rand()%4+1;
        if(random == 1){if(numbersQ){password+=numbers[rand()%numbers.length()+1];}else{i--;}}
        else if(random == 2){if(smallLettersQ){password+=smallLetters[rand()%smallLetters.length()+1];}else{i--;}}
        else if(random == 3){if(bigLettersQ){password+=bigLetters[rand()%bigLetters.length()+1];}else{i--;}}
        else if(random == 4){if(specialCharsQ){password+=specialChars[rand()%specialChars.length()+1];}else{i--;}}
    }
    cout << password << endl;
    return 0;
}
