# Ejercicio Github Actions 

## Ejercicio 1

    1) Se debe de crear un directorio en la raíz de proyectos que sea .github/workflow
    2) Dentro de ese directorio se crean archivos .yml o .yaml que será las instrucciones de las acciones o la pipeline de github.
    3) Se crea una para hacer el CI que se pide de la aplicacion en Javascript y la explicacion de cada pasa viene detallada dentro.
    4) Una vez terminado para enviarlo al repositorio se hace el git add, commit y push.
    5) Te metes en el directorio del proyecto y te vas a ACtions, dentro de Actions te vas al panel izquierdo y seleccionas el worflow correspondiente y le das al boton verde de la derecha que pone "Run workflow".
    6) Debería de aparecerte la pipeline ejecutandose con un icono amarillo que indica que está ejecutandose y puedes entrar y ver los jobs y las actions ejecutandose en tiempo real.
    7) Por ultimo se verá si todos los jobs se han ejecutado con satifsaccion.
    8) En mi caso el de "test" fallaba, pero era porque el codigo en si fallaba.

        `![test_error(https://imgur.com/a/topfJHU)]`

## Ejercicio 2

    1) Se crea un segundo archivo de .yml en la carpeta workflow donde irá la siguiente pipeline que será hacer un CD de la misma aplicación.
    2) La explicación de cada paso viene en el propio archivo.
    3) Hizo falta buscar una acción en internet que permitiera hacer un build y push a la vez al Github packages de donde se pueden almacener docker contaienrs.
    4) Se crea el GITHUB_TOKEN que hará falta para subirlo. Este token se crea de una manera diferente a como se hizo y la clase y en realidad hay que ir dentro de la funcion de Settings pinchando en nuestro avatar de Github en la esquina superior derecha y luego ir a Developer Settings y en Developer Settings se pincha en Personal Access Tokens. 
    Una vez dentro se seleccionan los permisos que se deseen y en este caso se necesitan los de write:packages y delecte:packages, pero sobre todo para este ejecicio el de write:packages.
    5) Se sube el fichero al repositorio con un commit-push
    6) Se ejecuta la pipeline de la misma manera que el ejercicio anterior y una vez que se completen todos los pasos con éxito se va a packages en nuestro perfi home de github y se comprueba que el container se ha creado y subido correctamente.
    
    `![Ejercicio2_completado(https://imgur.com/UH8j5E3)]`
    
    [Para ver el container](https://github.com/josekuma/git-actions-playground/pkgs/container/hangman-front)


