printf() : 출력
%d : 10진 정수로 출력
%f : 실수로 출력
%c : 문자로 출력
%s : 문자열로 출력

calculator.c

#include<stdio.h>

int main(void)
{
	int x;
	int y;
	int sum, diff, mul, div;

	x = 10;
	y = 20;

	sum = x + y;
	diff = x - y;
	mul = x * y;
	div = x / y;

	printf("두 수의 합 : %d\n", sum);
	printf("두 수의 차 : %d\n", diff);
	printf("두 수의 곱 : %d\n", mul);
	printf("두 수의 몫 : %d\n", div);

	return 0;
}

결과물:
두 수의 합 : 30
두 수의 차 : -10
두 수의 곱 : 200
두 수의 몫 : 0

scanf() : 입력

%d : 10진 정수 형태로 입력
%f : float형 실수 형태로 입력
%lf : double형 실수 형태로 입력
%c : 문자 형태로 입력
%s : 문자열 형태로 입력

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(void)
{
	int x;
	int y;
	int sum;

	printf("첫 번째 숫자를 입력하세요: ");
	scanf("%d", &x);

	printf("두 번째 숫자를 입력하세요: ");
	scanf("%d", &y);

	sum = x + y;
	printf("두 수의 합 : %d\n", sum);

	return 0;
}

결과물:
첫 번째 숫자를 입력하세요: 8
두 번째 숫자를 입력하세요: 7
두 수의 합 : 15

salary.c

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(void)
{
	int ysalary;
	int msalary;

	printf("연봉을 입력하세요(단위 : 만원): ");
	scanf("%d", &ysalary);

	msalary = ysalary / 12;
	printf("월수령액(단위 : 만원) : %d\n", msalary);

	return 0;
}

결과물:
연봉을 입력하세요(단위 : 만원): 5000
월수령액(단위 : 만원) : 416

circle.c

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(void)
{
	float radius;
	float area;

	printf("반지름을 입력하세요 : ");
	scanf("%f", &radius);

	area = radius * radius * 3.14;
	printf("원의 면적 : %f\n", area);

	return 0;
}

결과물:
반지름을 입력하세요 : 3
원의 면적 : 28.260000

exchange_rate.c

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(void)
{
	double rate;
	double usd;
	int krw;

	printf("환율을 입력하세요 : ");
	scanf("%lf", &rate);

	printf("원화 금액을 입력하세요 : ");
	scanf("%d", &krw);

	usd = krw / rate;
	printf("원화 %d원은 %f 달러입니다.\n", krw, usd);

	return 0;
}

결과물:
환율을 입력하세요 : 1477.62
원화 금액을 입력하세요 : 15000000
원화 15000000원은 10151.459780 달러입니다.

rectangle.c

#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>

int main(void)
{
	double w;
	double h;
	double area;
	double perimeter;

	w = 10.0;
	h = 5.0;
	area = w * h;
	perimeter = 2 * (w + h);

	printf("사각형의 넓이 : %f\n", area);
	printf("사각형의 둘레 : %f\n", perimeter);

	return 0;
}

결과물:
사각형의 넓이 : 50.000000
사각형의 둘레 : 30.000000