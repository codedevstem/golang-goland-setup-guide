# Setup guide for Goland

## Golang 1.11+ Go modules

### Installation

For installing Goland or any other of the Jetbrains tools I recommend using the Jetbrains Toolbox. [Link](https://www.jetbrains.com/toolbox-app/)
This makes installing and updating Goland a trivial matter and is available for free 

### Configuration

#### Setting

Once you have started Goland.

1. Click 'configure' button in the lower right corner
2. Click 'settings'
3. Click 'Go' on the top
4. Click 'Go Modules (vgo)'
5. Check 'Enable Go Modules (vgo) integration'
6. Apply and Exit settings

### Usage

Once you have created your golang-project

1. Open a terminal
2. Write ```go mod init github.com/<username>/<repository>```
3. Create ```main.go```
4. Create ```src/yourmodule/yourmodule.go```
5. Remember to capitalize the functions and types that you want exported from the class
6. Use the function in ```main.go``` and save
7. Goland should now have automatically added an import statement for your new function
8. Run the program by either 
    -   Right-clicking on `main.go -> 'run go build main.go'`
    -   Writing `go build main.go && ./main` 
### Example of finished structure

```
.
├── src
|   └── yourmodule
|   	└── yourmodule.go
└── mod.go
└── main.go
```



