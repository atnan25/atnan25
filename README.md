#include <iostream>

using namespace std;

int main ()
{
  unsigned gaji, tunjang, zakat, penghasilan, emas;
  cout << "Masukan gaji perbulan: ";
  cin >> gaji;

  cout << "Masukan tunjangan perbulan: ";
  cin >> tunjang;
  
  cout << "Masukan harga emas per gram saat ini: ";
  cin >> emas;
  
  gaji = gaji * 12;
  tunjang = tunjang * 12;
  penghasilan = gaji + tunjang;
  zakat = penghasilan * 0.025;
  emas = emas * 85;

  if (penghasilan > emas)
    cout << "Jumlah zakat yang harus dikeluarkan: " << zakat;
  else
    cout << "Anda tidak harus mengeluarkan zakat";

  return 0;
}
