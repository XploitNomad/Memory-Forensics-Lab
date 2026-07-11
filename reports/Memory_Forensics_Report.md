# Memory Forensics Investigation Report

## Objective

Perform basic analysis of a Windows memory image using Volatility 3.

---

## Image Information

Image Name

```
charlie-2009-12-11.windbgimage
```

Operating System

```
Windows XP
```

---

## Analysis Performed

### Windows Information

Collected operating system metadata including kernel information and system details.

---

### Running Processes

Enumerated all active processes from memory.

Examples observed:

- System
- smss.exe
- winlogon.exe
- services.exe
- explorer.exe
- lsass.exe
- svchost.exe
- spoolsv.exe
- thunderbird.exe

---

### Process Tree

Verified process hierarchy.

Observed expected parent-child relationships such as:

System

↓

smss.exe

↓

winlogon.exe

↓

services.exe

↓

svchost.exe

Explorer.exe was identified as the user shell process.

---

## Conclusion

This investigation demonstrates the ability to perform basic Windows memory analysis using Volatility 3. The project covers system identification, process enumeration, and process hierarchy analysis, forming a foundation for advanced memory forensic investigations.
