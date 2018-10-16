# Go-Decent-Copy

go-decent-copy provides a copy file for humans

## Usage

```go
package main

import "github.com/hugocarreira/go-decent-copy"

func main() {
    execPath, _ := os.Getwd()

    fileOrigin := "/testCopy.txt"
    fileDestiny := fmt.Sprintf(execPath + "/folder/" + fileOrigin)
    err := Copy(fileOrigin, fileDestiny)
    if err != nil {
        fmt.Printf("Error in copy file : %#v ", err.Error())
    }
}
```