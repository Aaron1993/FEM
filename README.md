# FEM
FEM is a Fast and Efficient short read Mapper. 

## Usage
Currently, we provide binaries compiled with gcc 5.3.0 on CentOS 7.2. The source code will be available soon.

### Indexing
```
FEM index <window size> <step size> <reference.fa> 
```

### Mapping
```
Usage:   FEM align [options] 

Options:
         -e        INT    error threshold 
         -t        INT    number of threads 
         -f        STR    seeding algorithm: "g" for group seeding and "vl" for variable-length seeding 
         -a               use one additional q-gram for filter

Input/output: 
         --ref     STR    Input reference file
         --read    STR    Input read file
         -o        STR    Output SAM file 
```


## Parameters
To reduce mapping time, we recommend to use the smallest step size as long as the index can fit into the memory. In next version, FEM will choose the step size according to given memory adaptively. 

## Contacts
Weiguo Liu <br />
Email: weiguo.liu@sdu.edu.cn

Haowen Zhang <br />
Email: hwzhang@gatech.edu

We welcome any bug report and suggestion.
