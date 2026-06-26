CC = gcc
CFLAGS = -Wall -Wextra -O2 -Iinclude
TEST_FLAGS = -Wall -Wextra -g -Iinclude

APP = system_monitor
TEST_APP = test_system_monitor

SRC = src/system_monitor.c
MAIN = src/main.c
TEST_SRC = tests/test_system_monitor.c

all:
	$(CC) $(CFLAGS) $(SRC) $(MAIN) -o $(APP)

test:
	$(CC) $(TEST_FLAGS) $(SRC) $(TEST_SRC) -o $(TEST_APP) -lm
	./$(TEST_APP)

clean:
	rm -f $(APP) $(TEST_APP)