myProgram: address.o employee.o main.o
	g++ main.o address.o employee.o -o myProgram

main.o: main.cpp address.h employee.h
	g++ -c main.cpp address.h employee.h

address.o: address.cpp
	g++ -c address.cpp 

emplyee.o: emplyee.cpp address.h
	g++ -c emplyee.cpp address.h
clean:
	rm -f *~ *.bak
	rm -f myProgram address.o employee.o main.o
