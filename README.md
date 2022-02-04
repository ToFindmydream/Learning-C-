# Learning-C-
C/C++ 배우는 과정입니다.

2022년 2월 4일

/*변수 알아보기*/
#include <stdio.h>
int main() {
	int a; //a라는 변수(정수)를 쓰겠다
	a = 10;
	printf("a의 값은 : %d \n", a); /*%d 는 a 의 값 (정확히는 
								   처음 "" 다음에 오는 첫 번째 변수) 
								   을 10 진수 로 출력하라*/
	return 0;
}

/*변수 알아보기2*/
#include <stdio.h>
int main() {
	int a;
	a = 127;
	printf("a의 값은 %d 진수로 %o 입니다. \n", 8, a); // %o 8진수로 표현
	printf("a의 값은 %d 진수로 %d 입니다. \n", 10, a); // %d 10진수로 표현
	printf("a의 값은 %d 진수로 %x 입니다. \n", 16, a); // %x 16진수로 표현
	return 0;
}

/*변수 알아보기3*/
#include <stdio.h>
int main() {
	float a = 3.141592f; //float 형이라는 것을 확실히 하기 위해 f 붙임
	double b = 3.141592;
	printf("a : %f \n", a);//%f는 실수형 변수를 출력할 때 사용된다.
	printf("b : %f \n", b);// 이때 반드시 1과 같은 정수가 아니라1.0같이 실수로 표현
	return 0;
}

/*printf 형식*/
#include <stdio.h>
int main() {
	float a = 3.141592f;
	double b = 3.141592;
	int c = 123;
	printf("a : %.2f \n", a); // 반드시 소수점 둘째자리까지 표시
	printf("b : %5d \n", c); // 되도록 숫자자리수를 5자리로 표시
	printf("b : %6.3f \n", b); // 둘이 합친 것
	return 0;
}

/*산술 연산*/
#include <stdio.h>
int main() {
	int a, b;
	a = 10; // =는 우측의 값을 좌측에 대입하는 것 우측부터 읽는다.
	b = 3; // 따라서 a = b = c = d = 5 도 성립한다.
	printf("a + b 는 : %d \n", a + b);
	printf("a - b 는 : %d \n", a - b);
	printf("a * b 는 : %d \n", a * b);
	printf("a / b 는 : %d \n", a / b); /*정수형 변수 연산 정수형변수는 언제나
									  정수로 유지된다. %f 넣는다고 실수값이 나오는 
									  것은 아니다.*/
	printf("a %% b 는 : %d \n", a % b); // %는 정수형 데이터에서만 계산가능
	return 0;
}

