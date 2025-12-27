```go
package GoodEmployees

import (
  p "people"
)

type Programming interface {
  Go()
  Python()
  SQL()
  TS()
}

type Language interface {
  Russian()
  English()
}

type CyberSecurity interface {
  Web()
  BlueTeam()
  RedTeam()
  Network()
  LLM()
}

type Skills interface {
  Programming
  Language
  CyberSecurity

  Coffee()
  Study()
} 

func main() {
  var cipherKeeper Skills = p.NewEmployee()
}
```
