How to check if some character (`|` pipe in this case) is escaped with preceding escape characters `\`? Or it is multiple escape characters which escape each other? Recursion helps in this case.
Here is an example in C:  

    #include <stdio.h>
    #include <stdlib.h>
    #include <string.h>

    int is_escaped(char * string, char ** string_start) {
        if( string == NULL ||
                &string == string_start ||
                *(string - 1) != '\\' ) {
            return 0;
        }

        return !is_escaped(string - 1, string_start);
    }

    int main(int argc, char ** argv) {
        char * original = "abc\\|def";

        printf("original='%s'\n", original);
        printf( "escape it='%d'\n",
                is_escaped(strstr(original, "|"), &original) );

        return 0;
    }

