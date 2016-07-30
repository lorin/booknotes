# The Practice of Cloud System Administration: Designing and Operating Large Distributed Systems, Volume 2
by Tom Limoncelli

# Chapters

## 6. Design patterns for resiliency

### Sections
- Software resiliency beats hardware reliability
- Everything malfunctions eventually
- Resiliency through spare capacity
- Failure domains
- Software failures
- Physical failurse
- Overload failures
- Human error
- Summary

### Terms
- Outage: A user-visible lack of service.
- Failure: A system, subsystem, or component that has stopped working.
- Malfunction: Used interchangeably with “failure.”
- Server: Software that provides a function or API. (Not a piece of hardware.)
- Service: A user-visible system or product composed of one or more servers.
- Machine: A virtual or physical machine.
- QPS: Queries per second. Usually how many web hits or API calls are received per second.
- Survivable system: failed component does not lead to a user-visible outage

### Notes

- Resiliency: system's ability to constructively deal with failures.
- A resilient system detects failure and routes around it
- During the first year of a typical Google datacenter, there will be five
  rack-wide outages, three router failures large enough to require diverting
  processing away from connected machines, and eight network scheduled
  maintenance windows, half of which cause 30-minute random connectivity losses.
  At the same time 1 to 5 percent of all disks will die and each machine will
  crash at least twice (2 to 4 percent failure rate) (Dean 2009).
 

