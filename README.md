# Matrix Addition With Unified Memory
## Aim:
To demonstrate matrix addition using CUDA programming with unified memory.

## Procedure:
1. Allocate unified memory for matrices A, B, and C.
2. Initialize matrices A and B with appropriate values.
3. Define the grid and block dimensions for the CUDA kernel.
4. Launch the CUDA kernel to perform matrix addition.
5. Synchronize the device to ensure all CUDA operations are completed.
6. Print the result matrix C.
7. Free the allocated device memory.

## Output:
![image](https://github.com/Kavya-Bollineni22/PCA-Matrix-Addition-With-Unified-Memory/assets/75235813/01038d16-b6c6-4f07-9a14-458c9d7bebcd)
![image](https://github.com/Kavya-Bollineni22/PCA-Matrix-Addition-With-Unified-Memory/assets/75235813/d187a3b8-373f-485b-a52d-c68968cc507e)
![image](https://github.com/Kavya-Bollineni22/PCA-Matrix-Addition-With-Unified-Memory/assets/75235813/81e4f3bc-a3d7-46e9-a250-d1c1b2917b10)

## Result:
The memset function calls are not necessary in this program. They were originally used to set the memory blocks for matrices A, B, and C to zero. However, the subsequent initialization loops already assign specific values to each element of the matrices, overwriting the previous values set by memset. Removing the memset calls does not affect the correctness of the program and has no significant impact on its performance. It is good practice to remove unnecessary code to improve code readability and maintainability.
The result printed to the console, showing the elasped time in the Host and the GPU to compare their performance.
