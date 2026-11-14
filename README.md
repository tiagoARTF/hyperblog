openssl genpkey -algorithm RSA -out firma_privada.pem

echo "Documento a firmar por parte de los estudiantes" > ejercicio3.txt

openssl dgst -sha256 -sign firma_privada.pem -out firma.bin ejercicio3.txt

openssl rsa -pubout -in firma_privada.pem -out firma_publica.pem

openssl dgst -sha256 -verify firma_publica.pem -signature firma.bin ejercicio3.txt
























Y como un amable recordatorio: **Este readme.md es un chiste**.  Diseñado para el ejemplo. Si llegas acá NO TE LO TOMES EN SERIO y mejor ve [**a ver el curso**](https://platzi.com/cursos/git-github/ "a ver el curso").
