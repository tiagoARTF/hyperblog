echo "Este archivo corresponde al taller evaluativo de principios de criptografia" > ejercicio2.txt


openssl enc -aes-256-cbc -salt -pbkdf2 -in ejercicio2.txt -out archivo_cifrado.enc


openssl enc -aes-256-cbc -d -pbkdf2 -in archivo_cifrado.enc -out archivo_descifrado.txt


cat archivo_descifrado.txt





















Y como un amable recordatorio: **Este readme.md es un chiste**.  Diseñado para el ejemplo. Si llegas acá NO TE LO TOMES EN SERIO y mejor ve [**a ver el curso**](https://platzi.com/cursos/git-github/ "a ver el curso").
