echo "Mensaje secreto para cifrar de la clase principios de criptografia" > ejercicio1.txt




openssl rsautl -encrypt -inkey clave_publica.pem -pubin -in ejercicio1.txt -out mensaje_cifrado.bin


openssl rsautl -decrypt -inkey clave_privada.pem -in mensaje_cifrado.bin -out mensaje_descifrado.txt


cat mensaje_descifrado.txt





















Y como un amable recordatorio: **Este readme.md es un chiste**.  Diseñado para el ejemplo. Si llegas acá NO TE LO TOMES EN SERIO y mejor ve [**a ver el curso**](https://platzi.com/cursos/git-github/ "a ver el curso").
