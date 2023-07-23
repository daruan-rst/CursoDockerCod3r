# 8: What is Docker?

The lesson covers the meaning and basic concepts of Docker, a virtualization technology. However, Docker differs from traditional virtualization based on virtual machines. By brushing over these concepts, it is possible to understand Docker as a container management engine that allows testing and running applications in isolation from the host system.

## Characteristics of Docker
1. Not a traditional virtualization system:

- Docker does not use complete virtual machines like traditional virtualization. It works with containers, which are segregated and isolated processes from the host system.
- Containers have an isolated file system, allowing the execution of software with its specific dependencies and libraries within a controlled environment.

2. Container management engine:

- Docker is a container management engine that allows creating and managing containers using Docker.
- Containers are segregated and isolated processes from the host system, where applications can be tested and executed.
- Each container has its own isolated file system, providing a controlled environment for software execution.

3. Utilizes LXC (Linux Containers) services:

- Docker is based on LXC technology, which belongs to Linux. This means that Docker containers are based on Linux operating systems like Debian, Ubuntu, or Red Hat.
- Containers cannot be based on operating systems like Mac or Windows because they depend on the host system's kernel.

4. Open Source and written in Go:

- Docker is an open-source technology, which contributed to its significant growth.
- It was developed using the Go programming language created by Google.

5. System-level software (OS) virtualization:

- Docker uses software-based virtualization, meaning it is virtualization based on the operating system.
- Unlike traditional virtualization, Docker shares the host machine's kernel with containers, resulting in lower resource consumption, higher speed, and efficient isolation.

6. Host and containers share the kernel:

- Docker shares the host machine's kernel with containers but does not directly use the host's kernel.
- Additionally, some libraries and binaries are also shared, contributing to Docker's efficiency.

7. Packages software with various levels of isolation:

- Docker offers various levels of isolation for containers.
- It is possible to isolate the amount of memory, CPU usage, network, and file system for each container.
- Each container has its own IP address, allowing access through that address.
- File system isolation is fundamental for Docker's control and effective isolation, ensuring that processes run only within the container's file system.

Understanding these characteristics is essential to develop a solid understanding of Docker and delve into the specific concepts that will be covered in subsequent lessons.

