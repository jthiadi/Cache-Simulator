# Cache Simulator

This repository contains an implementation of a cache simulator that reads cache configuration files and memory reference traces, then reports cache hits and misses for each reference — along with the total miss count.

---

## 🛠 Environment (MobaXterm)

This project is intended to be built and run inside:

- **MobaXterm terminal**
- With access to:
  - `g++`
  - `make`
  - A Linux-like shell (remote server or local subsystem)

---

## ⚙️ Build Instructions

Open **MobaXterm** and navigate to the project directory:

```bash
cd path/to/project
```

Then build the program:

```bash
make
```

This will compile the program into an executable named:

```
project
```

To remove compiled files:

```bash
make clean
```

---

## ▶️ Running the Simulator

The program expects **three arguments**:

1. Cache configuration file (`.org`)
2. Memory reference trace file (`.lst`)
3. Output report filename

Example:

```bash
./project config/cache1.org bench/reference1.lst out.rpt
```

This will generate a report file named:

```
out.rpt
```

---

## 📤 Viewing the Output (using `cat`)

To display the generated report in the terminal:

```bash
cat out.rpt
```

---

## 📄 Output Report Includes

- Cache configuration parameters  
- Derived offset and indexing bit counts  
- Indexing bit order  
- Each memory access result (`hit` / `miss`)  
- Total cache miss count  

---
