# Go Getting Started — Study Notes (Topic 1.1)

> Interactive lab: open `go-getting-started-lab.canvas.tsx` in Cursor anytime.

---

## The big picture (4 ideas)


| #   | Topic         | Simple meaning         | Command                              |
| --- | ------------- | ---------------------- | ------------------------------------ |
| 1   | Install Go    | Toolbox on your PC     | `go version`                         |
| 2   | Modules       | Project name tag       | `go mod init` → `go.mod`             |
| 3   | First program | Front door of your app | `package main` + `func main()`       |
| 4   | Tooling       | Daily chores           | `fmt`, `vet`, `test`, `run`, `build` |


---

## Your project folder

```
go-workshop/
├── go.mod          ← name tag
├── go.sum          ← security stamps (appears later)
├── main.go         ← your code
├── main_test.go    ← tests
└── greet.exe       ← built app (after go build)
```

---



## Lesson 1 — Install Go

**Analogy:** Buying a toolbox. Check it is in your room.

```powershell
go version
# go version go1.23.5 windows/amd64
```

If you see a version number → Go is ready.

- [ ] I understand: `go version` checks if Go is installed

---



## Lesson 2 — Modules

**Analogy:** A student ID card. `go.mod` says who this project is.

```powershell
go mod init github.com/you/go-workshop
```

**go.mod looks like:**

```
module github.com/you/go-workshop

go 1.23.5
```

- Line 1 = project name
- Line 2 = minimum Go version

**go.sum** — ignore for now. Appears when you download code from the internet.

- [ ] I understand: `go.mod` is my project's name tag

---



## Lesson 3 — First program

**Analogy:** Every shop needs a front door. Go starts at `func main()`.

```go
package main       // Rule 1: must be "main"

func main() {      // Rule 2: must have this
    fmt.Println("Hello!")
}
```

Both rules required. Change either → program won't run.

- [ ] I understand: `package main` + `func main()` = start button

---



## Lesson 4 — Tooling (5 daily commands)

**Order pros use:** fmt → vet → test → run → build


| Command                   | What it does     | Good output           |
| ------------------------- | ---------------- | --------------------- |
| `go fmt ./...`            | Auto-format code | File names or silence |
| `go vet ./...`            | Find logic bugs  | Silence = success     |
| `go test -v ./...`        | Run tests        | `PASS`                |
| `go run .`                | Run without .exe | Your print output     |
| `go build -o greet.exe .` | Save as .exe     | Creates `greet.exe`   |


**Analogies:**

- **fmt** — auto-indent in Word
- **vet** — spell-check for logic
- **test** — quiz your code
- **run** — cook and serve immediately
- **build** — pack lunch for later



### Real terminal practice

```powershell
cd "e:\Career Track\Focused Area\Development\Learnings\go-workshop"
go fmt ./...
go vet ./...
go test -v ./...
go run .
go build -o greet.exe .
.\greet.exe
```

- [ ] I tried all 5 tools and understand each one

---



## Tips

**go fmt not updating editor?**  
`go fmt` changes the file on disk. Reload the tab: `Ctrl+Shift+P` → **Revert File**.

**Module path:** Your `go.mod` may use your own name (e.g. `github.com/shuvo/...`) — that is fine.

---



## Progress tracker

- [x] Lesson 1 — Install Go
- [x] Lesson 2 — Modules
- [x] Lesson 3 — First program
- [x] Lesson 4 — Tooling

*Last synced from Cursor canvas lab.*
