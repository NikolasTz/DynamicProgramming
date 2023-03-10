
## Optimal Reservation Policy

### Description

The problem is to find the optimal reservation policy for an airline company that maximizes the company's revenue for each flight. The optimal reservation policy should consider the following parameters:

1. The capacity **X** of the airplane
2. The policy should be planned **K hours** before the flight
3. The number of reservations per hour
4. The number of canceled reservations
5. The cost of a ticket refund

### Problem configuration

    Statutory Equation: π(π + π) = π(π) β π(π) + πππ{π(π), π(π)}

     π(π): The number of reservation in the kth hour
     π(π): The number of the reservation during the kth hour. We assume that is a discrete stochastic random variable following the uniform distribution, P[z(k)]
     π(π): The maximum number of new reservations to be accepted during the k-th hour, 0 β€ π(π) β€ πππ{π«, ππ² β π(π)} with π β β€ , π(π) β [π, π«]
     π(π): The number of requested reservations during the k-th hour. We assume that is a discrete stochastic random variable following the uniform distribution, P[d(k)], π(π) β [π, π«]

```
Objective cost criterion    

π± = π β πππ{π(π),πΏ} β π β πππ{π, π(π) β πΏ}

The cost criterion refers to the companyβs revenue during one flight, given the π(π) and πΏ. 
The first term refers to the companyβs revenue from the sale of tickets with a value of v. 
The second term refers to the total amount of refunds for each customer who does not have a seat available on the airplane. We assume that the ticket refund is ΞΌ.

```

### Program configuration
    Input parameters
        1. The capacity X of the airplane
        2. The number of hours K
        3. The upper bound D for the uniform distributions d,u
        4. The parameter Ξ» that defines the upper bound of the new reservations
        5. The value of ticket v
        6. The ticket refund ΞΌ



### Compile and Run
    gcc -Wall -o main.c
    ./main.o
