# Distributed data processing system

## Why distributed data processing system

Data processing system generally are developed with a goal of processing lots of data (commonly terms as **Big Data**)

Size of data can vary from TB to PB to more.

Hence we need to process data (Big data) in multiple systems(servers, nodes) *as one system may not be capable of processing these huge data*.

Alternatively processing every data in a centralized server is known as **centralized data processing system**.

Centralized data processing systems are not popular due to many reason that you may have already guessed.

## Characteristics of distributed systems

- Basic idea is that **each server work in conjunction with other server in the cluster**.
- The servers are **managed by a centralized master node**, and it takes care of managing, distributed load.
- Each node is capable of **processing data in parallel**.
- Clusters or entire **setup is highly scalable and available**.
