## Code:
```c
#include <stdio.h>

void main() {
    char sentence[1000];
    int vowels = 0, consonants = 0, spaces = 0, i;

    printf("Enter a sentence: ");
    fgets(sentence, sizeof(sentence), stdin); // fgets used to read whitespaces, scanf doesn't read whitespaces

    for (i = 0; sentence[i] != '\0'; i++) {
        char ch = sentence[i]; // for easiness

        if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
            ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
            vowels++;
        } else if ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z')) {
            consonants++;
        } else {
            spaces++;
        }
    }

    printf("Vowels: %d\n", vowels);
    printf("Consonants: %d\n", consonants);
    printf("Whitespaces: %d\n", spaces);
}
```
## Algorithm:
> Will be updated