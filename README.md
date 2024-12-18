# Text File Compressor  

A high-performance text file compression tool using the **Huffman Coding Algorithm** to optimize file sizes for efficient storage and transfer.  

---

## Overview  
This program reduces text file sizes by approximately **50%** using Huffman Compression, a widely-used data encoding technique. It ensures fast and secure data handling, maintaining data integrity while optimizing file transfer speeds.  

---

## Theory  
Huffman Compression works by creating an optimal binary tree based on the frequency of characters in the file. Characters with higher frequencies are assigned shorter binary codes, while less frequent characters are assigned longer codes, ensuring minimal overall file size.  

**Example Input String:**  
`AAABBCAAADDFFAAAADCCCDAADDDAAACGAAACACA`  

**Character Frequencies:**  
| Character | Frequency |  
|-----------|-----------|  
| A         | 20        |  
| B         | 2         |  
| C         | 7         |  
| D         | 7         |  
| F         | 2         |  
| G         | 1         |  

The binary tree is built using these frequencies, and the resulting Huffman codes are assigned as follows:  

| Character | Huffman Code |  
|-----------|--------------|  
| A         | 0            |  
| B         | 1011         |  
| C         | 11           |  
| D         | 100          |  
| F         | 10100        |  
| G         | 10101        |  

---

## Features  
- **High Compression Efficiency:** Achieves approximately 50% size reduction for text files.  
- **Speed:** Compresses and decompresses files efficiently.  
- **Integrity:** Ensures that decompressed files are identical to the original.  

---

## Usage  
1. **Compile the Program:**  
   ```bash  
   g++ huffman-compression.cpp -o compressor  

