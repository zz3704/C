* 4주차 C언어 실습

```C
#include <stdio.h>

int main(void) {

  double x, y, result;

  printf("두개의 실수를 입력하시오 : ");
  scanf("%lf  %lf", &x, &y);

  result = x + y;
  printf("%f / %f =%f\n", x, y, result);

  result = x - y;
  printf("%f / %f =%f\n", x, y, result);

  result = x + y;
  printf("%f / %f =%f\n", x, y, result);

  result = x / y;
  printf("%f / %f =%f\n", x, y, result);

  return 0;
} 
```
#include <stdio.h>

int main(void) {

  int x, y, back;
  int chon, obak, bak;

  printf("물건 값을 입력하시오 : ");
  scanf("%d", &x);

  printf("투입한 금액을 입력하시오 : ");
  scanf("%d", &y);

  back = y - x;
  printf("거스름돈은 다음과 같습니다.\n");

  chon = back / 1000;
  back %= 1000;

  printf("천원권 : %d개\n", chon);

  obak = back / 500;
  back %= 500;

  printf("오백원권 : %d개\n", obak);

  bak = back / 100;
  back %= 100;
  printf("백원권 : %d개\n", bak);

  return 0;
}
