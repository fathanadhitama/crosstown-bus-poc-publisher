# Tutorial 8 Reflection
> Fathan Naufal Adhitama - 2206825965

1. Try to answer the following questions, and write the answer in the and new file readme.md in 
you repository.  
a. How many data your publisher program will send to the message broker in one run? <br>
Akan ada 5 data yang akan dikirim ke message broker dalam satu kali run. Hal ini dapat dilihat dari banyaknya perintah `_ = p.publish_event("user_created".to_owned(), UserCreatedEventMessage { user_id: "1".to_owned(), user_name: "2206825965-Amir".to_owned() });` yang terdapat pada program<br><br>
b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber 
program, what does it mean? <br>
URL tersebut adalah URL untuk koneksi ke message broker. Apabila URL pada publisher dan subscriber sama, artinya keduanya terhubung ke server yang sama untuk melakukan message exchange. Tujuannya adalah untuk memastikan bahwa message yang dipublish oleh publisher dapat diterima dan diolah oleh subscriber.

2. Running RabbitMQ as message broker.
 ![rabbitmq.jpg](img/rabbitmq.jpg)

3. Sending and processing event
 ![subscriber.png](img/subscriber.png)
  ![publisher.png](img/publisher.png)
  > Kedua gambar tersebut adalah yang terjadi ketika saya melakukan perintah `cargo run` pada subscriber dan publisher. Yang terjadi adalah publisher mengirim 5 event kepada message broker yang kemudian event tersebut akan diterima dan diproses oleh publisher ditandai dengan output output tersebut pada gambar pertama.







