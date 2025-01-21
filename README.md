# TCP-Connection-Monitoring

TCP Connection Monitoring to identify performance bottleneck

As a part of Computer Networks, we did a project under the guidance of Dr. Kotaro Kataonka to develop an efficient
TCP connection monitoring tool which can help to identify and fix performance problems. We took inspiration
from the research paper on SNAP(Scalable Network-Application Profiler) by Minlan Yu et al, and developed a similar
tool of our own. It consisted of the following components:

1. Our network topology was a full duplex TCP client-server model

2. At the client socket, we deployed the monitoring tool which would monitor statistics such as timeouts, fast-
retransmissions, bytes sent, congestion window etc and store these stats.

3. We monitored these stats at poisson intervals, to make the monitoring as CPU-efficient as possible

4. The final results were - CPU utilization increased by 6.2 percent due to monitoring, and memory utilization by
1.8 percent, demonstrating that our tool is light-weight, was not very heavy on compute resources.


   
