Use more to view a file.
root@ubuntu-host ~/Pranaya ➜more Text.cpp

Scroll down in more (Enter or Space).
Press Enter

Search in more (/word).
Search word by using /someword

Exit more (q).
Just q

Use head to display the first 10 lines of a file.
root@ubuntu-host ~/Pranaya ➜  head Text.cpp 

#include<iostream>

using namespace std:

class Parent{
        public:
                Pranaya(){
                        cout<<"Parent constructor"<<endl;
                }
                void fn1(){

Use head -n 20 to display the first 20 lines.
root@ubuntu-host ~/Pranaya ➜  head -n 20 Text.cpp 
#include<iostream>

using namespace std:

class Parent{
        public:
                Pranaya(){
                        cout<<"Parent constructor"<<endl;
                }
                void fn1(){
                        cout<<"parent class function"<<endl;
                }
};
class Derived : Public Parent{
        public:
                Derived(){
                        cout<<"Derived constructor"<<endl;
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;

Use head with a command pipeline.
root@ubuntu-host ~/Pranaya ➜  head Text.cpp | grep Pranaya
                Pranaya(){

Use tail to display the last 10 lines.
root@ubuntu-host ~/Pranaya ➜  tail Text.cpp 
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;
                        }
}
int main(){
        Parent *p1 = new Derived();
        p1->fn1();
        return 0;
}

Use tail -n 20 for the last 20 lines.
root@ubuntu-host ~/Pranaya ➜  tail -n 20 Text.cpp 
                        cout<<"Parent constructor"<<endl;
                }
                void fn1(){
                        cout<<"parent class function"<<endl;
                }
};
class Derived : Public Parent{
        public:
                Derived(){
                        cout<<"Derived constructor"<<endl;
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;
                        }
}
int main(){
        Parent *p1 = new Derived();
        p1->fn1();
        return 0;
}

Use tail -f to monitor a log file in real-time.
root@ubuntu-host ~/Pranaya ➜  tail -f Text.cpp 
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;
                        }
}
int main(){
        Parent *p1 = new Derived();
        p1->fn1();
        return 0;
}

Combine tail with grep to filter recent logs.
root@ubuntu-host ~/Pranaya ➜  tail Text.cpp | grep Derive
        Parent *p1 = new Derived();

Use head to preview the start of a file before editing.
root@ubuntu-host ~/Pranaya ➜  head Derived.cpp 

root@ubuntu-host ~/Pranaya ➜  

Blank output
Use more to paginate through a file.
#include<iostream>

using namespace std:

class Parent{
        public:
                Pranaya(){
                        cout<<"Parent constructor"<<endl;
                }
                void fn1(){
                        cout<<"parent class function"<<endl;
                }
};
class Derived : Public Parent{
        public:
                Derived(){
                        cout<<"Derived constructor"<<endl;
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;
                        }
}
int main(){
        Parent *p1 = new Derived();
        p1->fn1();
        return 0;

Use head with a command pipeline to get the first few lines of command output.
root@ubuntu-host ~/Pranaya ➜  ls -l | head
total 4
-rw-r--r-- 1 root root   0 Aug 13 11:53 Derived.cpp
-rw-r--r-- 1 root root 402 Aug 13 11:31 Text.cpp

Use tail with a command pipeline to get the last few lines.
root@ubuntu-host / ➜  ls -l|head
total 80
lrwxrwxrwx   1 root   root       7 Apr 22  2024 bin -> usr/bin
drwxr-xr-x   1 root   root    4096 Mar 31  2024 bin.usr-is-merged
drwxr-xr-x   1 root   root    4096 Apr 22  2024 boot
drwxr-xr-x   5 root   root     420 Aug 13 09:58 dev
drwxr-xr-x   1 root   root    4096 Aug 13 09:58 etc
drwxr-xr-x   1 root   root    4096 Oct 16  2024 home
lrwxrwxrwx   1 root   root       7 Apr 22  2024 lib -> usr/lib
drwxr-xr-x   1 root   root    4096 Jul  1  2024 lib.usr-is-merged
lrwxrwxrwx   1 root   root       9 Apr 22  2024 lib64 -> usr/lib64

Use tail -n +10 to skip the first 9 lines.
root@ubuntu-host ~/Pranaya ➜  tail -n+10 Text.cpp 
                void fn1(){
                        cout<<"parent class function"<<endl;
                }
};
class Derived : Public Parent{
        public:
                Derived(){
                        cout<<"Derived constructor"<<endl;
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;
                        }
}
int main(){
        Parent *p1 = new Derived();
        p1->fn1();
        return 0;
}


