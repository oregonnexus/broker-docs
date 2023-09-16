# Broker Concepts
Different vocabulary can be used to describe the same concepts that the Broker uses.

## Vocabulary
* *Receiving School*. When a parent registers their student at a new school, this school will become the receiving school. It may also be called the enrolling school, the receiving school or the requesting school.
* *Sending School*. This is the student's previous school and the one that will send records to the receiving school. It may also be called the releasing school.
* *Records Clerk*. The person that processes student records. Adding *receiving* or *sending* in front of *records clerk* designates which school's records clerks is being referred.
* *Incoming Request*. The receiving records clerk generates an incoming request in their Broker, entering the information necessary to generate the  
* *Outgoing Request*. When the new school generates the incoming request, the receiving school's Broker sends that request to the sending school's Broker. That request appears for the sending school as an outgoing request.

## Diagram
```mermaid
flowchart TD
    A[Receiving School Records Clerk] -->|Incoming Request| B(Receiving School's Broker);
    B-->|Transfer| C(Sending School's Broker);
    C-->|Outgoing Request| D[Sending School Records Clerk];
```

## Business Process Rules
1. The receiving school always starts the process and initiates the request. The records are pulled to the new school - not pushed. The sending school will never start the request.
