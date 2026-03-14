07

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(void)
{
	float inch, mm;
	printf("인치 단위로 입력 : ");
	scanf("%f", &inch);
	mm = inch * 25.4;
	printf("%f 인치 = %f mm", inch, mm);
	return 0;
}

결과물:
인치 단위로 입력 : 10
10.000000 인치 = 254.000000 mm

08

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(void)
{
	int x, y, prod;
	scanf("%d", &x);
	scanf("%d", &y);
	prod = x * y;
	printf("곱셈의 결과: %d", prod);
	return 0;
}

결과물:
6
3
곱셈의 결과: 18