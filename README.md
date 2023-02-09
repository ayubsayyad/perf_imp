# perf_imp

while findding bottelnecks in performance few tools are handy and dont need too many changes in code.

on linux perf comes handy as it shows what is consuming most cpu.
sudo perf record -g --call-graph=dwarf -F 99 -p <pid>
sudo perf report --call-graph --stdio -G

for looking at each system call and time consumed by it 
strace -T -p  <pid>

ltrace is also useful for few cases

