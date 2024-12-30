# VSD-RiscV
-------------------------------------------------

<details>
<summary><b>Task 1:</b> Task 1</summary>

## C based lab
1. Install Leafpad in terminal.

   
   Type:
   ```
	sudo snap install leafpad
	```
   ![1](https://github.com/user-attachments/assets/71f822f1-d06e-4e7f-86d5-907d6a803bc4)

2. Type  Password which is invisible.
   ```
	vsdiat
	```
   ![2](https://github.com/user-attachments/assets/f4b495fe-9a47-47e4-8839-87dd556d4ffe)

3. Enter these commands in Terminal to create the file in leafpad:
   ```
	cd
	```
   ```
   leafpad sum1ton.c &
	```
   ![image](https://github.com/user-attachments/assets/15a33703-b677-49e6-bcf6-1f79a58c0925)

4. Type this Program is Leafpad
   ```
	#include <stdio.h>
   int main() {
    int i, sum = 0, n = 5;
    for (i = 1; i <= n; ++i) {
        sum += i;
    }
    printf("sum of numbers from 1 to %d is %d\n", n, sum);
    return 0;
   }

	```
   ![3](https://github.com/user-attachments/assets/395709d8-d198-452b-89ab-e11791283db9)


6. Result of the program:

   ![4](https://github.com/user-attachments/assets/ba9d132e-136e-4eac-a9c3-e01865de6486)
   ![5](https://github.com/user-attachments/assets/2018dc2e-dd75-4e16-9cc0-477d98079f9f)
   ![6](https://github.com/user-attachments/assets/7da14d9e-901b-481c-9233-60dd19b7a74b)
## RISC based lab

1. Enter this CAT command in terminal.
    ```
    cat sum1ton.c
	```
2. Then Program is displayed in the terminal.
3. Now run this following command in terminal  to compile the code in riscv64 gcc compiler:
    ```
    riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
	```
    
4. Enter this command in terminal.
    ```
	ls -ltr sum1ton.o
	```
    ![1](https://github.com/user-attachments/assets/142f5936-7c84-4863-8ddb-860187c032f4)

5. Open the new Terminal tab and run this command.
   
    ```
	riscv64-unknown-elf-objdump -d sum1ton.o
	```
6. # Objdump using O1 format
![2](https://github.com/user-attachments/assets/f4705547-c769-48ef-b284-802e89a252cb)
![3](https://github.com/user-attachments/assets/6c218bc9-7aff-4bc6-87d9-e519cff8f9d1)
