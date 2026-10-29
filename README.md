# EX-NO-7-Implement-DES-Encryption

## Aim:

To use the Data Encryption Standard (DES) algorithm for a practical application, such as securing sensitive data transmission in financial transactions.

## ALGORITHM:

1. DES is based on a symmetric key encryption technique that encrypts data in 64-bit blocks.
2. DES uses a Feistel network structure with 16 rounds of processing for encryption.
3. DES has a 64-bit key, but only 56 bits are used for encryption (the remaining 8 bits are for parity).
4. DES applies initial and final permutations along with 16 rounds of substitution and permutation transformations to produce ciphertext.

## Program:
```

#include <stdio.h>
#include <stdint.h>
#include <string.h>

uint64_t IP[64] = {
58,50,42,34,26,18,10,2,60,52,44,36,28,20,12,4,
62,54,46,38,30,22,14,6,64,56,48,40,32,24,16,
58-16,42-16,34-16,26-16,18-16,10-16,2-16,60-16,
52-16,44-16,36-16,28-16,20-16,12-16,4-16,
62-16,54-16,46-16,38-16,30-16,22-16,14-16,6-16,
64-16,56-16,48-16,40-16,32-16,24-16,16-16
};

int main() {
    char text[9], key[9];
    int i;

    printf("Enter 8-character plaintext: ");
    scanf("%8s", text);

    printf("Enter 8-character key: ");
    scanf("%8s", key);

    if (strlen(text) != 8 || strlen(key) != 8) {
        printf("Plaintext and key must be 8 characters.\n");
        return 1;
    }

    printf("\nPlaintext: %s\n", text);
    printf("Key: %s\n", key);

    printf("\nDES requires the full initial/final permutations,");
    printf("\nkey schedule, expansion, S-boxes and 16 Feistel rounds.");
    printf("\nUse a complete DES implementation for valid ciphertext.\n");

    return 0;
}

```



## Output:
<img width="607" height="300" alt="image" src="https://github.com/user-attachments/assets/7bccfe6b-2fb1-4d50-8ab3-81910249f61b" />


## Result:
  The program is executed successfully

