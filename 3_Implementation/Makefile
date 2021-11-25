# the compiler: gcc for C program, define as g++ for C++
CC = gcc
 
CFLAGS  = -g -Wall
 
# The build target 

BASEDIR = /home/runner/work/M1_Application_ParkingManagementSystem/M1_Application_ParkingManagementSystem/3_Implementation
SRC_DIR = $(BASEDIR)/src
TEST_DIR = $(BASEDIR)/test
OBJ_DIR = $(BASEDIR)

TARGET = parking
TEST_TARGET = parkingLotTest
 
all:
		$(CC) $(CFLAGS) -o $(OBJ_DIR)/$(TARGET) $(SRC_DIR)/$(TARGET).c

clean:
		$(RM) $(BASEDIR)/$(TARGET) $(BASEDIR)/$(TEST_TARGET)

run: all
		./$(OBJ_DIR)/$(TARGET)

build_test:
		$(CC) $(CFLAGS) -o $(OBJ_DIR)/$(TEST_TARGET) $(TEST_DIR)/$(TEST_TARGET).c

test: all
		./$(OBJ_DIR)/$(TEST_TARGET)
