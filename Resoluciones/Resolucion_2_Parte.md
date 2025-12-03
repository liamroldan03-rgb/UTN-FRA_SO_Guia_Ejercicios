# Resolucion 1er ejercicio
sudo useradd usuario1
sudo passwd usuario1

# Resolucion 2do ejercicio
sudo groupadd Grupo1
sudo useradd -G Grupo1 usuario2
sudo passwd usuario2

# Resolucion 3er ejercicio
sudo groupadd Grupo2
sudo groupadd Grupo3
sudo grep usuario1 /etc/shadow
usuario1:$6$T1J....$yH8.....:...
$6$T1J....$yH8.....
sudo useradd -m -g Grupo1 -G Grupo2,Grupo3 -p '$6$T1J....$yH8.....' usuario3

#Resolucion 4to ejercicio 
sudo useradd -m -d /otroHome usuario4
sudo passwd usuario4
sudo usermod -aG Grupo3 usuario4

# Resolucion 5to ejercicio
grep usuario1 /etc/passwd
grep usuario1 /etc/shadow
ls -ld /home/usuario1
ls -ld /otroHome       # usuario4
grep usuario1 /etc/passwd
groups usuario1
groups usuario2
groups usuario3
groups usuario4
sudo grep usuario1 /etc/shadow
