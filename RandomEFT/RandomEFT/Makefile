# Simple makefile
testRamdom: testRandom.cxx
	g++ -c -fPIC Root/*.cxx -I. `root-config --cflags`
	g++ -c -fPIC cMorphWrapper.cxx -I. `root-config --cflags`
	g++ -shared -Wl,-soname,libcMorphWrapper.so -o libcMorphWrapper.so *.o -L/usr/lib64/root -lGui -lCore -lRIO -lNet -lHist -lGraf -lGraf3d -lGpad -lTree -lRint -lPostscript -lMatrix -lPhysics -lMathCore -lThread -pthread -lm -ldl -rdynamic
