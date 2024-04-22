1. Importing Libraries
numpy: For numerical operations, especially creating and manipulating arrays.
threading: For creating and managing threads to execute tasks concurrently.
time: For time-related functions such as measuring execution time.
psutil: For getting system-related information like CPU usage.
pandas: For creating and manipulating data frames.
matplotlib.pyplot: For data visualization, particularly plotting graphs.

2. Generating Constant Matrix
constant_matrix: Generates a 1000x1000 matrix filled with random integers between 0 and 9.

3. Function to Generate Random Matrices
matrices: Creates a list of 100 matrices, each having dimensions 1000x1000 and filled with random integers between 0 and 9.

4. Matrix Multiplication Function
matmul: Function to perform matrix multiplication of the constant matrix with a subset of matrices from the list.
st and ed: Define the starting and ending index of the subset of matrices to be multiplied.
cpu: List to store CPU usage during matrix multiplication.

5. Storing Time taken
data: Creates a list of 6, which will store the time taken by threads.

6. Main Execution
This section initiates the matrix multiplication task using multiple threads.
It iterates over a range of thread counts from 1 to 6.
For each thread count, it calculates the number of matrices each thread will handle (size), distributing them evenly, from st to ed.
It then creates and starts threads, each calling the matmul function with appropriate arguments.
After all threads finish execution, it collects CPU usage data from each thread and calculates the average CPU usage.
It measures the time taken for the entire operation and stores it in the data list.

7. Data Visualization
Converts the data list into a numpy array, reshapes it, and then creates a DataFrame for better organization.
Plots the execution time against the number of threads using Matplotlib.
Displays the plot showing how execution time varies with the number of threads.

This code demonstrates the utilization of multithreading for matrix multiplication and analyzes its impact on execution time and CPU usage. The report provides insights into how increasing the number of threads affects the overall performance of the task.
As we can see, the graph first decreases and then increases, showing the variation of number of threads to the time taken for matrix multiplication.

CPU USAGE during THREAD 1:
 
