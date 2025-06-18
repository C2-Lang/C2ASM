# ⚙️ C² Bytes Assembler (c2asm)

A lightweight assembler that compiles `.c2asm` assembly source files into `.c2b` bytecode,  
designed for the C² Virtual Machine (C2VM).  
Ideal for assembling human-readable assembly code into executable bytecode for C² projects.

<p align="center">
  <img src= "https://cdn.discordapp.com/attachments/1153973442824118323/1384884686920089701/c2vmLogo.png?ex=68540ddf&is=6852bc5f&hm=086d39d04ccd84b89a7f09debe6fa70d441adb622082bc4f3468f8f23a417474&"/>
</p>


---

## 🚀 Features

- Compiles `.c2asm` source code into `.c2b` bytecode files  
- Supports full C² assembly instruction set  
- Simple command-line interface  
- Fast and lightweight  
- Ideal for educational purposes and embedded scripting  

---

## 🛠 Installation & Building

Clone the repository and build using your preferred toolchain:

```bash
git clone https://github.com/C2-Lang/C2ASM.git
cd c2asm
make
````

---

## ⚙️ Usage

Compile a `.c2asm` file into `.c2b` bytecode:

```powershell
c2vmasm.exe -o <output dir> <file.c2asm>
```
The compiled file will be placed inside the output directory
---

## 📝 Example Program

Here is a simple `.c2asm` program to print "Hello, World!":

```asm
start:
    push 72    ; H
    syscall 1
    push 101   ; e
    syscall 1
    push 108   ; l
    syscall 1
    push 108   ; l
    syscall 1
    push 111   ; o
    syscall 1
    push 44    ; ,
    syscall 1
    push 32    ; (space)
    syscall 1
    push 87    ; W
    syscall 1
    push 111   ; o
    syscall 1
    push 114   ; r
    syscall 1
    push 108   ; l
    syscall 1
    push 100   ; d
    syscall 1
    push 33    ; !
    syscall 1
    push 10    ; newline
    syscall 1
    halt
```

For more info regarding the instruction set and more examples please visit [C2VM Repository](https://github.com/C2-Lang/C2ASM/) OR look at the examples
---

## 🧩 Integration with C2VM

Run the compiled bytecode on C² Virtual Machine:

```bash
c2vm <directory>/hello_world.c2b
```

---

## 📄 License

This project is licensed under the **MIT License**.
Feel free to use, modify, and distribute as you wish with or without credit.

## 💡 Contributions

Contributions, bug reports, and feature requests are welcome!
Please open issues or submit pull requests on GitHub.
