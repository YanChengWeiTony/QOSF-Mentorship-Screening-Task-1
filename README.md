# QOSF-Mentorship-Screening-Task-1

## File Description:
### 1. Task1.ipynb: 
It completes the requirements for the screening task 1. Specifically, the procedure is listed below

    a. It firstly generates a random state, phi.
    
    b. It then runs series of QC with different layers, and it compares the distance between the final state and phi. I use the package "qiskit.aqua.components.optimizers" and use "gradient descent" to search for the opitmal parameters to minimize the distance. I run from 1 to 9 layers, and the total time is about 2~3 hours.
    
    c. I then save it as a file, call "resultx.txt", where x is the index for the running case
    
    d. I also plot it and save as a "resultx.pdf"
    
    e, To give better understanding of its performance, I run the above procedure for three times, with index = 0, 1, 2. The final results are recorded in .txt file and plotted in " Plot_Results.ipynb'"
    
    
### 2. Task1-CNOT.ipynb
To conduct the Bonus task, I repeat the procedure in "Task1.ipynb" but replace the "CZ" gate with "CNOT" gate. Some notes are listed below.

    a. I then run it with the same states generated in "Task1.ipynb", for fair comparison. 

    b. I then save it as a file, call "resultx_CNOT.txt", where x is the index for the running case

    c. I also plot it and save as a "resultx_CNOT.pdf"
    

### 3. Plot_Results.ipynb
Here, I summarize the results generated in two above codes, and then I plot it for comparison.
    
    a. I plot all results in "result_all.pdf"
    
    b. I calculate the average and standard deviation for three cases, and compare the performance of "CZ" and "CNot" case. I plot all results in "result_avg_std.pdf".
    
    c. It looks like there is not significant difference in these two cases. Namely, we can replace CZ with CNOT. Surely, it will be nicer to sample more random statea, and I here simply use 3 cases only. The bottleneck is that single case takes too much time, and thus I am unable to sample more cases.
