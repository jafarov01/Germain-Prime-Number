#include <stdio.h>

int main()
{
	int temp, x, y, arr[1000], count = 0, prime = 0, check;

	printf("Enter x: ");
	scanf_s("%d", &x);
	printf("Enter y: ");
	scanf_s("%d", &y);
	if (x > y) //swapping x and y
	{
		temp = x;
		x = y;
		y = temp;
	}
	for (int i = x; i <= y; i++) // x = 5, y = 9,  i = 5 6 7 8 9
	{
		check = 1;
		for (int j = 2; j < i; j++) // i = 5, j = 2 3 4
		{
			if (i % j == 0) {
				check = 0;
			}
		}
		if (check == 1) {
			prime = i;
			for (int a = 2; a <= 2 * i; a++) // a = 2 3 4 5 6 7 8 9 10
			{
				if ((2 * i + 1) % a == 0)
				{
					check = 0;
				}
			}
			if (check == 1) {
				arr[count] = prime;
				count++;
			}
		}
	}

	for (int i = 0; i < count; i++)
	{
		printf("%d\t", arr[i]);
	}
	printf("\n");
	return 0;
}
