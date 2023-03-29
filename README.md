# GoLang-Fun-Call
Go Function call from another file

### 1. In greeting folder
1. Create `go.mod` file in greetings folder
    - `go mod init ughosh/greetings` 
    - [Note] you can put any name here. Go suggest to make it like a folder structure
2. Create greetings.go file
    - copy the file. It's just a sample file for reference


### 2. In Hello folder
1. Create `go.mod` file in greetings folder
    - `go mod init ughosh/hello`
1. Create hello.go file


### 3. Importing function in other folder
   1. Notice that we've used - `"ughosh/greetings"` as an `import` to import `greetings.go`

   2. Run in Hello folder
      - `go mod edit -replace="ughosh/greetings"=../greetings`
       - `go mod tidy`
       - `go run .`   // this will run your program succesfully!!