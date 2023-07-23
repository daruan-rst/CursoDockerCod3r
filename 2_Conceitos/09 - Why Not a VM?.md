# 9: Why Not a VM?

In this lesson, the question of why not use a virtual machine (VM) instead of Docker was addressed. Although VMs have revolutionized the technology market and are widely used, Docker offers distinct benefits. Docker is a container-based virtualization technology that provides advantages in terms of resource consumption.

## Characteristics of Docker
1. Advantages of virtual machines:

- System Isolation: VMs allow complete isolation of the operating system and applications.
- Elasticity: It is possible to adjust the amount of resources allocated to a VM according to the need.

2. Advantages of Docker compared to VMs:

- Reduced Resource Consumption: Docker containers consume fewer resources compared to a complete VM. The container startup time is very fast, around seconds.
- Resource Sharing: Docker shares the operating system kernel with containers, resulting in resource savings, such as memory.
- Ease of Use: Docker provides a user-friendly access layer, making it easier to create and manage containers.

3. Comparison between Docker and VMs:

- Both have a physical server as a base and an installed operating system.
- In the case of VMs, each has a complete operating system, while Docker containers share the host's operating system kernel.
- Docker containers run as isolated processes with isolated file systems, allowing the execution of applications with their dependencies in controlled environments.
- Docker uses LXC (Linux Containers) technology to manage containers, providing a friendly layer to access them.

Docker offers most of the advantages of VMs, such as isolation and elasticity, while consuming fewer resources. However, there are specific cases where VMs are necessary, such as when running non-Linux operating systems or using specific technologies available only in certain VMs.

Docker has simplified the use of container technology, making it more accessible and popular. Its adoption has grown rapidly, being widely used in both development and production environments.

