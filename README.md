#include <stdio.h>
double calculate_time(int t1, int t2, int t3) {
    double total_speed = (1.0 / t1) + (1.0 / t2) + (1.0 / t3);
    double time = 1.0 / total_speed;
    return time;
}
int main() {
    int t1, t2, t3;
    printf("Введіть три значення t1, t2, t3: ");
    scanf("%d %d %d", &t1, &t2, &t3);
    double time = calculate_time(t1, t2, t3);
    printf("Час, за який троє гостей з'їдять пиріг: %.2f годин\n", time);
    return 0;
}
