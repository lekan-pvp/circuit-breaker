# Circuit Breaker

The **Circuit Breaker** pattern automatically disables service functions in response to a probable failure to prevent larger or cascading failures, eliminate repetitive errors, and perform reasonable error checking.

## Applicability

Errors and failures are an indisputable fact in the life of distributed cloud systems. Services may be misconfigured, databases may go down, networks may stop working. We cannot prevent it; we can only accept and consider it.

Ignoring the possibility of errors and failures can have rather unpleasant consequences. 

The Circuit Breaker pattern allows you to detect failures and "break the circuit" by temporarily stopping requests and returning an error message to clients, as per the service contract.

## Components

This template includes the following components:

**Circuit**

A function that interacts with the service.

**Breaker**

A closure function with the same signature as the Circuit function.

