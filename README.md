Very fast multi-threaded line count program that matches the performance of wc command

Please note that wc program caches the count after first run. So if you want to compare, always compare with first attempt of wc as subsequent runs are cached results


how to compile

gcc -O3 -lpthread -o main main.c 

for Ubuntu use

gcc -O3 -pthread -o main main.c

time ./main FILENAME

You can compare it with compare with wc like

time wc -l FILENAME


