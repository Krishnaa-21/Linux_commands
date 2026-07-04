# 🌐 Essential Linux Networking Commands

This document covers some of the most commonly used Linux networking commands for troubleshooting, monitoring, and network management.

---

## 1. `ping`

**Description**

Checks connectivity between your system and a remote host by sending ICMP Echo Request packets.

### Syntax

```bash
ping <host>
```

### Example

```bash
ping google.com
```

---

## 2. `netstat`

**Description**

Displays active network connections, listening ports, routing tables, and network statistics.

> **Note:** `netstat` is considered legacy. Use `ss` on modern Linux distributions.

### Syntax

```bash
netstat [options]
```

### Example

```bash
netstat -tuln
```

**Common Options**

| Option | Description |
|---------|-------------|
| `-t` | Show TCP connections |
| `-u` | Show UDP connections |
| `-l` | Show listening ports |
| `-n` | Display numerical addresses |

---

## 3. `ifconfig` (Legacy)

**Description**

Displays or configures network interfaces.

> **Note:** `ifconfig` has been replaced by the `ip` command on modern Linux systems.

### Syntax

```bash
ifconfig
```

### Example

```bash
ifconfig
```

---

## 4. `ip`

**Description**

Modern utility for managing network interfaces, IP addresses, routes, and more.

### Syntax

```bash
ip <object> <command>
```

### Example

```bash
ip a
```

or

```bash
ip addr show
```

---

## 5. `traceroute`

**Description**

Displays the route packets take from your system to a destination host.

### Syntax

```bash
traceroute <host>
```

### Example

```bash
traceroute google.com
```

---

## 6. `ip route`

**Description**

Displays or modifies the system routing table.

### Syntax

```bash
ip route
```

### Example

```bash
ip route
```

---

## 7. `mtr`

**Description**

Combines the functionality of **ping** and **traceroute** to provide real-time network diagnostics.

### Syntax

```bash
mtr <host>
```

### Example

```bash
mtr google.com
```

---

## 8. `wg` (WireGuard)

**Description**

Manages and displays WireGuard VPN interfaces and peer information.

### Syntax

```bash
wg
```

### Example

```bash
sudo wg show
```

---

## 9. `ss`

**Description**

Displays socket statistics, active network connections, and listening ports.

> **Note:** `ss` is the modern replacement for `netstat`.

### Syntax

```bash
ss [options]
```

### Example

```bash
ss -tuln
```

**Common Options**

| Option | Description |
|---------|-------------|
| `-t` | TCP sockets |
| `-u` | UDP sockets |
| `-l` | Listening sockets |
| `-n` | Show numerical addresses |

---

## 10. `iptables`

**Description**

Configures and manages Linux firewall rules.

### Syntax

```bash
iptables [options]
```

### Example

```bash
sudo iptables -L
```

---

# 📚 Quick Reference

| Command | Purpose |
|----------|---------|
| `ping` | Test network connectivity |
| `netstat` | View network connections (Legacy) |
| `ifconfig` | View network interfaces (Legacy) |
| `ip` | Modern network configuration utility |
| `traceroute` | Trace packet route to a destination |
| `ip route` | Display routing table |
| `mtr` | Real-time network diagnostics |
| `wg` | Manage WireGuard VPN |
| `ss` | View socket statistics (Modern) |
| `iptables` | Configure firewall rules |

---

> **Recommended for Modern Linux Systems**
>
> Prefer using:
>
> - `ip` instead of `ifconfig`
> - `ss` instead of `netstat`
> - `nftables` instead of `iptables` (on newer distributions)
