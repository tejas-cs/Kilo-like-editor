# Kilo  

A nano-like text editor built with pure C  

Kilo is a simple text editor inspired by the original [kilo](https://github.com/antirez/kilo) created by Salvatore Sanfilippo. This project serves as a way to learn more about handling TUI (Text User Interface) interactions without using any external libraries, including ncurses. Instead, Kilo uses standard VT100 (and similar terminals) escape sequences for text-based UI manipulation.  

Kilo is designed to be lightweight and easy to modify. People are encouraged to use it as a starting point for writing other text editors or command-line interfaces.  

## Preview 🙈  
![Kilo Editor Preview](./images/Screenshot(350).png) 
![Preview 2](./images/Screenshot(351).png)
![Preview 3](./images/Screenshot(352).png)

## Keybindings ⌨️  
| Shortcut       | Action             |  
|---------------|--------------------|  
| `Ctrl+Q`      | Quit Kilo          |  
| `Ctrl+S`      | Save file          |  
| `Ctrl+F`      | Find text          |  


## How to Install ⬇️  
### Clone this repo:  
```sh  
git clone https://github.com/yourusername/kilo.git  
cd kilo  
```  

### Compile the project:  
```sh  
make  
```  

### Run Kilo:  
```sh  
./kilo <filename>  
```  

### Optionally, install Kilo system-wide:  
```sh  
make install  
```  
Then restart your shell and run:  
```sh  
kilo <filename>  
```  

## Windows Support 🖥️  
Kilo relies on `termios` and `ioctl`, which do not work in the default Windows terminal. To run Kilo on Windows, you need to use **Cygwin** or **WSL (Windows Subsystem for Linux)**.  

### Running Kilo in Cygwin  
1. Install [Cygwin](https://www.cygwin.com/) with the **gcc** and **make** packages.  
2. Open the Cygwin terminal.  
3. Clone and compile Kilo:  
   ```sh  
   git clone https://github.com/yourusername/kilo.git  
   cd kilo  
   make  
   ```  
4. Run Kilo:  
   ```sh  
   ./kilo <filename>  
   ```  

### Running Kilo in WSL  
1. Install **WSL** with an Ubuntu distribution.  
2. Open WSL and follow the standard **How to Install** instructions.  

## Goals 🥅  
- [ ] Add visual mode (selection, copy, paste, delete)  
- [ ] Improve replace functionality  
- [ ] Add keyboard configuration (e.g., `CTRL+X` to exit)  
- [ ] Implement syntax highlighting configuration  
- [ ] Introduce a shell mode  
- [ ] Create an integrated help system
- [ ] Implement a VI mode  
- [ ] Add Vim mode  
- [ ] Implement line numbers  

## Work in Progress ⚒️  
This project is still in development!  

## Special Thanks 🙏  
Inspired by:  
- [viewsourcecode](https://viewsourcecode.org/)  
- [kilo](https://github.com/antirez/kilo)  

---

