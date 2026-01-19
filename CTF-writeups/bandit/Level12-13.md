# Bandit Level 12 → Level 13

## Objective
Decompress a repeatedly compressed and renamed file (`data.txt`) to retrieve the password.

## Commands Used
cd /tmp/bandit12_work
cp ~/data.txt
xxd -r data.txt > datafile
file datafile
mv datafile datafile.gz
gzip -d datafile.gz
file datafile
mv datafile datafile.bz2
bzip2 -d datafile.bz2
file datafile
mv datafile datafile.gz
gzip -d datafile.gz
file datafile
tar -xf datafile
file data5.bin
tar -xf data5.bin
file data6.bin
mv data6.bin data6.bin.bz2
bzip2 -d data6.bin.bz2
file data6.bin
cat data6.bin

## Password
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
