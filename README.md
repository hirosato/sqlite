# CGO Free GORM Sqlite Driver

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