Use head -c 50 to get the first 50 bytes.
root@ubuntu-host ~/Pranaya ➜  head -c 50 Text.cpp 
#include<iostream>

using namespace std:

class Pa

Use tail -c 50 to get the last 50 bytes.
root@ubuntu-host ~/Pranaya ➜  tail -c 50 Text.cpp 
ent *p1 = new Derived();
        p1->fn1();
        return 0;
}

Use more with a compressed file (zcat piped into more).
root@ubuntu-host ~/Pranaya ➜  zcat compress.gz | more
gdh
FHSMn
yfjsmn
jeyfbn

Use head to get the first 5 lines of a command output.
root@ubuntu-host / ➜  ls -l | head -n 5
total 80
lrwxrwxrwx   1 root   root       7 Apr 22  2024 bin -> usr/bin
drwxr-xr-x   1 root   root    4096 Mar 31  2024 bin.usr-is-merged
drwxr-xr-x   1 root   root    4096 Apr 22  2024 boot
drwxr-xr-x   5 root   root     420 Aug 13 09:58 dev

Use tail to get the last 5 lines of a command output.
root@ubuntu-host / ✖ ls -l | tail -n 5
drwxr-xr-x   1 root   root    4096 Oct 16  2024 srv
dr-xr-xr-x  13 nobody nogroup    0 Jun  1 21:57 sys
drwxrwxrwt   6 root   root    4096 Aug 13 12:02 tmp
drwxr-xr-x   1 root   root    4096 Oct 16  2024 usr
drwxr-xr-x   1 root   root    4096 Aug 13 09:58 var

Use less to view a file and search for multiple words.
root@ubuntu-host / ➜  less Text.cpp

Use more to view a large file with line numbers (nl).

Use head to preview a file before copying.
root@ubuntu-host ~/Pranaya ➜  head Text.cpp 
#include<iostream>

using namespace std:

