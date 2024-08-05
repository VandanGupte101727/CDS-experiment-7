# CDS-experiment-7

AIM:- To study and implement strings and arrays <br>

Software used:- VS code <br>

THEORY:-<br>
The two basic data structures in C++ for storing elemental sequences are arrays and strings. A group of identically typed elements kept in consecutive memory regions is called an array. Arrays have a fixed size when they are declared, and their index starts at 0. To declare an array of five numbers, for instance, use {int arr[5];`. Although arrays offer quick access to items, dynamic resizing is difficult due to their fixed sizes.

Character arrays ({char arr[]}) or the Standard Library's std::string class can be used to manage strings in C++. Character arrays are null-terminated strings in the C style ({'\0'}). char str[] = "Hello", for example, defines a C-string. More functionality and simplicity of use are provided by the `std::string} class, which includes member functions for manipulation, concatenation, and dynamic scaling.Take std::string s = "Hello"; as an example. Today's C++ programmers prefer the std::string class because of its robustness and flexibility.<br>

CODE:-
1).<br>

    #include<iostream><br>
    using namespace std;<br>

    int main() {
    int array1[5] = {19, 10, 18, 17, 9};
    int array2[] = {19, 10, 18, 17, 9};
    int array3[5] = {19, 10, 8};

    // Printing array using the traditional method 
    cout << "\nTraditional method: ";
    for (int i = 0; i < 5; ++i) {
        cout << array1[i] << " ";
    }
    cout << endl;

    // Printing the array with the modern method 
    cout << "Modern method: ";
    for (int j : array1) {
        cout << j << " ";
    }

    return 0;
    }
