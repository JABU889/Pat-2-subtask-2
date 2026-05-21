# Pat-2-subtask-2
#include <iostream>
#include <string>
#include <cctype>
#include <limits> // Added for input safety

using namespace std;

// Function to translate English letters into Morse code
string getMorseCode(char ch) {
    switch (toupper(ch)) {
        case 'A': return ".-";
        case 'B': return "-...";
        case 'C': return "-.-.";
        case 'D': return "-..";
        case 'E': return ".";
        case 'F': return "..-.";
        case 'G': return "--.";
        case 'H': return "....";
        case 'I': return "..";
        case 'J': return ".---";
        case 'K': return "-.-";
        case 'L': return ".-..";
        case 'M': return "--";
        case 'N': return "-.";
        case 'O': return "---";
        case 'P': return ".--.";
        case 'Q': return "--.-";
        case 'R': return ".-.";
        case 'S': return "...";
        case 'T': return "-";
        case 'U': return "..-";
        case 'V': return "...-";
        case 'W': return ".--";
        case 'X': return "-..-";
        case 'Y': return "-.--";
        case 'Z': return "--..";

        // Space between words
        case ' ': return "/";

        // Numbers
        case '0': return "-----";
        case '1': return ".----";
        case '2': return "..---";
        case '3': return "...--";
        case '4': return "....-";
        case '5': return ".....";
        case '6': return "-....";
        case '7': return "--...";
        case '8': return "---..";
        case '9': return "----.";

        default: return "?";
    }
}

int main() {
    string message;

    cout << "======================================" << endl;
    cout << "        MORSE CODE TRANSLATOR         " << endl;
    cout << "======================================" << endl;

    cout << "\nAbout Morse Code:" << endl;
    cout << "Uses dots (.) and dashes (-) to represent characters." << endl;

    cout << "\nEnter a message to translate:" << endl;
    
    // getline is the best way to get a full sentence including spaces
    getline(cin, message);
    

    cout << "\nTranslated Morse Code:" << endl;
    cout << "--------------------------------------" << endl;

    
