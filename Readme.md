# Description 
## Data yang harus dimassukkan
Username
Password
E-mail
Birthday
Proffesion

Controller yg ada pada package ini di desain  untuk menghandle request URL/Register
@request mapping(value="/register")

Disini kita menggunakan 2 cara yaitu view Registration dan process Registration untuk menggunakan GET dan POST request masing masing cara ini
merupakan cara yang flexible karena kita bebas memilih nama dan parameter yang dinginkan.
## ViewRegistration()
disini kita menggunakan userForm sebagai model
###### User userForm = new User();
###### model.put("userForm", userForm);
Cara ini akan menghasilkan View name 'Registration' yang akan dihasilkan pada screenshot dibawah ini
## Process Registration
##### ModelAttribute("userForm") User user
Ini akan membuat objek yang disimpan pada model userForm dapat dipanggil kembali ,karena
spring akan otomatis binds hasil dari registratsi pada model dan dapat di print dengan
###### System.out.println("username: " + user.getUsername());
Code di atas akan mengeprint data yang disimpan dalam proess registrasi 

## Screenshot
![Scan/Photo of Sketches](https://github.com/DennasTrue/Tugas-MVc/blob/master/Spring%20MVC%20Form%20Registration%20Test%20-%20Success%20Page.png)
![Scan/Photo of Sketches](https://github.com/DennasTrue/Tugas-MVc/blob/master/Spring%20MVC%20Form%20Registration%20Test.png)




