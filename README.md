Ось детально розписаний опис інструменту `htop` у Markdown-форматі:

```markdown
# 📊 `htop` — Interactive Process Viewer

`htop` is a powerful, interactive process viewer for Unix systems. It is a more advanced and user-friendly alternative to the traditional `top` command.

---

## ✅ Features

- Real-time monitoring of system processes
- Colorful, customizable, and easy-to-read interface
- Horizontal and vertical scrolling
- Mouse support (select, kill, search)
- Process tree view
- CPU, Memory, Swap usage bars
- Easy process management (kill, renice, etc.)

---

## 🔧 Installation

### On Debian/Ubuntu:
```bash
sudo apt update && sudo apt install htop
```

### On Red Hat/CentOS/Fedora:
```bash
sudo dnf install htop
```

### On Arch Linux:
```bash
sudo pacman -S htop
```

---

## 🚀 Usage

### Start `htop`:
```bash
htop
```

### Common Keyboard Shortcuts:
| Key | Action                            |
|-----|-----------------------------------|
| `F1` | Help                              |
| `F2` | Setup (configure interface)       |
| `F3` | Search for process                |
| `F4` | Filter processes                  |
| `F5` | Tree view                         |
| `F6` | Sort by a selected column         |
| `F9` | Kill a process                    |
| `F10`| Quit                              |
| `Space` | Mark a process                 |
| `U`   | Unmark all processes             |
| `S`   | Trace system calls (strace)      |
| `L`   | Show open files (lsof)           |

---

## 📈 Interface Overview

- **Top Bar**: CPU(s), memory, and swap usage visual meters
- **Main Table**: List of running processes and stats
  - PID, USER, CPU%, MEM%, TIME+, Command
- **Footer**: Function keys and their mapped actions

---

## ⚙️ Configuration

Press `F2` to enter the setup menu, where you can:
- Change color schemes
- Customize columns
- Hide/show meters
- Set default sort order

Configuration is saved in:
```
~/.config/htop/htoprc
```

---

## 💡 Tips

- Use the **tree view (F5)** to easily visualize parent-child relationships between processes.
- Use `F6` to sort by `%MEM`, `%CPU`, or any column for quick performance diagnostics.
- Combine with `ssh` for remote monitoring:
  ```bash
  ssh user@server -t htop
  ```

---

## 🧩 Alternatives

- `top` — Traditional, more basic alternative  
- `glances` — Cross-platform, advanced monitoring tool  
- `atop` — Resource usage logger over time  

---

## 📚 More Info

- Website: [https://htop.dev](https://htop.dev)  
- GitHub: [https://github.com/htop-dev/htop](https://github.com/htop-dev/htop)

```
