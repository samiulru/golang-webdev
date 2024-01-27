#
# Useful GO Commands


## Run Go file

- To run single Golang file Replace the <b style="color:rgb(140, 215, 230)">path and file_1.go by file path filename</b> of the desired file respectively
        
        go run path/'file_1.go'

- To run multiple Golang file, replace the <b style="color:rgb(140, 215, 230)">path_1 file_1.go, path_2 file_2.go</b> with file path and file names repectively

        go run path_1/file_1.go path_2/file_2.go ...

- To run all Golang files in the same directory follow command is used
For Linux and MacOS:

        go run path/*.go

- For Windows:

        go run path/*.go



#
## Testing In Go


- The following command executes test functions (whose names begin with Test) in test files (whose names end with _test.go).
                            
        go test 

-  To run all test in the current directory along with the cild directory:

        go test -v ./...

 - <b style=" color: RGB (140, 215, 230)">-v</b> flag is added to get verbose output that lists all of the tests and their results.

       go test -v

- <b style="color:rgb(140, 215, 230)">-cover</b> Shows how much of the entire code is tested

        go test -cover
- Using the flag <b style="color:rgb(140, 215, 230)">-coverprofile</b> will create a local coverage report file.You can also use go tool cover to format the report. For example, the -html flag will open your default browser to display a graphical report.
    
        go test -coverprofile=coverage.out && go tool cover -html=coverage.out

