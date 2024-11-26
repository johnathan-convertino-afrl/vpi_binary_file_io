# VPI binary file io
### read and write binary functions for VPI

![image](docs/manual/img/AFRL.png)

---

   author: Jay Convertino   
   
   date: 2023.01.01  
   
   details: Read and write binary file functions for VPI. This is threaded and does all file IO outside of the simulation function call.   
   
   license: MIT   
   
---

### Version
#### Current
  - V1.0.0 - initial release

#### Previous
  - none

### DOCUMENTATION
  For detailed usage information, please navigate to one of the following sources. They are the same, just in a different format.

  - [vpi_binary_file_io.pdf](docs/manual/vpi_binary_file_io.pdf)
  - [github page](https://johnathan-convertino-afrl.github.io/vpi_binary_file_io/)

### DEPENDENCIES
#### Build
  - AFRL:utility:sim_helper
  - AFRL:utility:generators:1.0.0

### COMPONENTS
#### SRC

* binary_file_io.c
* binary_file_io.h
* binary_file_io.sft
* read_binary_file.c
* read_binary_file.h
* write_binary_file.c
* write_binary_file.h
  
#### TB

* tb_vpi.v
* count_test.bin
* rand_test.bin

### FUSESOC

* fusesoc_info.core created.
* Simulation uses icarus to run data through the core.

#### TARGETS

* RUN WITH: (fusesoc run --target=sim VENDER:CORE:NAME:VERSION)
  - default (for IP integration builds)
  - sim
  - sim_rand_data
  - sim_8bit_count_data
