# Resolucion 1er ejercicio
cd /home
echo "Soy el usuario $USER y estoy parado en mi Directorio home que está ubicado en: $HOME"

# Resolucion 2do ejercicio 
mkdir -p proyecto/{docs/{pdfs,imagenes},src/{bash,python},backups}
proyecto/
 ├── docs/
 │     ├── pdfs/
 │     └── imagenes/
 ├── src/
 │     ├── bash/
 │     └── python/
 └── backups/
# Resolucion 3er ejercicio
echo "PC: $(hostname)" > Info-pc.txt
echo "Modelo CPU: $(grep 'model name' /proc/cpuinfo | head -n1 | cut -d: -f2)" >> Info-pc.txt
echo "IP: $(hostname -I | awk '{print $1}')" >> Info-pc.txt
PC: linux-practice
Modelo CPU:  AMD Ryzen 5 3600 6-Core Processor
IP: 192.168.1.50
