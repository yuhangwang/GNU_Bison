# GNU_Bison
**GNU Bison general-purpose parser generator**

This is an unofficial verbatim redistribution of the binary&source form of the GNU Bison under its open source license (GPL 3.0) terms (see the LICENSE file).

This redistribution is under the same license as the original.

Please visit the official website for more details: http://www.gnu.org/software/bison

## Download
You can download the compiled binary files at the [release page](https://github.com/yuhangwang/GNU_Bison/releases).

## Compilation notes
### Compilation environment
* CentOS 6.6
* x86_64 architecture
* Compiler: gcc version 4.4.7 20120313 (Red Hat 4.4.7-11)

### Compilation steps
#### Version: 1.4.17 (2013)
```bash
wget http://ftp.gnu.org/gnu/bison/bison-3.0.4.tar.gz
tar xvf bison-3.0.4.tar.gz
mkdir build_bison-3.0.4
cd build_bison-3.0.4
../bison-3.0.4/configure --prefix=/home/steven/install/bison/3.0.4 --enable-threads=posix
make -j16
make check -j16 | tee QualityVerification.txt
make install
```

### Quality verification
See the "QualityVerification.txt" for the output of "make check".
