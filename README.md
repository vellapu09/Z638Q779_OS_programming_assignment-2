# Z638Q779_OS_programming_assignment-2
This project implements a basic simulation of a lottery scheduling algorithm, a probabilistic scheduling algorithm for processes in an operating system. Each process is assigned a set of lottery tickets, and the scheduler selects a winning ticket at random to decide which process gets to run next. This simulation explores the concept by allowing for different ticket allocation strategies and simulating process execution.

Features
Process Simulation: Each process is represented with a unique ID and a set of lottery tickets.
Lottery Scheduler: A scheduler that manages processes, allocates lottery tickets based on a specified strategy, and selects the next process to run.
Random and Sequential Ticket Allocation: Supports different strategies for ticket allocation to processes.
Process Execution Simulation: Simulates the execution of a process by reducing its number of tickets, mimicking progress towards completion.
State Display: Ability to display the current state of the scheduler and processes, including the distribution of tickets.
Setup
To run this simulation, you need a Python interpreter (version 3.6 or newer recommended). No external libraries are required as it only uses the standard library.

Clone or download this repository to your local machine.
Navigate to the project directory in your terminal or command prompt.
Running the Simulation
Execute the script from the command line:

bash
python lottery_scheduling.py
Upon running, the script will:

Initialize a scheduler with a predefined number of processes.
Allocate lottery tickets to each process based on the chosen allocation strategy.
Simulate the selection and partial "execution" of processes by randomly selecting a winning ticket and then simulating execution for a few iterations.
Display the state of the scheduler and processes before and after each selection and simulated execution.
Configuration
The main parameters of the simulation, such as the number of processes and the ticket allocation strategy, can be adjusted directly in the main function of the script:

Change the allocation_strategy in the Scheduler initialization to "random" or "sequential" based on preference.
Modify the loop in the main function to create a different number of processes.
Exploring the Code
Process Class: Represents a process in the system with a unique ID and a list of lottery tickets.
Scheduler Class: Manages processes and implements the lottery scheduling algorithm, including ticket allocation and process selection.
