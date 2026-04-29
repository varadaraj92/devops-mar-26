#!/bin/bash

echo "===== SYSTEM INFORMATION ====="

echo "Hostname: $(hostname)"
echo "OS: $(uname -o)"
echo "Kernel Version: $(uname -r)"
echo "Architecture: $(uname -m)"

echo ""
echo "===== CPU INFORMATION ====="
echo "CPU Model: $(lscpu | grep 'Model name' | cut -d ':' -f2)"
echo "CPU Cores: $(nproc)"

echo ""
echo "===== MEMORY INFORMATION ====="
free -h

echo ""
echo "===== DISK USAGE ====="
df -h

echo ""
echo "===== UPTIME ====="
uptime

echo ""
echo "===== CURRENT USER ====="
whoami

echo ""
echo "===== IP ADDRESS ====="
hostname -I

echo ""
echo "===== RUNNING PROCESSES (Top 5) ====="
ps -eo pid,ppid,cmd,%mem,%cpu --sort=-%cpu | head -n 6
