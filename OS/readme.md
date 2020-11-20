> Difference between process and thread?
* Process: Program which is under execution ,It has its own control block,stack and address space. using message passing and shared memory, process communicate between them. 
*  Thread: segment of process, it doesnot have a control block of its own. It shares parents control block code section data section and files are shared.Less context switch time.Process execution is faster f we use multiple threads because processes are run parallely using multiple threads.Each thread has its own stack space registers and PC.Communication between processes is easy compared to between the processes.
> Benefits of Multithreaded processes in OS?
* It increases responsiveness because multiple threads run parallely and since they have shared memory communication is easy and context switch time is also less when multiple threads are present more efficiency since all the tasks handled at the same time by worker threads.Cost is less compared to multiprocess.
> What is multi programming?
* Whenever a process goes for block/wait state the cpu remains idle in a non multi programming system, but in a multi programming system it is not like that cpu handles other processes also so more efficiency. Switching the processes
> What is multi processing?
* Multi Processing is used when we need to execute more than one process smultaneously. Having multiple processors
> What is multi Tasking?
* Multi Tasking is used to run multiple processes by defining a time quantum after which processes change
> Multi Threading example from gfg
* We can think of threads as child processes that share the parent process resources but execute independently. Now take the case of a GUI. Say we are performing a calculation on the GUI (which is taking very long time to finish). Now we can not interact with the rest of the GUI until this command finishes its execution. To be able to interact with the rest of the GUI, this command of calculation should be assigned to a separate thread. So at this point of time, 2 threads will be executing i.e. one for calculation, and one for the rest of the GUI. Hence here in a single process, we used multiple threads for multiple functionality.