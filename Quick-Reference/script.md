
==SCRIPTING NOTES==

# print 1-5
for i in {1..5}; do
	echo Index=[$i]
done 

# countdown
counter=5
while [[ $counter -gt 0 ]]; do
	echo Countdown [$counter]
	counter=$(($counter - 1))
done
