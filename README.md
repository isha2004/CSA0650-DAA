#include <stdio.h>
#include <string.h>

#define MAX 100

int main() {
    char str[MAX], reversedStr[MAX];
    int length, i, isPalindrome = 1;
    printf("Isha Singh-192210252\n");
    printf("Enter a string: ");
    gets(str);

    length = strlen(str);

    for (i = 0; i < length; i++) {
        if (str[i] != str[length - i - 1]) {
            isPalindrome = 0;
            break;
        }
    }

    if (isPalindrome) {
        printf("The string is a palindrome.\n");
    } else {
        printf("The string is not a palindrome.\n");
    }

    return 0;
}
