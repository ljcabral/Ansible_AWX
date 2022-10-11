Para generar un nuevo usuario, ejecutar el template "New User" de AWX.
Previamente a ésto, ingresar al servidor de ansible y generar una password hasheada ya que no permite ingresar passwords en plano:
- Ingresar al servidor lnv-da3229dans (172.31.3.229)
- Ejecutar el siguiente comando en el que nos pedira la contraseña a hashear: mkpasswd --method=sha-512
- Copiar el hash e ingresar en la variable "password" del template "New User".
