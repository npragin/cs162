CXX = g++
CXXFLAGS = -g
EXE = hooping_catalog

.INTERMEDIATE = catalog.o run_catalog.o

$(EXE): run_catalog.o catalog.o
	$(CXX) $(CXXFLAGS) run_catalog.o catalog.o -o $(EXE)

run_catalog.o: run_catalog.cpp
	$(CXX) $(CXXFLAGS) run_catalog.cpp -c

catalog.o: catalog.cpp catalog.h
	$(CXX) $(CXXFLAGS) catalog.cpp -c

clean:
	rm -rf *.o $(EXE)