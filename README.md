# Numa
Clang based numerical analysis

Description: change REAL or other types in iRRAM to specific types,and the environment is Ubuntu-14.04 and the llvm-clang-3.6.0
Basic Tutorial in here;
1. we should download Ubuntu-14.04,and then download llvm-clang-3.6.0 and build it;
2. http://releases.llvm.org/download.html you can find the Clang-3.6.0 and download it, of course, you can just download the pre-built clang;
3. Unzip it to where you want to install llvm+clang; some detials you can refer http://blog.csdn.net/firebird321/article/details/48528569
, note we don't need to install libcxx,etc;
4. then you can just use command "clang -v" to make sure you install it correctly;
5. we still need to download iRRAM,before it we need to install gmp and mrfp;
6. use "sudo apt-get install libgmp-dev" and "sudo apt-get install libmpfr-dev" to install them
7. http://irram.uni-trier.de/index.php/download/ the address to download, I downloaded 2013_01 version;
8. https://github.com/norbert-mueller/iRRAM/blob/master/INSTALL the tutorial about how to install it;
9. the matcher.cpp in src is the file we use to achieve my goal;
10. change the makefile, just modify the llvm's path is ok
11. change the run.sh shell script, modify the path to iRRAM is ok;
12. we need to create a filefolder output in Numa;
12. then we just use command "./run.sh ./test/**.cpp" **.cpp means somefile in test.
13.check the result
