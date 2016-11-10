CXX = g++
#CXXFLAGS = -g -L/opt/gtest/lib -lgtest -lgtest_main -lpthread
include /repo/ezzoccn/ezzoccn_grat_wp/workspace_design/common-grat/GTOOLS/unit_test_env/default_variables.mk
INCS = -I./ -I../../include -I/opt/gtest/include -I/repo/ezzoccn/ezzoccn_grat_wp/workspace_design/common-grat/GTOOLS/gtest-1.7.0/include
OBJS = func.o funcTest.o

testAll: $(OBJS)
	$(CXX) $(CXXFLAGS) $(INCS) -o testAll  main.cpp $(OBJS) $(INCS)

.cpp.o:
	$(CXX) $(CXXFLAGS) -c $< -o $@ $(INCS)

clean:
	rm testAll *.o
