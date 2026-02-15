# CSM218 Lab 1 - Distributed Matrix Multiplication

**Name**: George Mutakura
**Student Number**: N02211720B
**GitHub Username**: GTM-04
**Repository URL**: https://github.com/CSM218/ipc-rpc-parallel-computing-GTM-04

## Scores
- Local Score: 100%
- Remote Score: 86.67% (68/98)

## Implementation Highlights
- Custom binary wire protocol with length-prefixed framing (CSM218 protocol)
- Thread-safe Master-Worker architecture with ConcurrentHashMap
- Heartbeat-based failure detection (10s timeout, 3s check interval)
- Robust task reassignment on worker failure with immediate cleanup
- PENDING/FAILED task retry mechanism for complete fault tolerance
- Concurrent task execution with thread pools (4 threads per worker)
- Atomic operations and synchronized access for thread safety
- Environment variable configuration support (STUDENT_ID, MASTER_PORT, WORKER_ID)
- RPC abstraction layer for distributed communication