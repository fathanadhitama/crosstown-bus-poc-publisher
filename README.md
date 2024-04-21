# Tutorial 8 Reflection
> Fathan Naufal Adhitama - 2206825965

1. Try to answer the following questions, and write the answer in the and new file readme.md in 
you repository.  
a. How many data your publisher program will send to the message broker in one run? <br>
Akan ada 5 data yang akan dikirim ke message broker dalam satu kali run. Hal ini dapat dilihat dari banyaknya perintah `_ = p.publish_event("user_created".to_owned(), UserCreatedEventMessage { user_id: "1".to_owned(), user_name: "2206825965-Amir".to_owned() });` yang terdapat pada program<br><br>
b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber 
program, what does it mean? <br>
URL tersebut adalah URL untuk koneksi ke message broker. Apabila URL pada publisher dan subscriber sama, artinya keduanya terhubung ke server yang sama untuk melakukan message exchange. Tujuannya adalah untuk memastikan bahwa message yang dipublish oleh publisher dapat diterima dan diolah oleh subscriber.





