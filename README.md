# Struct validator for golang

Another dumb library on the topic

```go

import (
		"github.com/Ajnasz/config-validator"

		"log"
)
type Config struct {
	Foo string `required:"true"`
	Bar int `required:"true"`
}


func main() {
	config := Config{}
	err := configValidator.Validate()

	if err != nil {
		log.Fatal(err)
	}
}

```
