Exercise 1 - Theory questions
-----------------------------
 
 ### What is the difference between concurrency and parallelism?
 >  Concurrency is when two or more tasks can start, run and complete in overlapping time. They don´t necessarily have to run at the same instant, ex. on a single-core machine. Parallellism is when tasks literally run at the same time, ex on a multicore processor.
 
 ### Why have machines become increasingly multicore in the past decade?
 > multi-core processor is a computer processor on a single integrated circuit with two or more seperate processing units, called cores, each of which reads and execute program instructions. in multi-core processors the processor can run ordinary instructions on seperate cores at the same time, which increasing overall speed for programs that support multithreading or other parallel computing techniques. 

 ### Why do we divide software (programs) into concurrently executing parts (like threads or processes)?
 (Or phrased differently: What problems do concurrency help in solving?)
 > the concurrency can be designed as independent processes working togheter on a specific composition. Can model processes in the outside world that happen concurrently. Can help with tackle complexity. 
 -the number of tasks completed in a given time in a give time to increase proportionally to the number of processor. 
 -High responsiveness for input/output

 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > As said in the task above, the current programming type can help with model actual processes that happens concurrently. It can also help with tackling complexity of programming problems. 
 The problem with this type of programming is that you need to decide how decied how to split the application up in smaller parts that can run on different threads, which is said to be harder than it sounds. So i would say both. 
 
 ### What is the conceptual difference between threads and processes?
 > Process mean a program is in execution, wheras thread means a segement of the process. A process takes more time to terminate than a thread. 
 
 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 > Fibers is lightweight thread that uses cooperative multitasking instead of preemptive multitasking. A running fiber must explicitly "yield" to allow another fiber to run. 

 A coroutine is a component that generalizes a subroutine to allow multiple entry points for suspending and resuming execution at certain locations.  Coroutine can exit by calling other coroutines, which may later return to the point where they were invoked in the orginal coroutine. 
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 > A goroutine is a lightweight thread managed by the Go runtime. The goroutines runs un the same address space, so access to shared memory must be synchroniced. 
 A goroutine are functions or methods that run concurrently with other functions or methods.
The pthread allows us to create multiple threads for concurrent process flow. Pthreads are defined as a set of C language programming types and procedure calls. 

 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
 > it sets the maximum number of the CPUs that can be executing simultaneously and returns the previous setting. 


 
 
 
 
