# occlum-trace

### How to install? 
cargo install --path .

### This tool is aimed to  
1. simplify occlum's trace log(OCCLUM_LOG_LEVEL=trace) to output strace-style logs. TODO: IO-related syscalls need more information(filename, etc.)
2. check common bugs found in log.
    - file can't be found
    - thread not exits normally
3. statistic on unimplemented syscalls
4. filter logs by syscall name

Usage example: occlum-trace -i trace-file-name -o output-file-name -f futex,exit

