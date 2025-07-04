<p align="center">
<pre>
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠤⣴⣶⣶⣶⣶⣦⣤⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⣀⣴⣾⣿⣶⣄⠈⠻⣿⣿⣿⣿⣿⣿⡀⢰⣦⣀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⢠⣾⣿⣿⣿⣿⣿⣿⣿⣷⣤⡀⠙⢿⣿⣿⣿⡇⠀⣿⣿⣷⡄⠀⠀⠀
⠀⠀⠀⡰⠿⠿⠿⠿⠛⠛⠛⠛⠋⠉⠉⠀⠀⠈⠻⣿⡇⠀⣿⣿⣿⣿⣆⠀⠀⠀
⠀⠀⣀⣤⣤⣤⣤⣴⣶⠖⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠁⠀⣿⣿⣿⣿⡿⠂⠀⠀
⠀⢀⣿⣿⣿⣿⣿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢹⣿⣿⠋⢀⣴⡀⠀
⠀⢸⣿⣿⣿⡿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⠟⠁⣠⣾⣿⡇⠀
⠀⢸⣿⣿⠋⢀⣴⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣾⣿⣿⣿⡇⠀
⠀⠈⠟⠁⣠⣿⣿⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣿⣿⣿⣿⣿⠁⠀
⠀⠀⠠⣾⣿⣿⣿⣿⠀⢠⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠴⠿⠿⠟⠛⠛⠛⠋⠀⠀
⠀⠀⠀⠹⣿⣿⣿⣿⠀⢸⣿⣦⣄⠀⠀⣀⣀⣀⣤⣤⣤⣤⣤⣶⣶⣶⠆⠀⠀⠀
⠀⠀⠀⠀⠘⢿⣿⣿⡄⠸⣿⣿⣿⣷⣄⡈⠙⢿⣿⣿⣿⣿⣿⣿⡿⠃⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠉⠻⠇⠀⣿⣿⣿⣿⣿⣿⣦⡀⠉⠻⣿⡿⠟⠉⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠛⠻⠿⠿⠿⠟⠓⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
</pre>
</p>

## TRKG Features

```bash
# Basic usage
trkg [command] [options] [arguments]
```

### Command Reference

| Command  | Usage                          | Description                          |
|----------|--------------------------------|--------------------------------------|
| init     | `trkg init <package-name>`     | Create new package template          |
| build    | `trkg build <path>`            | Build package                        |
| install  | `trkg install <package.trkg>`  | Install package                      |
| remove   | `trkg remove <package-name>`   | Remove package                       |
| search   | `trkg search <keyword>`        | Search packages                      |
| upgrade  | `trkg upgrade`                 | Upgrade all installed packages       |
| list     | `trkg list [--installed]`      | List packages                        |
| info     | `trkg info <package-name>`     | Show package details                 |

---

## System Requirements

### Required Dependencies

```bash
# Debian/Ubuntu
sudo apt update && sudo apt install -y \
    libcurl4-openssl-dev \
    libssl-dev \
    libcjson-dev \
    openssl
```

### Minimum Versions

| Package   | Version     | Check Command          |
|-----------|-------------|------------------------|
| OpenSSL   | ≥ 1.1.x     | `openssl version`      |
| libcurl   | ≥ 7.64.0    | `curl --version`       |
| libcjson  | ≥ 1.7.14    | `dpkg -l libcjson-dev` |

---

## License Information

**TRKG - Lightweight ARM Package Manager**  
Copyright (C) 2025 dreamtech.dev & FreeC-14

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License v3.0.  
This program comes WITHOUT ANY WARRANTY.

*Full license text: See the LICENSE file*

---

## Contribution Process

1. **Fork the repository**  
   Click Fork on GitHub

2. **Develop**
   ```bash
   git clone https://github.com/your-username/trkg-arm.git
   cd trkg-arm
   git checkout -b feature-branch
   ```

3. **Commit and push changes**
   ```bash
   git add .
   git commit -m "Add new feature xyz"
   git push origin feature-branch
   ```

4. **Create a Pull Request**  
   Open a PR from your feature branch to the main repo

---

## Troubleshooting

### Common Issues

**Error: Missing dependencies**
```bash
# Solution:
sudo apt --fix-broken install
```

**Error: ARM architecture mismatch**
```bash
# Check architecture:
dpkg --print-architecture
uname -m
```

**Error: Permission denied**
```bash
# Solution:
sudo chmod +x /usr/local/bin/trkg
```

---

## Contact & Support

| Platform        | Link                  |
|-----------------|-----------------------|
| GitHub Issues   | [Open Issue]          |
| Email           | sussyarch@proton.me   |
| Discord         | [Join Server]         |

---

> Developed by dreamtech.dev & FreeC-14  
Last update: 2025
```
