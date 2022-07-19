# CGO Free GORM Sqlite Driver
go-gorm/sqlite uses github.com/mattn/go-sqlite3 but this uses https://gitlab.com/cznic/sqlite witch is CGO free version of sqlite.
## USAGE

```go
import (
  "github.com/hirosato/sqlite"
  "gorm.io/gorm"
)

// https://gitlab.com/cznic/sqlite
db, err := gorm.Open(sqlite.Open("gorm.db"), &gorm.Config{})
```

Checkout [https://gorm.io](https://gorm.io) for details.

## THE TRADEOFF
While CGO free version make things simple, it has performance drawback.<br/>
go-sqlite3 performs 1.5~2 times better than . For more details, refer to [this benchmarking issue](https://gitlab.com/cznic/sqlite/-/issues/27)
