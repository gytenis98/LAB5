LAB5
====
##Functionality
1st program functionality verified by Dr. Neeble on Friday, 18 April.

2nd program functionality on PRISM Simulator and on FPGA verified by Capt. Silva on Thursday 24 April. 


##1st Program

I followed the Lab 5 instructions and most of the lab was straigt forward. 
Program worked as it suppost to. It counts from "0", "9", "8", "a", "b", "c", "d", "f" and back to "0" again. And stops at "0". Counting happens only when the number is negative. If number is possitive, then program goes straight to "jump 0" and stops. 

![alt tag](http://s13.postimg.org/kmrmg8j6f/image.jpg)

#####35-45 ns - fetch
#####45-55 ns - decode
#####55-65 ns - immediate execute
#####65-75 ns - fetch
#####75-85 ns - decode
#####85-95 ns - decode addr low
#####95-105 ns - direct I/O execute
#####105-115 ns - fetch
#####115-125 ns - decode
#####125-135 ns - decode LoAddr


![alt tag](http://s29.postimg.org/zf1p7jdev/image.jpg)

#####135-145 ns - decode hiAddr
#####145-155 ns - jmp execute
#####155-165 ns - fetch


##Answer to prism questions
#######1)   
            a.PCLd-high
            b.IRLd-high
            c.ACCLd-low
#######2) 
            Asserted: MARLoLd, PCLd,MemSel_L. 
            Next state will be: Direct IO Execute.
#######3) jmp,jn,jz
#######4) It is important because when it is active, value in accumulator will change. It need to be active so the new value from the addition could be put into accumulator.
#######5) To have extra instruction one has to add extra bit. Also, data bus should get bigger to store the extra bit. I THINK (but not sure) that registrars should get bigger too.
