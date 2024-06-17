# Chat-Bot
# Pasos a seguir<br />
> 1. Descarga Anaconda: https://www.anaconda.com/download<br />
> 2. Abre la aplicaion anaconda prompt<br />
> 3. Crea un nuevo un nuevo enviroment (solo debes de hacerlo la primera vez): <br /> conda create -n Chatbot python=3.6 <br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/72c8ff7f-9900-4cd0-93ca-c02464fa95da)
> 4. Activa en enviroment creado se vera asi: <br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/3525f2bf-63b6-4384-a05c-ebf75c4a2776)
> 5. Descarga desde este torrent todo la informacion de reddit:<br /> magnet:?xt=urn:btih:32916ad30ce4c90ee4c47a95bd0075e44ac15dd2&dn=RC%5F2015-01.bz2&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A80&tr=udp%3A%2F%2Fopen.demonii.com%3A1337&tr=udp%3A%2F%2Ftracker.coppersurfer.tk%3A6969&tr=udp%3A%2F%2Ftracker.leechers-paradise.org%3A6969<br />
>> - O puedes descargar con este link un solo mes solo ten en cuenta que el bot estara limitado si no tiene la suficiente informacion: https://mega.nz/file/ysBWXRqK#yPXLr25PgJi184pbJU3GtnqUY4wG7YvuPpxJjEmnb9A<br />
> 6. Ya con la informacion lo colocaras en una carpeta nueva donde quieras guardar tu proyecto<br />
> 7. Ahora tendras que usar 2 programas que se llaman chatbot_database y create_training_data<br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/b820b966-e6ab-4a42-80a3-73114996b073)
>> - El primero sirve para hacer una base de datos ordeanda de la informacion descargada los unicos cambios que debes de hacer son:<br />
>>> - ![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/40775ed7-1c77-487f-b2c0-1d265d7bb992) <br />Tendras que cambiar lo que esta entre comillas con el mes que deseas hacer la base de datos despues de eso lo dejas correr dependiendo que tan grande quieras que sea tu base de datos es importante que corras este programa primero<br />
>>> - ![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/c143be86-1bce-4e2c-8feb-8026474582ab) Aqui pondras la direccion de la carpeta en la que se encuentra el archivo RC descargado si tienes el archivo suelto en la carpeta no funcionara debes de crear un carpeta donde pongas el año del archivo RC con el que trabajas asi:<br /> ![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/3863d8d9-7b89-48bc-b4e8-e048e1708168)
>>>  Este programa no se debe parar.
>> - El segundo tiene la funcion de convertir esta informacion en 2 archivos trein.to y train.from esto con el fin de separar la informacion en una especie de preguntas y respuestas que al fianl es como funciona reddit, aqui solo tendras que cambiar el time frame donde pondras la base de datos creada en el anterior programa<br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/9369815b-f7aa-4d27-b2ac-6bd0395f6546)
> 8. Ahora instalaremos git para clonar los repositorios: conda install git con<br />
> 9. Creamos una carpeta en la cual guardaremos el repositorio<br />
> 10. Ahora si estas en windows pondras en anaconda prompt cd "Tu direccion de la carpeta donde quieres que se clone el repositorio" esto con el fin de ir a esa direccion <br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/04905d93-6c79-46d1-a483-47f745ef131a)
> 11. Usaremos directamente esta linea de codigo: __git clone --recursive https://github.com/daniel-kukiela/nmt-chatbot__
> 12. Entramos a la carpeta recien creada que deberia llamarse nmt-chatbot:<br /> **cd nmt-chatbot**
> 13. Ahora en cualquier IDLE de corra python abriras este programa:<br />
>> - ![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/86ecfc39-18f5-4da5-a267-fe351c80e68e) el cual esta ubicado dentro de la carpeta ![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/b4b27e4b-1cc1-4899-aaca-6a6bef82ffa5) el cual tiene una gran cantidad de variables con las que se puede jugar pero las principales son 2:<br />
>>> - vocab_size el cual sirve para saber cuantas palabras claves va tokenizar para usarlas en su entranmeinto entre mas grande sea puede que tenga un vocabulario mas variado <br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/5e643490-561e-4032-bb79-4eab7b5cd9ee)
>>> - Y batch size esta opcion esta coemntada pues el entrenamiento se adapta al procesador que tengas pero creo que es mejor poder decidir cuanto quieres forzar tu pc yo lo le usado en 64 y funcioan muy bien:<br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/2f2aef08-626e-4ed0-bab6-559e42983d88)
> 14. Ahora directamente ve a tu carperta donde este tu proyecto y entra a la carpeta llamada new_data<br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/63a5d558-c03e-4172-b7a0-ad4c7218e7fc)
>> - Ahi sustituiras los 2 archivos que creaste con training data que eran train.to y train.from los otros los puedes ignorar<br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/85fac373-6455-4bba-8ed7-805134d1d764)
> 15. ya que esta listo todo lo que no es directamente con anaconda volvemos al anaconda propmt y desde donde lo dejamos que seria que estamos en la carpeta de nmt-chatbot usaremos una linea con la cual se instalara todo lo necesario para que corran los programas internos del entrenamiento<br />  ![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/0e9bddfa-b9af-4ae1-a95d-fa0da1c2008f)
> 16. hay que escribir cd setup para entrar a la carpeta por medio del enviroment ya que los requisitos que se ocupan solo estan instalados en este enviroment, ahora usaremos: python prepare_data.py para que se prepare la informacion que le subimos y con la que entrenara el bot
> 17. volvemos a la carpeta princiapl con: cd ../
> 18. Y usamos <br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/a01ac1a2-0dcf-42ee-88f7-d9abd9e82b62) <br /> con el fin de empezar a entrenar a tu bot
> 19. Ya que se este entrenando saldra esto cada 100 pasos los pasos se refiere a las iteraciones que hace el entrenamiento:<br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/cf8c93ec-a03d-4213-8bda-971995b3db9d)<br />Cada 100 paso se dara un informe como este en el cual te dira informacion importante como lo es cuanto tarda en dar cada paso, las palbaras por segundo usadas, ppl que es perplexity un IA la cual ayuda a que nuestro bot maneje un lenguaje natural entre mas bajo es mejor, el gn que es el gradiente normal el cual se debe de mantener bajo e indica si va explotar o no el entranmiento en pocas palabras y el bleu el cual debe de subir y significa cuanto elocuencia y sentido tiene los textos que escribe segun la el texto que tu le pongas.<br />Toma en cuenta que el belu al menos en mi caso no subio y que puede que tenga momentos en medio del entrenamiento que empiece a hablar con soltura si lo vez en condiocnes para el programa pues si se deja mucho tiempo puede que en el siguiente checkpoint deje de decir cosas coherentes
> 20. en medio del entrenamiento puedes probarlo abre otro anaconda prompt y activa tu enviroment del chat bot dirigite a la carpeta del proyecto dentro de nmt y escribe python inference.py <br /> Con esto podras porbar como va tu bot y preguntarle cosas:<br />![image](https://github.com/salvador0401/Chat-Bot/assets/77693692/9c5eb422-1b5e-434c-9e55-144544bb5837)
  





