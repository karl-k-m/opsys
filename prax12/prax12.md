# Praktikum 12
Siin kirjutasin sh skripte ja lõpus lasin AIl ühe teha.

## Skript 1
<img width="960" alt="esimene" src="https://github.com/karl-k-m/opsys/assets/74490726/d1020867-7e71-438f-ad4e-f751b2b2ead2">

```
#!/bin/sh
echo "Mis on su nimi?"
read nimi
echo "Mis on su eriala?"
read eriala
echo "Mis on su martiklnumber?"
read mn
echo "$nimi, $eriala, $mn"
```

## Skript 2

```
#!/bin/sh

for i in *
    do
        if [ ${i##*.} = $1 ]
        then
            mv $i $(echo $i | sed -e s/.$1/.$2/g)
        fi
    done
```

## Skript 3

```
#!/bin/sh
pid=$(pgrep $1)
echo $pid
```

## AI Skript
```
#!/bin/bash

# Function to calculate the exponent
calculate_exponent() {
    base=$1
    exponent=$2
    result=1

    for ((i=1; i<=exponent; i++)); do
        result=$((result * base))
    done

    echo $result
}

# Input validation
if [ $# -ne 2 ]; then
    echo "Usage: $0 <base> <exponent>"
    exit 1
fi

# Parse input arguments
base=$1
exponent=$2

# Call the function to calculate the exponent
result=$(calculate_exponent $base $exponent)

echo "$base raised to the power of $exponent is equal to $result"
```
