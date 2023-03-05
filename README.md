# -m-s-t-v-s-k-t-c-a-v-n-b-n-
đếm số từ và số ký tự của văn bản 
#include <iostream>
#include <conio.h>
#include <math.h>
#include <cstring>
#include <sstream>
#include <math.h>
#include <iomanip>
using namespace std;
int main()
{
    string sentence;
    cout << "Nhap mot cau: ";
    getline(cin, sentence); 

    int wordCount = 0, charCount = 0;
    stringstream ss(sentence); 

    string word;
    while (ss >> word) 
    {
        wordCount++;
    }

    for (int i = 0; i < sentence.length(); i++) 
    {
        if (sentence[i] != ' ') 
        {
            charCount++;
        }
    }

    cout << "So tu trong cau la: " << wordCount << endl;
    cout << "So ky tu trong cau la: " << charCount << endl;

return 0;
}

