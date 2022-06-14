# Complete Aws EC2 Tutorial With Node-Js
- EC2 Stands For Elastic Compute Cloud.
- Amazon EC2 Provides Scalable Computing Capacity In The Aws Cloud. Using Amazon EC2 Eliminates Your Need To Invest In Hardware Up Front, So You Can Develop And Deploy Applications Fa Steffic.
- You Can Use Amazon EC2 To Launch As Many Or As Few Virtual Server As You Need Configure Security And Networking And Manage Sotrage.
- Amazon EC2 Enables You To Scale Up Or Scale Down The Instance.
- Amazon EC2 Is Having Two Storage Options I.E. Ebs & Instance Store.
- Preconfigured Templates Are Available Know As Amazon Machine Image.
- Bydefault, When You Can Create An EC2 Account With Amazon, Your Account Is Limited To A Maximum 20 Instance Per EC2 Region With Two Default High I/O Instances.


## Types Of EC2
1. General Purpose (Balanced Memory)
2. Compute Optimized(More Cpu Then Ram)
3. Memory Optimized (More Ram)
4. Storage Optimized (Low Latency)
5. Accelerated Computing/Gpu(Graphics Optimized)
6. High Memory Optimized (High Ram, Nitro System)
7. Previous Generation



# General Purpose Instances:- 

- General Purpose Instances Provide A Balance Of Compute Memory And Networking Resources, And Can Be Used For A Variety Of Workloads.


## 3 SERIES IN GENERAL PURPOSE INSTANCES:- 

1. A SERIES (Medium, Large)
    1. A1
2. M SERIES (Large)
    1. M4 
    2. M5
    3. M5A
    4. M5AD
    5. M5F
3. T SERIES (Nano, Small, Medium & Large)
    1. T2
        1. T2 Micro(Free Tier Available)
    2. T3
    3. T3A

> Instance Available In Four Size Nano, Small, Medium & Large.

### A1- Instances
- A1-instances are ideally Suited for Scale-Out Workloads
that are Supported by the ARM Ecosystem.

- ARM Ecosystem of software partners provide customers a wide range of products to gets to market faster than the competition ARM Development boards are the ideal platform for accelerating the development and reducing the risk of new SoC Designs.

- These Instances are well suited for the following application:- 
    - webservers
    - caching fleets
    - distributed data stores
    - containerized micro services
    - application that requires arm instruction set 

> Microservice: it is a distinct method to developing software systems that tries to focus on building single function modules with well degined interfaces and operations.

> Caching is a high-speed data storage layer which stores a subset of data, typically transient in nature, so that future request for that data are served up faster.

### M Series:- 

Instance Available In M Series is M4, M5, M5a, M5ad and M5d.

#### M4 Instance
- The New My instances featuresaCustom Intel Xeon E5-2676 v3 Haswell processor Optimized Specifically For EC2.

```sh
VCPU --> 2 to 40(Max)
RAM --> 8GB to 160GB(Max.)
Instance Storage --> EBS Only(Elastic Block Storage)
```
#### M5, M5a, M5ad, M5d Instances:- 

- These instances provide an ideal cloud buffering a balance of compute memory and netwoking Resources for a Broad range or applications.

- this is mostly used in Gaming Server, Web server, small and medium.

```sh
VCPU --> 2 to 96(Max)
RAM --> 8GB to 384GB(Max.)
Instance Storage --> EBS Only(Elastic Block Storage) & NVMe SSD
```


> Amazon Elastic Block Store (Amazon EBS) provides block level storage volumes for use with EC2 instances. EBS volumes behave like raw, unformatted block devices. You can mount these volumes as devices on your instances.

> AWS Elastic Block Store (EBS) is Amazon's block-level storage solution used with the EC2 cloud service to store persistent data. This means that the data is kept on the AWS EBS servers even when the EC2 instances are shut down.


### T Series:- 

