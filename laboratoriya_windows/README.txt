Windows lab packages (chapters 13, 15, 16, 17, 18)

Each archive contains the files to copy into the FLARE VM (or another isolated Windows
analysis VM) and PROTOCOL.txt with the exact steps and expected results.

The .exe files are the book's own harmless training programs (win_beacon, agent17,
antidbg_win, crackme_pe_upx, ...). They were built from the sources in the corresponding
chapter archives and imitate malware behaviour (beacons to 127.0.0.1, encrypted
configuration, anti-debug checks, UPX packing) without any harmful function. Some antivirus
products may still flag them because of this behaviour; rebuild them from source if you
prefer. lab18 contains the Mirai string-table harness and object files only (no bot code).
