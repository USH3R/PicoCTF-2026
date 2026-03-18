# Corrupted Files

**Category:** Forensics  
**Challenge Source:** [PicoCTF](https://picoctf.org/)  
**Challenge Description:**  
We are given a file that seems broken. The goal is to inspect the file, fix the corruption, and recover the hidden flag.  

---

## Files Provided
- `corrupted_file` – The corrupted JPEG file provided by the challenge.

---

## Steps Taken / Solution Approach

1. **Inspect the File**
   ```bash
   file corrupted_file
   hexdump -C corrupted_file | head

   ## Skills Demonstrated / Learned
- **File Forensics** – Understanding file signatures and headers, specifically JPEG format.  
- **Hexadecimal Analysis** – Reading and interpreting raw file bytes using hex editors.  
- **File Recovery** – Manually repairing corrupted files by modifying header bytes.  
- **Command-Line Tools** – Using `file`, `hexdump`, and other utilities for file inspection.  
- **Attention to Detail** – Comparing actual vs. expected file headers to locate corruption.  
- **Problem-Solving** – Applying small, precise changes to recover hidden data (the flag).  
- **Digital Investigation Mindset** – Approaching a “broken” file methodically to extract meaningful information.
