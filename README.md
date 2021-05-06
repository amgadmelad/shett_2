# shett_2
bash shell (sheet_2)

Q1:Convert seconds to hours , minutes and seconds

#! /bin/bash

sec=0

hr=0

min=0

sec1=0

echo "Enter The Seconds:"

read sec
hr=$(( sec / 3600 ))
sec=$(( sec % 3600 ))
min=$(( sec / 60 ))
sec1=$(( sec % 60 ))
echo "Equivalient time= $hr : $min : $sec1"
-----------------------------------------------------------------------------
Q2:Calaculate the Power:
#! /bin/bash
echo "Enter The base number:"
read number
echo "Enter The Power number:"
read Power
if (( number >0 ))
then
exp=$(( number ** Power ))
echo "Resulet=$exp"
else
echo "Please Enter a positive number:"
fi
--------------------------------------------------------------------------
Q3:Check the Prime number
#! /bin/bash
echo "Enter The Number:"
read number
for((i==2; i<number/2; i++))
do
  ans=$(( number%i ))
  if (( ans==0 ))
  then
    echo "$number is not a prime number:"
    exit 0
  fi
done
echo "$number is a prime number:"

------------------------------------------------------------------------------------------------------
Q4:To convert from celsius degree to farenhit degree:
#! /bin/bash
celsius=0
read -p  "Enter the degree celsius temperature:" celsius #To Print the message and the input in one line
fahrenheit= echo "scale=4;$celsius*1.8 + 32" | bc
echo $fahrenheit 
-------------------
