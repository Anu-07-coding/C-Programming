String Handling

<html>
<head>
<title>Programming</title>
<link href= "design.css" rel="stylesheet" type="text/css">
</head>
<body>
<h2>String Handling Functions</h2>

<pre>
#include <stdio.h>
#include <string.h>

int main() {

    char str1[100], str2[100], str3[100];
    char str4[50]="APPLE", str5[50]="mango";
    int len;

    // 1. strcpy() - Copy string
    strcpy(str1, "Hello");
    printf("str1 after strcpy: %s\n", str1);

    // 2. strlen() - Length of string
    len = strlen(str1);
    printf("Length of str1: %d\n", len);
    
    // 3. strcmp() - Compare two strings
    int result = strcmp(str1, str2);
    if (result == 0) {
        printf("str1 and str2 are equal.\n");
    } else if (result > 0) {
        printf("str1 is greater than str2.\n");
    } else {
        printf("str1 is less than str2.\n");
    }

    // 4. strcat() - Concatenate two strings
    strcpy(str2, " World");
    strcat(str1, str2);
    printf("str1 after strcat: %s\n", str1);

    // 5. strncat() - Concatenate n characters from second string to first string
    strcpy(str3, " Everyone");
    strncat(str1, str3, 4); // Concatenate only first 4 characters of str3
    printf("str1 after strncat: %s\n", str1);
    
    // 6. strlwr() - Convert the string to lowercase
  
    printf("String in lowercase: %s\n",   strlwr(str4));

    // 7. strupr() - Convert the string to uppercase
   
    printf("String in uppercase: %s\n",  strupr(str5));

    return 0;
}
</pre>
</body>
</html>

<img width="338" alt="string handling1" src="https://github.com/user-attachments/assets/95f36fcd-24d4-4ee9-8cf3-94cbb89ef423" />
<img width="389" alt="string handling" src="https://github.com/user-attachments/assets/828edf1e-31c2-46c3-ac0e-38db2e7aa1d6" />
