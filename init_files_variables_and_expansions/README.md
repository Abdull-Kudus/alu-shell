#SCRIPTS EXPLANATIONS OF THE SHELL, INIT FILES, VARIABLES AND EXPANSIONS



1. Hello you (1-hello_you): $USER is a built-in environment variable containing the current username, echo "hello $USER" prints "hello " followed by the username and variable expansion happens inside double quotes. The $USER is set by the system at login and variable expansion using $VARIABLE_NAME syntax
2. The path to success (2-path): $PATH contains current PATH (colon-separated directory list), "$PATH:/action" appends :/action to existing PATH, export makes the change available to the current shell and child processes and /action becomes the last directory searched for commands
3. If the path be beautiful (3-paths): echo $PATH outputs PATH variable (directories separated by colons), tr ':' '\n' replaces every colon with newline (one directory per line) and wc -l counts lines = number of directories.
4. Global variables (4-global_variables): printenv displays all environment variables, Shows only exported/global variables (not local shell variables) and output format: VARIABLE_NAME=value
5. Local variables: set command displays all shell variables (local, environment) and functions
6. Local variable: Creates a local variable BEST with value "School" and Local variables are only available in the current shell
7. Global variable: export makes the variable available to child processes and reates a global/environment variable
8. True knowledge: Uses arithmetic expansion $(()) to add 128 to TRUEKNOWLEDGE. The result is: 128 + 1209 = 1337
9. Divide and rule: Performs integer division using arithmetic expansion….42784 / 32 = 1337
10. Love exponent breath: Uses ** for exponentiation in arithmetic expansion…4^3 = 64
11. Binary to decimal: 2# prefix tells bash to interpret the number as base 2. It converts binary to decimal
12. Combinations: Brace expansion {a..z}{a..z} generates all combinations. tr ' ' '\n' converts spaces to newlines while grep -v oo excludes "oo"
13. Print float (13-print_float): printf "%.2f\n" "$NUM" formats the number with exactly 2 decimal places, %.2f is the format specifier: %f = floating point number, .2 = exactly 2 decimal places, \n = newline character, Quotes around "$NUM" handle cases where NUM might be empty or contain spaces, Format specifiers control output precision
14. Decimal to hexadecimal (14-decimal_to_hexadecimal): printf "%x\n" "$DECIMAL" converts decimal to lowercase hexadecimal, %x format specifier converts to hexadecimal (lowercase)
15. ROT13: tr command performs character translation which maps A-Z to N-Z,A-M and a-z to n-z,a-m (13-character shift)
16. Odd lines: paste - - pairs consecutive lines and cut -f1 extracts first field (odd-numbered lines)
17. Water and stir: Complex base conversion problem, converts WATER from base "water" (5-character base) to decimal, converts STIR from base "stir." (5-character base) to decimal, adds them together and converts result to base "bestchol" (8-character base) using octal as intermediate
