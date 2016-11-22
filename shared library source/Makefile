LIBRARY_NAME = libpreprocessor
VER = .1

PROG = $(LIBRARY_NAME).so
CFLAGS = -fPIC -O3 -Wl,-soname,$(PROG)$(VER)

SRCS = preprocessor.cpp gcode.cpp vector.cpp
CFLAGS += -Wall -std=c++11 -fvisibility=hidden -shared

all:
	$(CXX) $(CFLAGS) -o ../octoprint_m33fio/static/libraries/$(PROG) $(SRCS)

clean:
	rm -f ../octoprint_m33fio/static/libraries/$(PROG)
