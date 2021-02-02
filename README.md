#include <stdio.h>
#include <string.h>
#include <stdlib.h>

const int NUMBER_OF_GRADES = 9;
const int scores[NUMBER_OF_GRADES] = {95, 90, 85, 80, 75, 70, 65, 60, 0};
const char *grades[NUMBER_OF_GRADES] = {"A+", "A", "B+", "B", "C+", "C", "D+", "D", "F"};
int main(void)
{
    printf("학점 프로그램\n 종료를 원하면 '999'를 입력 \n [학점 테이블]\n")
    printf("A+    A    B+    B    C+    C    D+    D    F\n 95    90    85    80    75    70    65    60    0\n");
    while (true)
    {
        int end = 0;
        int score = get_int("성적을 입력하세요 : ");
        for (int i = 0; i<9, i++)
        {
            int nimber = i;
            if (score == 999)
            {
                printf("프로그램을 종료합니다.\n");
                end = 1;
                break;
            }
            if (score <= 100 && 0 <= score && score >= scores[number])
            {
                printf("학점은 %s입니다. \n", grade[number]);
                break;
            }
            if (score > 100 && score < 0)
            {
                printf("성적을 올바르게 입력하세요 (0 ~ 100)\n");
                break;
            }
        }
        if (end ==1)
        {
            break;
        }
    }
}
