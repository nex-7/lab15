## Laboratory work XV

Данная лабораторная работа посвещена изучению инструментов статического и динамического анализа кода
```ShellSession
$ open http://cppcheck.sourceforge.net
```

## Tasks

- [X] 1. Ознакомиться со ссылками учебного материала
- [X] 2. Используя **cpplint** провести анализ проекта на **C++**
- [X] 3. Используя **Cppcheck** провести анализ проекта на **C++**
- [X] 4. Используя **OCLint** провести анализ проекта на **C++**
- [X] 5. Используя **Valgrind** провести анализ проекта на **C++**
- [X] 6. Составить отчет и отправить ссылку личным сообщением в **Slack**

## cpplint
```ShellSession
$ cpplint test.cpp
Done processing test.cpp
```

## cppcheck
```ShellSession
$ cppcheck test.cpp
Checking test.cpp...
```

## OCLint
```ShellSession
$ oclint test.cpp -- -c


OCLint Report

Summary: TotalFiles=1 FilesWithViolations=0 P1=0 P2=0 P3=0 


[OCLint (http://oclint.org) v0.13]
```

## Valgrind
```ShellSession
$ valgrind ./test
==23275== Memcheck, a memory error detector
==23275== Copyright (C) 2002-2017, and GNU GPL'd, by Julian Seward et al.
==23275== Using Valgrind-3.13.0 and LibVEX; rerun with -h for copyright info
==23275== Command: ./test
==23275== 
Hello world!
==23275== 
==23275== HEAP SUMMARY:
==23275==     in use at exit: 72,704 bytes in 1 blocks
==23275==   total heap usage: 2 allocs, 1 frees, 73,728 bytes allocated
==23275== 
==23275== LEAK SUMMARY:
==23275==    definitely lost: 0 bytes in 0 blocks
==23275==    indirectly lost: 0 bytes in 0 blocks
==23275==      possibly lost: 0 bytes in 0 blocks
==23275==    still reachable: 72,704 bytes in 1 blocks
==23275==         suppressed: 0 bytes in 0 blocks
==23275== Rerun with --leak-check=full to see details of leaked memory
==23275== 
==23275== For counts of detected and suppressed errors, rerun with: -v
==23275== ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0)
```

## Links

- [Google C++ Style Guide](https://github.com/cpplint/cpplint)
- [Cppcheck Manual](http://cppcheck.sourceforge.net/manual.pdf)
- [Valgrind Quick Start Guide](http://valgrind.org/docs/manual/index.html)
- [OCLint Tutorial](http://docs.oclint.org/en/stable/intro/tutorial.html)

```
Copyright (c) 2017 Братья Вершинины
```


