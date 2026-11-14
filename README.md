openssl rsa -pubout -in clave_privada.pem -out clave_publica.pem
echo "Mensaje..." > ejercicio1.txt

openssl rsautl -encrypt -inkey clave_publica.pem -pubin -in ejercicio1.txt -out mensaje_cifrado.bin

openssl rsautl -decrypt -inkey clave_privada.pem -in mensaje_cifrado.bin -out mensaje_descifrado.txt

cat mensaje_descifrado.txt

echo "Este archivo..." > ejercicio2.txt

openssl enc -aes-256-cbc -salt -pbkdf2 -in ejercicio2.txt -out archivo_cifrado.enc

openssl enc -aes-256-cbc -d -pbkdf2 -in archivo_cifrado.enc -out archivo_descifrado.txt

cat archivo_descifrado.txt

















# hyperblog
un blog increíble para el[ curso de Git y Github]
(https://platzi.com/cursos/git-github/ " curso de Git y Github") de [Platzi](https://platzi.com/ "Platzi")
> El curso de Git y Github de Platzi es lo que me hacía falta para triplicar mi salario y lanzarme a la industria del tejido de lana sintética con Machine Learning
> - niñita

## En este curso vemos de todo
* Todos los comandos de Git
* El flujo de trabajo en Github
* El verdadero amor por las buenas prácticas
* Trucos muy locos del profesor
* Las personalidades múltiples de Freddy

Y como un amable recordatorio: **Este readme.md es un chiste**.  Diseñado para el ejemplo. Si llegas acá NO TE LO TOMES EN SERIO y mejor ve [**a ver el curso**](https://platzi.com/cursos/git-github/ "a ver el curso").
