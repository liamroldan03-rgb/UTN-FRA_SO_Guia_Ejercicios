# Resolucion 1er ejercicio
A1    A2    A3
B1,B2,B3
C1    C2,C3
D1    D2    D3   D4   D..n
sudo tee archivo.txt > /dev/null << 'EOF'
A1    A2    A3
B1,B2,B3
C1    C2,C3
D1    D2    D3   D4   D..n
EOF
A1    A2    A3
B1,B2,B3
C1    C2,C3
D1    D2    D3   D4   D..n

# Resolucion 2do ejercicio 
awk 'NR==1 {print $2}' archivo.txt
awk -F',' 'NR==2 {print $2}' archivo.txt
awk 'NR==3 {split($2,a,","); print a[1]}' archivo.txt
awk 'NR==4 {$1=""; sub(/^ /,""); print}' archivo.txt
