all: build-load-balancer

load-balancer-files = LoadBalancer.cpp LoadBalancer.hpp ../lib/httplib.h ../lib/json.hpp ../lib/umbridge.h

build-load-balancer:
	- g++ -O3 -Wno-unused-result -std=c++17 $(load-balancer-files) -o load-balancer -pthread

build-test-server:
	- g++ -O3 -Wno-unused-result -std=c++17 test/MultiplyBy2/minimal-server.cpp -o test/MultiplyBy2/minimal-server -pthread
