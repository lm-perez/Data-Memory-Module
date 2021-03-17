# Data-Memory-Module
The objective is to implement and simulate a simple memory unit which is capable of reading and writing data within a single clock cycle.

The data memory module has 256 words and each word has 32 bits. There are five inputs: clock (clk), address (addr), data input (data_in), and two enables (en & wen); and one output (data_out). The address input is where the data input goes (word). The two enable inputs determine if the data memory module will write or read. To write, en and wen has to both be high (1), the address and the data input are specified, and the function happens after the falling edge of the clock input. The output for this is 0. To read data, en has to be high (1) and wen has to be low (0), the address has to be specified while the data input has to be 0, the function will happen after the falling edge of the clock input and the output is the data inside the specified address. If en is 0 and wen is either 0 or 1, there is nothing happening; therefore, the output is 0. 