- these instances provide a baseline level of cpu performance with the abality to burst to a higher level when required by your workload
- an unlimited instances can sustain high cpu performance for any period of time whenever required 
- specially used for testing. its not for large task like website development or hosting. Not Provide good performance. Very Cheap any one can buy. 

- Used for:- 

    1. Website & Web App
    2. Code Repositories.
    3. Development, Build, Test.
    4. MicroServices.

```sh
VCPU --> 2 to 8(Max)
RAM --> 0.5GB to 32GB(Max)
BANDWIDTH --> 5 GBPS(Max)
```




# Compute Optimized

- Computer optimized instances are ideal for compute bound applications that benefit from high performance processors.

- Three types are available -->
1. C4
2. C5
3. C5n
> C3 Previous Instance in place of C3 now we can buy C5 which is 25% less cost then C3. 

- it only have C Series. Its cost effective. it provides parallel processing.



## C4

- C4 instances are optimized for Compute intensive Workloads and deliver Very Cost effective high performance
at a low Price per Compute Ratio.

    ```sh
    VCPU --> 2to 36
    RAM --> 375 to 60 GB
    Network --> BandWidth 10 Gbps 
    Storage --> EBS Only
    ```

- Use cases:- Webserver, Batch Processing, MMO Gaming, Video Editing


## C5

- C5 are optimized for compute-intensive workloads and delivers cost effective high performance at a low price per compute ratio.

- Powered by AWS Nitro System.
    ```sh
    VCPU --> 2 to 72
    RAM --> 4 to 192 GB
    Network --> BandWidth 25 Gbps 
    Storage --> EBS Only & NVMe SSD
    ```

- Use cases:- High Performance Webserver, Gaming, Video Encoding

> Note:- C5 supports max 25 EBS Volumes.
> C5 use Elastic Network Adapter
> C5 Uses new EC2 Hypervisor.


# Memory Optimized Instances:- 

- Memory Optimized Instances have three series.
    1. R Series
    2. X Series
    3. Z Series

## R Series

- R Series have R4,R5,R5ad and R5d Instances.

- High performance Relational (MySQL) and NoSQL(MongoDB,Cassandra) database.

- distributed web scale cache stores that procides in memory caching of key value type data.

- Used in financial services, Hadoop

```sh
VCPU --> 2 to 96
RAM --> 16GB to 768GB
Instance Storage --> EBS Only & NVMe SSD
```



## X Series

- X Series have X1, X1e Instances.

- Well suited for High Performance database, Memory intensive enterprise application Relational Database Workload, SAP HANA

- Electronic Design Automation

```sh
VCPU --> 4 to 128
RAM --> 122GB to 394GB
Instance Storage --> SSD
```

## Z Series

- Z Series have Z1d Instances.

- High Frequency z1d delivers a sustained all cors frequency of upto 4 0 GHz, the fastest of any cloud instances.

- AWS Nitro System, Xeon processor, upto 1.8TB of instances storage
.

```sh
VCPU --> 2 to 48
RAM --> 16GB to 384GB
Instance Storage --> SSD
```

> UseCase:- Electronic Design Automation and Certain database workloads with high per-core licensing cost.


# Storage Optimized Instances

- Storage Optimized Instances have three series.
    1. I Series
    2. D Series
    3. H Series


- Storage Optimized instances are designed for workloads that required high sequential read and write access to very large data sets on local storage.

- They are optimized to deliver tens of thousands of low latency. 

- Random I/O Operations per seconds(IOPS) to application.



## I Series 

- It have I3 and I3en Instances.

- High Frequency online transaction processing system(OLTP)

- Relational Database
- NoSQL database
- Distributed file system.
- Data warehousing application.

```sh

VCPU --> 2 to 96
RAM --> 16GB to 786GB
Local Storage --> NVMe SSD
Networking Performance --> 25GBPS to 100GBPS
Sequential Throughput
    Read: 16 GB/s
    Write: 64 GB/s(I3)
           8 GB(I3en)

```


## D Series 

