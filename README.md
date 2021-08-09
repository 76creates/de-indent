# de-indent

Go tool for deindenting the strings, good to use when writing multiline strings and still wanting to preserve good looking formatting like:
~~~go
package main

import deindent "github.com/76creates/de-indent"

func main() {
	description := deindent.DeIndent(`
        Hello this is my description
        it stays classy :)
    `)
	print(description)
}
~~~

~~~bash
go run .
Hello this is my description
it stays classy :)
~~~