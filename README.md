# Əks mühəndislik: x86-64 və ARM arxitekturalarında binar analiz və zərərli proqramların tədqiqi

Source code and lab materials for the Azerbaijani textbook *"Reverse engineering: binary analysis
and malware research on x86-64 and ARM architectures"* by **Asif Qanbayev**.

## Contents

| Archive | Chapter |
| :--- | :--- |
| `fesil01_menbe_kodlari.zip` | 1. Əks mühəndisliyə giriş |
| `fesil02_menbe_kodlari.zip` | 2. C kodundan maşın koduna |
| `fesil03_menbe_kodlari.zip` | 3. ELF formatı |
| `fesil04_menbe_kodlari.zip` | 4. Laboratoriya mühiti |
| `fesil05_menbe_kodlari.zip` | 5. x86-64 assembly |
| `fesil06_menbe_kodlari.zip` | 6. ARM assembly |
| `fesil07_menbe_kodlari.zip` | 7. C konstruksiyaları iki arxitekturada |
| `fesil08_menbe_kodlari.zip` | 8. MIPS-ə giriş |
| `fesil09_menbe_kodlari.zip` | 9. PE formatı |
| `fesil10_menbe_kodlari.zip` | 10. Windows binarlarının daxili quruluşu |
| `fesil11_menbe_kodlari.zip` | 11. Statik analiz (Ghidra, IDA Free, radare2) |
| `fesil12_menbe_kodlari.zip` | 12. Linux-da dinamik analiz |
| `fesil13_menbe_kodlari.zip` | 13. Windows-da dinamik analiz |
| `fesil14_menbe_kodlari.zip` | 14. Emulyasiya (QEMU, Unicorn, Qiling) |
| `fesil15_menbe_kodlari.zip` | 15. Obfuskasiya və anti-analiz |
| `fesil16_menbe_kodlari.zip` | 16. Analiz metodologiyası, göstəricilər, YARA və hesabat |
| `fesil17_menbe_kodlari.zip` | 17. Praktik analiz: Windows nümunəsi |
| `fesil18_menbe_kodlari.zip` | 18. Praktik analiz: Mirai |
| `fesil19_menbe_kodlari.zip` | 19. Praktik analiz: Gafgyt və Tsunami |
| `fesil20_menbe_kodlari.zip` | 20. Analizin avtomatlaşdırılması |
| `fesil21_menbe_kodlari.zip` | 21. Crackme və CTF tapşırıqları |
| `fesil22_menbe_kodlari.zip` | 22. Yekun layihə |
| `elaveler_menbe_kodlari.zip` | Əlavə A. Linux sistem çağırışlarının nömrələri |
| `laboratoriya_windows/` | Windows lab packages for chapters 13, 15-18 |

Every archive has a `README.txt` describing its files and how to build and run them.
From chapter 11 on, `*.spec` files and `session.py` reproduce the exact commands of the
book's listings, and `results_book/` (or `out_book/`) holds the outputs quoted in the book.

## Safety

* No real malware is distributed here. Real samples discussed in the book are referenced
  by SHA-256 and public collections (MalwareBazaar, vendor reports).
* Mirai, Gafgyt and Tsunami are studied from public source code; the scripts fetch the
  sources and compile only harmless parts (for example the Mirai string table).
* Run everything in an isolated analysis VM without network access.

## Toolchain

Ubuntu 24.04, GCC 13.3, Clang/LLD 18, NASM, QEMU user-mode, GDB, Ghidra 12.x with JDK 25,
YARA 4.5, Python 3 (pefile, pyelftools, capstone, yara-python, z3). Windows labs: FLARE VM
(x64dbg, Procmon, PE-bear, Ghidra).
