# go-map

A library for working with Magic Attribute Protocol. Used in conjunction with a Tape from [go-bob](https://github.com/rohenaz/go-bob)

## Usage

```go
    import "github.com/rohenaz/go-bob"
    mapp import "github.com/rohenaz/go-map"

    line := "<BOB formatted json string>"

    bobData := bob.New()
    if err := json.Unmarshal(line, &bobData); err != nil {
      fmt.Println("Error:", err)
      return
    }

    mapData := mapp.New()
    mapData.FromTape(tape)

    log.Printf("MAP TYPE is %s", MAP.type)
```
