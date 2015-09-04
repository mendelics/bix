bix
===

Tabix files in go.

[![GoDoc] (https://godoc.org/github.com/brentp/bix?status.png)](https://godoc.org/github.com/brentp/bix)


```go
tbx, err := bix.New(f)

// Query returns an io.Reader
rdr, err := tbx.Query(chrom, start, end)
buf := bufio.NewReader(rdr)
for {
	line, err := bufr.ReadString('\n')
	if err == io.EOF {
		break
	}
	fmt.Println(line)
}
```
