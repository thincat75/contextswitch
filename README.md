# contextswitch
g++ -O3 -o test_latency test_latency.cpp -lpthread
./test_latency 0 1

g++ -o test test.c
./test

/* tuned the performance of the servers */
tuned-adm active /* display the profile of server, default is balanced */
tuned-adm list
tuned-adm profile latency-performance /* optimaize for the latency performance */
