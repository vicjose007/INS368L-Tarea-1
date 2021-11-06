\#include <iostream>

 

using namespace std;

 

int main()

{  

  int x = 0, y = 1, limite, aux = 1;



  bool primo = true;



  cout << "Escriba el limite cantidad de numeros: ";



  cin >> limite;



  for(int i = 0; i < limite; i++)

  {

​     

​    aux = x + y;

​    x = y;

​    y = aux;



​    for(int i = 2; i < limite; i++)

​    {

​      if(y % i == 0) primo = false;

​    }

​    if(primo == true)

​    {

​      cout << y << " Primo. \n";

​    }

​    else 

​    {

​      cout << y << " No primo. \n";

​    }



​    if(y % 2 == 0)

​    {

​      cout << " Par ";

​    }

​    else

​    {

​      cout << " Impar ";

​    }

​      

  }



}