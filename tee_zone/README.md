# Trusted Zone code

<<<<<<< HEAD
## Trace Flow API
This directory offer API for tracing control flow and calculate overflow
We use System call to protect each informations with hashing
This hash value send to peer and confirm validity

## user_API

### USAGE
1. Put API in your work space(This API use several tool supported by optee-os)
2. modify add API in sub.mk(i.e. 'srcs-y += test.c')
3. include in your code
4. USE LOGH() or LOGH2()

### hello_world
This directory is example directory.

### problems
1. current D_test function is non-static

=======
## About Syscall
  Our code is use syscall to record control flow with hashing.
  To guarantee integrity, we record it on secure OS(OPTEE-OS)

## About Chaincode
  This chaincode use 'coffee_tracking' chaincode.
  The 'Chaincode' directory contains execution in TEE.

## About static binary analysis and modifier
  Our implements is needed trampoline that intercept flow and call system call.
  So, This analyzer search branch code and modify it.
>>>>>>> 17322fc361273003f8301510db90910a70d2d35c