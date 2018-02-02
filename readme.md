### Simple Agent

## file construct
### header
---------------------------------------
header MICRO -> SYS header -> defined header ->  define MICRO --> struct  --> function

## simple support

### timer

implement by timewheel. 
problem: without execute timeout check,  execute over duration check.

### worker

implement use pthread.  
problem: use pthread_barrier_t which some problem on mac os. 


### mutli io

implement by epoll. 
problme: others multi io not support like "select/poll/keque". 

###  protocol

implement use binary protocl just lick |type|magic|len|pay_load|. 
simple to scala.


### sstring use

like sds library, but more simple.

### smalloc

smalloc use the memory like system, with a head metric message on memory head and with monitor.

### advantage
- all is simple
- all implement by self

## notice
- cannot build on mac os which not support pthread_barrier_t
