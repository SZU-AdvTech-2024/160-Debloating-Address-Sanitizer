## Linux Flaw Project
For Linux flaw project, we prepared detailed reproduce instructions under each CVE folder. 

Take [CVE-2006-0539](https://github.com/junxzm1990/ASAN--/tree/master/testcases/linux_flaw_project/CVE-2006-0539) as an example, you can follow the instructions in README.md to reproduce the crash. Please note that some "Experiment Environment" of CVEs are different, but you still can reproduce them on Ubuntu 18.04.

Dependencies needed to support the testcases:
```
sudo apt-get install sendmail
sudo apt-get install vim
sudo apt-get install pkg-config
sudo apt-get install fontconfig
sudo apt-get install libfontconfig1-dev
export CC=$(readlink -f ../../llvm-4.0.0-project/ASan--Build/bin/clang) CXX=$(readlink -f ../../llvm-4.0.0-project/ASan--Build/bin/clang++)
```


