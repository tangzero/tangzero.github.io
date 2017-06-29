---
title: "Hello World"
date: 2017-06-27T17:10:01-04:00
draft: true
---

# Hello World

{{<highlight go>}}
package main

import "fmt"

func main() {
    ch := make(chan float64)
    ch <- 1.0e10    // magic number
    x, ok := <- ch
    defer fmt.Println(`exitting now\`)
    go println(len("hello world!"))
    return
}
{{</highlight>}}
