---
title: Projects
description: Programming and computer science projects
slug: projects
date: 2023-05-20 00:00:00+0000
toc: true
#image: cover.jpg
#categories:
#    - Example Category
#tags:
#    - Example Tag

#Welcome to Hugo theme Stack. This is your first post. Edit or delete it, then start writing!

#For more information about this theme, check the documentation: https://docs.stack.jimmycai.com/

#Want a site like this? Check out [hugo-theme-stack-stater](https://github.com/CaiJimmy/#hugo-theme-stack-starter)

#> Photo by [Pawel Czerwinski](https://unsplash.com/@pawel_czerwinski) on [Unsplash](https://#unsplash.com/)

---

## Secure File Storage

![ ](cloud.jpg)

Through this API, users can authenticate themselves with a server to upload and download files that are stored and transmitted using end-to-end encryption. Users can also share files with other users, revoke their access, and download shared files. Under the assumption that an adversary can eavesdrop network traffic and modify the dataserver, this API still manages to provide confidentiality, integrity, and efficiency. From **threat modeling** to security analysis, this project considers principles of **secure software development** such as defense in depth and security by design.

**Timeline:** April - May 2023  
**Technologies:** Python, GitHub, Visual Studio

## Private Information Retrieval

![ ](pir.jpg)

As we outsource more of our data storage to cloud services, we need to make sure it's not only encrypted, but that the way in which we access it doesn't reveal unnecessary information to the server. This private information retrieval scheme uses **somewhat homomorphic encryption** to allow a client to retrieve database entries without the server learning which entry is being sent. Data is stored in a **hypercube data store** whose dimension and side length optimize the tradeoff between communication and computation. Using the BFV homomorphic encryption protocol, the server computes an encryption for the entry specified by the client's selection vector.

**Timeline:** April 2023  
**Technologies:** C++, CryptoPP, Microsoft SEAL

## Secure Two-Party Computation

![ ](yao.jpg)

By making use of **Yao's Garbled Circuits**, this program allows two parties to jointly compute any Boolean circuit without learning the other party's inputs. The garbler samples random labels for each wire and generates a garbled circuit for each gate. The evaluator runs an **Oblivious Transfer** protocol to retrieve the labels corresponding to their inputs, and then evaluates the circuit gate by gate. Circuits are specified using Bristol Format which consists of AND, XOR, and NOT gates. This program showcases how secure MPC enables joint analysis of distributed data while preserving its privacy.

**Timeline:** March - April 2023  
**Technologies:** C++, CryptoPP, Docker, Visual Studio

## Anonymous Online Voting

![ ](vote.jpg)

Four parties come together to form a secure voting platform: Arbiters generate election parameters and decrypt the final result, a Registrar issues voting certificates, a Tallyer checks that votes are valid, and the voters themselves cast the votes. I use non-interactive **Zero-Knowledge Proofs** to establish a framework of trust by ensuring that votes are generated correctly, and that the final results are honest. Votes are encrypted using additive homomorphic encryption and partially decrypted using **threshold ElGamal** before they're combined to retrieve the final result.

**Timeline:** March 2023  
**Technologies:** C++, CryptoPP, Docker, Visual Studio

## Public Key Infrastructure

![ ](certificate.jpg)

This client-server authentication platform leverages **digital signatures** in order for a central verification authority to issue certificates that authenticate users' public keys. Clients log in to a server using a password and two-factor authentication response to obtain a certificate that verifies their identity when communicating with other users. Passwords are hashed using a salt and pepper before being stored in a SQL database. This program achieves an authenticated key exchange that is secure against **man-in-the-middle attacks**.

**Timeline:** February - March 2023  
**Technologies:** C++, Docker, Visual Studio, SQLite

## Secure Communication Framework

![ ](signal.jpg)

The most fundamental problem in cryptography is that of establishing a **secure communication channel** that provides both message confidentiality and integrity. This program accomplishes just that. Two clients connect to each other to exchange encrypted and verified text messages through a command line interface. A **Diffie-Hellman ratchet** ensures keys are changed every time the direction of communication switches. The following cryptographic parameters are used – Key Exchange: Diffie-Hellman and HKDF. Encryption: 256-bit AES in CBC mode with random IV. Message Authentication: HMAC-SHA256 with salt.

**Timeline:** February 2023  
**Technologies:** C++, CryptoPP, Docker, Visual Studio

## Thread Safety and Synchronization

![ ](clock.jpg)

We like threads to cooperate by using shared memory. But what happens when two threads try to concurrently access the same memory? This project examines different ways of resolving race conditions and the **critical section problem**. Noun and adjective generators initialize threads that must share structures in a bounded buffer before they can be printed to the screen. In order to ensure mutual exclusion of memory among threads, I used **semaphores**, mutexes, and condition variables.

**Timeline:** January - May 2022  
**Technologies:** EOS Linux, POSIX System Calls, Von Neumann Architecture

## Data Structures and Algorithms Library

![ ](structures.jpg)

This Java library of over 30 data structures and algorithms demonstrates the importance of **algorithmic complexity** in relation to the choice of data structures. In it, I've coded linked-list and array-based variations of stacks, queues, trees, lists, graphs, hash tables, and other structures. I've also included implementations of related algorithms such as Quicksort, Breadth-first search, Dijkstra's Algorithm, tree traversal algorithms, and many others. This project was built using the principles of **Object-Oriented Programming** and does not rely on existing Java libraries.

**Timeline:** January - May 2021  
**Technologies:** Java, Eclipse, Jenkins, GitHub

## Movie Database

![ ](database.jpg)

This program manages a database of movie entries that are loaded from a file. The command line interface allows the user to sort and display movies by genre or release date. By using the C language, a **low-level procedural programming** approach allowed me to explore concepts such as memory leaks, function pointers, and **dynamic memory allocation**. As a behind-the-scenes look at object orientation, this project exposes how techniques like inheritance and overriding work in C++.

**Timeline:** January - May 2021  
**Technologies:** C language, Valgrind, GNU Debugger (GDB), GitHub

## Management System Application

![ ](management.jpg)

Based on the Model-View-Controller design pattern, I developed a **management application** for handling the customers, inventory, and orders of a fictional business. This project gave me experience with the **software development lifecycle**, debugging techniques, continuous integration practices, and unit/system testing. From UML class diagrams to user stories, this project took a comprehensive look at software development processes and practices.

**Timeline:** August - December 2020  
**Technologies:** Java, Eclipse, UMLet, GitHub

Due to academic integrity policies, I'm not able to provide source code for some or all of my projects.
