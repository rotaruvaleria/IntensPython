#include <iostream>
#include <cmath>

using namespace std;

float ef(float x) 
  {
    return x - 0.2 * (pow(x, 2) + 6.0);
  }
  float sim(float x_0, float epsilon) 
  {
      float x = x_0;
      int iter = 0;
      while (true) 
      {
          float x_new = 0.2 * (pow(x, 2) + 6.0);
          if (fabs(x_new - x) < epsilon) 
          {
              cout << "Количество итераций: " << iter << endl;
              return x_new;
          }
          x = x_new;
          iter++;
      }
  }
int main() 
{
  float x_0 = 0;
  float epsilon = 1e-2;
  float root = sim(x_0, epsilon);
  cout << "Решение уравнения: x=" << root << endl;
  float fun=ef(root);
  cout << "Значение функции: " << root << "=" << fun << endl;
}
