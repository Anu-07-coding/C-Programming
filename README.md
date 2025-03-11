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

Errors

<html>
<head>
<title>Errors</title>
<link rel="stylesheet" href="design.css" type="text/css">
</head>

<body>
        <h1>Errors</h1>
    </header>
    <h2>Code</h2>
    <hr>
    <h2> Syntax Error</h2>
    <pre>
        #include <stdio.h>

            int main() {
               print ("Hello World");
            }
            
            </pre>
    <h2>Output</h2>
    <hr>
    <img src="syntax.png" alt="Output of the code" width= 500 height=100>

    </pre>
    <h2> Runtime Error</h2>
    <hr>
    <pre>
        #include <stdio.h>
                int main() {
                 int a;
                 a=2/0;
                 printf ("%d",a);
                }
                
            </pre>
    <h2>Output</h2>
    <hr>
    <img src="runtime.png" alt="Output of the code" width= 500 height=100>

    </pre>
    <h2> Logical Error</h2>
    <hr>
    <pre>
       
        #include <stdio.h>

            int main() {
           int a=1,b=4;
           int sum;
           sum= a-b;
           printf("Sum: %d",sum);
            }

            </pre>
    <h2>Output</h2>
    <hr>
    <img src="logical.png" alt="Output of the code" width= 500 height=100>

    </pre>
    <h2> Semantics Error</h2>
    <hr>
    <pre>
        #include <stdio.h>

            int main() {
                int a = 0;
                2 = a;
                printf ("%d",a);
                        }
            
            
            </pre>
    <h2>Output</h2>
    <hr>
    <img src="semantic.png" alt="Output of the code" width= 500 height=100>

    </pre>
    <h2> Linker Error</h2>
    <hr>
    <pre>
        #include<stdio.h>
            main() {
                int x = 52;
                int y = 0;
                printf("Div : %f", x/y);
            }
            </pre>
    <h2>Output</h2>
    <hr>
    <img src="linker.png" alt="Output of the code" width= 300 height=20>

    </pre>
</body 
</html>

<img width="554" alt="e1" src="https://github.com/user-attachments/assets/481221bb-67c2-4597-9673-683b9b512779" />
<img width="551" alt="e2" src="https://github.com/user-attachments/assets/a5e392b4-a0d2-4541-b0b6-58d0f0bf108f" />
<img width="551" alt="e3" src="https://github.com/user-attachments/assets/d5524136-c034-41c9-8834-843c5c0e8d47" />
