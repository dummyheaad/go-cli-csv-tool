# CSV Tool CLI App

A simple CLI App that can be used to perform several calculations like avg, sum, min, and max on a single column of csv file.

## How to Install
### Clone the repository

    git clone https://github.com/dummyheaad/go-cli-csv-tool.git

### Build the executable

    go build .

## Functionalities
### Calculate the average values of a column

    ./colStats -col 2 -op avg testdata/example.csv
    Output:
    1.5206989902e+09

### Calculate the sum of all values of a column

    ./colStats -col 2 -op sum testdata/example.csv
    Output:
    7.603494951e+09

### Find the maximum value of a column

    ./colStats -col 2 -op max testdata/example.csv
    Output:
    1.520699379e+09

### Find the minimum value of a column

    ./colStats -col 2 -op min testdata/example.csv
    Output:
    1.520698621e+09

### Calculate the average values of a column from multiple csv file

    ./colStats -col 2 -op avg testdata/example.csv testdata/example2.csv
    Output:
    1.52069922348e+09

## Show Tracing Results

    go tool trace trace01.out
