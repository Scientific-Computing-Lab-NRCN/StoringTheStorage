# Assessing the Use Cases of Persistent Memory in High-Performance Scientific Computing
As the High Performance Computing (HPC) world moves towards the Exa-Scale era, huge amounts of data should be analyzed, manipulated and stored. In  the traditional storage/memory hierarchy, each compute node retains its data objects in its local volatile DRAM. Whenever the DRAM’s capacity becomes insufficient for storing this data, the computation should either be distributed between several compute nodes, or some portion of these data  objects must be stored in a non-volatile block device such as a hard disk drive (HDD) or an SSD storage device. These standard block devices offer  large and relatively cheap non-volatile storage, but their access times are orders-of-magnitude slower than those of DRAM. Optane™  Data Center Persistent Memory Module (DCPMM), a new technology introduced by Intel, provides non-volatile memory that can be plugged into standard memory bus  slots (DDR DIMMs) and therefore be accessed much faster than standard storage devices. In this work, we present and analyze the results of a comprehensive performance assessment of several ways in which DCPMM can 1) replace standard storage devices, and 2) replace or augment DRAM for  improving the performance of HPC scientific computations. To achieve this goal, we have configured an HPC system such that DCPMM can service I/O operations of scientific applications, replace standard storage devices and filesystems (specifically for diagnostics and checkpoint-restarting), and  serve for expanding applications’ main memory. We focus on keeping the scientific codes with as few changes as possible, while allowing them to access the NVM transparently as if they access persistent storage. Our results show that DCPMM allows scientific applications to fully utilize nodes’ locality by providing them with sufficiently-large main memory. Moreover, it can also be used for providing a high-performance replacement  for persistent storage. Thus, the usage of DCPMM has the potential of replacing standard HDD and SSD storage devices in HPC architectures and enabling a more efficient platform for modern super computing applications. \
**This repository contains experimental results and some codes and scripts used in our work.**