- It have D2 instances.

- Well suited for the following:-

    - massive parallel processing(MVP) data warehouse.

    - Map reduce and hadoop distributed computing.

    - log or data processing app.

    ```sh

    VCPU --> 4 to 36
    RAM --> 30.5GB to 244GB
    Local Storage -->  SSD
    
    ```



## H Series 

- It have H1 Instances.

- the family feature upto 16TB of HDD based local storage, high disk thoughput and balance of compute & memory.

- well suited for app requiring sequential access to large amounts of data on direct attached instance storage.

- application that requires high throughput access to large quantities of data.

```sh

VCPU --> 8 to 64GB
RAM --> 32GB to 256GB
Storage --> HDD

```


# Accelerated Computing Instance 

- Accelerated Computing Instances have three series.
    1. P Series
    2. G Series
    3. F Series



## P Series

- It have P2 & P3 Instances.

- It have NVIDIA Tesla GPUs.

- Provide high bandwidth networking.

- upto 32 GB of memory per GPUs which makes them ideal for deep learning & computational fluid dynamics.

- P2 Instances 

    ```sh
    VCPU --> 4 to 64
    GPU --> 1 to 16 
    RAM --> 61 to 732GB
    GPU RAM --> 12GB to 192GB
    Network BW --> 25GBPS
    ```

- P3 Instances 

    ```sh
    VCPU --> 8 to 96
    GPU --> 1 to 8
    RAM --> 61 to 768GB
    Storage --> SSD & EBS
    ```

> Used in Machine Learning Database, Seismic Analysis, Genomicsm, Molecular Modeling, AI, Deep Learning.

> Note: P3 supports CUDA 9 & Open CL APIs. P2 Supports CUDA 8 and & Open CL 12 

## G Series

- It have G2 & G3 Instances.

- Optimized for Graphics Intensive  application
                       
- Well Suited for app like 3D Visualisation
- G3 Instances use NVIDIA Tesla
M60 GPU and provide a Cost Effective, high performance platform for Graphics applications.


```sh
VCPU --> 4 to 64
GPU --> 1 to 4
RAM -->  305 to 488GB
GPU Memory -->8 to 32 GB
Network Performance- 25 Gbps
```


- Used in-Video Creation Services, 3D Visualisation,Streaming Graphics-intensive application.

## F Series

- F1 Instances offers Customizable Hardware acceleration with Field Programmable Gate arrays(FPGA)

- Each FPGA Contains 2.5 million Logic Elements&6900 DSP engines
- Designed to accelerate Computationally intensive algorithms. Such as data flow or highly parallel Operations.

- It provides Fi Local NVM SSD Storage

```sh
VCPU --> 8 to 64
FPGA --> 1to8
RAM --> 122 to 976 GB
Storage --> NVMe SSD

```
> Used in Genomics Research, Financial analytics, Real time Video Procesong & Big data Search



# High Memory Instances 

- High Memory Instances are purpose built to run large-in-memory databases including production developments of SAP HANA the Cloud.

- Features:- 

    1.  Latest Generation Intel Xeon Pentium 8176M Processor. 

    2. 6,9,12 TB of instance  Memory, the Largest of any EC2 Instance.

    3. Powered by the AWS Nitro System a combination of dedicated hardware & lightweight hyperversion.

    4. Base metal performance with direct access to host hardware.

    5. EBS optimized by default at no additional cost.

    Model No:- U-6tb1 metal, U-9tb1 metal & U-12tb1 metal

    6. Network performance - 25GBPS 
       Dedicated EBS Bandwidth - 14GBPS

    7. Each Instance offer 448 logical processor

> Note:- High Memory Instances are bare metal instances and do not run on a hyperversion.

> Only Available under dedicated host purchasing category(for 3yr term)

> OS Directly on Hardware.


# Previous Generation Instances

- It have T1, M1, C1, CC2, M2, CR1, CG1, I2, HS1, M3, C3 & R3.