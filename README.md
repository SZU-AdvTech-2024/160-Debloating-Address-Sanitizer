## 代码使用说明
### 构建ASan--
执行以下命令
``` bash
$ cd ASan--
$ mkdir ASan--Build && cd ASan--Build
$ cmake -DLLVM_ENABLE_PROJECTS="clang;compiler-rt" -G "Unix Makefiles" ../llvm
$ make -j
```
### 使用ASan--
执行以下命令
``` bash
$ ASan--/ASan--Build/bin/clang -fsanitize=address buggy.c -o buggy
$ ./buggy
```
### 复现SPEC CPU2006
商用数据集需要自行[购买](https://www.spec.org/cpu2006/)

按spec文件夹中README的步骤进行
### 复现Linux Flaw Project(CVEs)
按linux_flaw_project文件夹中README的步骤进行
### 复现Juliet Test Suite(CWEs)
公开数据集可自行[下载](https://samate.nist.gov/SARD/testsuite.php)

按juliet_test_suite文件夹中README的步骤进行