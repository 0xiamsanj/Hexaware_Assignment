#!/bin/bash

# Function to add leading zeros
add_leading_zeros() {
  printf "%02d" $1
}

for (( n=5; n<=18; n++ ))
do
    # Add leading zeros to the number
    padded_number=$(add_leading_zeros $n)

    # Generate filename
    filename="${padded_number}_Query.mysql"

    cat > "$filename" << EOF
/**
 * Script to create table $n
 */
EOF
done
