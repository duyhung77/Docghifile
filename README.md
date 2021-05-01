#include <fstream>
#include <iostream>
using namespace std;

int main()
{
    // Cấp phát
    char data[100];

    // Mở một file 
    ofstream outfile;
    outfile.open("savefile.txt");

    cout << "Ghi du lieu vao trong file!" << endl;
    // Ghi thêm dữ liệu cần ghi vào trong file ở dưới





    // Ghi dữ liệu đã nhập vào trong file
    outfile << data << endl;

    // Đóng file 
    outfile.close();

    // Mở một file
    ifstream infile;
    infile.open(".txt");

    cout << "\n===========================\n";
    cout << "Doc du lieu co trong file!" << endl;
    infile >> data;

    // Ghi dữ liệu ra màn hình
    cout << data << endl;

    // Tiếp tục đọc và hiển thị dữ liệu ra nếu có 
    infile >> data;
    cout << data << endl;

    // Đóng file
    infile.close();

    return 0;
}
