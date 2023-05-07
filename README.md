Download Link: https://assignmentchef.com/product/solved-parallelcomputing-assignment-5-gpu-basics
<br>



<h1>Preliminary</h1>

To use CUDA, add module load cuda in your .bashrc or .bash profile on mamba.

To submit a CUDA job, use -lnodes=1:ppn=7:gpus=1

Processing on the GPU can be asynchronous, which can lead to time measurement of 0 seconds. Use cudaDeviceSynchronize() to ensure previously submitted tasks have completed.

<h1>1           Polynomial expansion</h1>

(Code for polynomial expansion on the CPU is given.)

<strong>Question: </strong>Write a simple CUDA code that allocates and fill an array on the CPU and transfer it to the GPU. (Take array size as a parameter)

<strong>Question: </strong>Compute the polynomial expansion of each element of the array on the GPU. (Take block size and degree of the polynomial as a parameter.)

<strong>Question: </strong>Bring the results back on the CPU and confirm the GPU code is correct.

<h1>2           Measurements</h1>

<strong>Question: </strong>Measure PCI-express latency. (That is the time for an array of size 1.)

<strong>Question: </strong>Measure PCI-express Bandwidth. (The initial memory copy for different size of the array.)

<strong>Question: </strong>Measure GPU memory bandwidth. (Exclude memory copies and use a low degree polynomial.) <strong>Question: </strong>Measure GPU flops rating. (Exclude memory copies and use a high degree polynomial.)