class Parent{
        public:
                Pranaya(){
                        cout<<"Parent constructor"<<endl;
                }
                void fn1(){

Use less to view a file and save a copy (:w filename).
root@ubuntu-host / ➜  less Text.cpp

Use head to get the first 100 bytes of a file.
root@ubuntu-host ~/Pranaya ✖ head -c 100 Text.cpp 
#include<iostream>

using namespace std:

class Parent{
        public:
                Pranaya(){
                        cout<<"Parent const

Use tail to get the last 100 bytes.
root@ubuntu-host ~/Pranaya ✖ tail -c 100 Text.cpp 
erived constructor"<<endl;
                        }
}
int main(){
        Parent *p1 = new Derived();
        p1->fn1();
        return 0;
}

Use more to view a file with a custom prompt.
more -P "=== Viewing File: %f (%p%% complete) ===" Text.cpp
Use head to get the first 10 lines of multiple files.
root@ubuntu-host ~/Pranaya ✖ head -n 10 Text.cpp Derived.cpp 
==> Text.cpp <==
#include<iostream>

using namespace std:

class Parent{
        public:
                Pranaya(){
                        cout<<"Parent constructor"<<endl;
                }
                void fn1(){

==> Derived.cpp <==

Use tail to get the last 10 lines of multiple files.
root@ubuntu-host ~/Pranaya ✖ tail -n 10 Text.cpp Derived.cpp 
==> Text.cpp <==
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;
                        }
}
int main(){
        Parent *p1 = new Derived();
        p1->fn1();
        return 0;
}

==> Derived.cpp <==

Use head with sort to preview sorted data.
root@ubuntu-host ~/Pranaya ✖ sort Text.cpp |head -n 10


                                cout<<"derived constructor"<<endl;
                        cout<<"Derived constructor"<<endl;
                        cout<<"Parent constructor"<<endl;
                        cout<<"parent class function"<<endl;
                        void fn1(){
                        }
                Derived(){
                Pranaya(){

Use tail with grep to find recent errors.
root@ubuntu-host ~/Pranaya ➜  tail -n 50 Text.cpp | grep "ERROR"
ERROR

Use less to view a file with line numbers (-N).
root@ubuntu-host / ➜  less -N Text.cpp

Use more with line numbers (-N).
       
     2  using namespace std:
     3  ERROR
     4  class Parent{
     5          public:
     6                  Pranaya(){
     7                          cout<<"Parent constructor"<<endl;
     8                  }
     9                  void fn1(){
    10                          cout<<"parent class function"<<endl;
    11                  }
    12  };
    13  class Derived : Public Parent{
    14          public:
    15                  Derived(){
    16                          cout<<"Derived constructor"<<endl;
    17                  }
    18                          void fn1(){
    19                                  cout<<"derived constructor"<<endl;
    20                          }
    21  }
    22  int main(){
    23          Parent *p1

Use head to get the first 10 lines of a command output.
root@ubuntu-host / ➜  ls -l | head -n 10
total 84
drwxr-xr-x    2 root   root    4096 Aug 13 12:46 Pranaya
lrwxrwxrwx    1 root   root       7 Apr 22  2024 bin -> usr/bin
drwxr-xr-x    1 root   root    4096 Mar 31  2024 bin.usr-is-merged
drwxr-xr-x    1 root   root    4096 Apr 22  2024 boot
drwxr-xr-x    5 root   root     420 Aug 13 12:24 dev
drwxr-xr-x    1 root   root    4096 Aug 13 12:24 etc
drwxr-xr-x    1 root   root    4096 Oct 16  2024 home
lrwxrwxrwx    1 root   root       7 Apr 22  2024 lib -> usr/lib
drwxr-xr-x    1 root   root    4096 Jul  1  2024 lib.usr-is-merged

Use tail to get the last 10 lines of a command output.
root@ubuntu-host / ✖ ls -l | tail -n 10
dr-xr-xr-x 1423 root   root       0 Aug 13 12:24 proc
drwx------    1 root   root    4096 Aug 13 12:46 root
drwxr-xr-x   14 root   root     420 Aug 13 12:44 run
lrwxrwxrwx    1 root   root       8 Apr 22  2024 sbin -> usr/sbin
drwxr-xr-x    1 root   root    4096 Mar 31  2024 sbin.usr-is-merged
drwxr-xr-x    1 root   root    4096 Oct 16  2024 srv
dr-xr-xr-x   13 nobody nogroup    0 Jun  8 01:47 sys
drwxrwxrwt    6 root   root    4096 Aug 13 12:44 tmp
drwxr-xr-x    1 root   root    4096 Oct 16  2024 usr
drwxr-xr-x    1 root   root    4096 Aug 13 12:24 var

Use more to view a file and jump to the end (G).

Use head to preview a file before processing.
root@ubuntu-host /Pranaya ➜  head -n 20 Text.cpp 
#include<iostream>

using namespace std:
ERROR
class Parent{
        public:
                Pranaya(){
                        cout<<"Parent constructor"<<endl;
                }
                void fn1(){
                        cout<<"parent class function"<<endl;
                }
};
class Derived : Public Parent{
        public:
                Derived(){
                        cout<<"Derived constructor"<<endl;
                }
                        void fn1(){
                                cout<<"derived constructor"<<endl;

Use tail to follow a log file (-f).
root@ubuntu-host /Pranaya ➜  tail -f /var/log/journal/05ee70c460a9dd015c31410c674044a5/system.journal

Use head to get the first 10 lines of a command output and save to a file.
root@ubuntu-host /Pranaya ➜  ls -l | head -n 10 > Text.cpp

Use tail to get the last 10 lines and save to a file.
root@ubuntu-host /Pranaya -> ps aux | tail -n 10 > bottom10.txt

root@ubuntu-host /Pranaya ➜  ls
Derived.cpp  Teaxt.cpp  Text.cpp  bottom10.txt

root@ubuntu-host /Pranaya ➜  vi bottom10.txt 

Use head and tail together to extract specific sections of a file.
root@ubuntu-host /Pranaya ➜  head -n 30 Text.cpp | tail -n 10
total 8
-rw-r--r-- 1 root root  66 Aug 13 12:46 Derived.cpp
-rw-r--r-- 1 root root 159 Aug 13 12:56 Teaxt.cpp
-rw-r--r-- 1 root root   0 Aug 13 12:57 Text.cpp

Use less to view a large text file.
root@ubuntu-host /Pranaya ➜less Text.cpp
Scroll down in less using the spacebar.
Spacebar to move forward by one page
Exit less (q).
q



View your command history (history command).
root@ubuntu-host ~/Pranaya ➜  history
    1  history
    2  clear
    3  history
    4  mkdir Pranaya
    5  cd Pranaya/
    6  vi Text.cpp
    7  history

Re-execute the last command (!!).
Re-execute a specific command from history (!n, where n is the command number).
root@ubuntu-host ~/Pranaya ➜  !4
mkdir Pranaya

Clear the command history (history -c).
root@ubuntu-host ~/Pranaya ✖ history -c  

root@ubuntu-host ~/Pranaya ➜  history
    1  history





