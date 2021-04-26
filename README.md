# simple-file-base-muti-user-authentication

---

此程式主要展示基於認證文件的多用戶認證流程，靈感是源自於Linux的使用者認證。（用於資安研究）



## Features

---

+ Create New User after Checking

  ![image](https://github.com/yuuR-Meow/simple-file-base-muti-user-authentication/blob/main/sample_image/1.createUser.gif)

+ Deny Toleration （3 times per application exercution）

  ![image](https://github.com/yuuR-Meow/simple-file-base-muti-user-authentication/blob/main/sample_image/2.deny.gif)

+ Time for Password Expiration（３minutes default）

  ![image](https://github.com/yuuR-Meow/simple-file-base-muti-user-authentication/blob/main/sample_image/3.login.gif)

+ Repeat-Login and Warning

  ![image](https://github.com/yuuR-Meow/simple-file-base-muti-user-authentication/blob/main/sample_image/4.relogin.gif)

+ Input Password Without Display

  ![image](https://github.com/yuuR-Meow/simple-file-base-muti-user-authentication/blob/main/sample_image/5.hiddenPW.png)



## How to store user date?

---

+ Field In File	"user_auth.dat"：

  username：password：lastChange：expired：lastLogin：connection

  *（Actually, symbol '：' is halfwidth in file.）

+ Password Hash：

  We choose SHA3-512 as our hash algorithm to hash user password. Then, encode the hash result to hexadecimal encoding.



## Main Test Platform

---

+ Microsoft Terminal（Windows）
+ Bash （Ubuntu）

## Author

---

yuuR-Meow	a.k.a.	JunWei Liao

## License

---

Baic MIT licence. 