##LAB 5


## Create Local YUM repository on CentOS 7 #

## 1.Create Source: ##
### 1.1 Mount the CD/DVD ROM on the any directory of your wish, for testing mount it on /cdrom. ###

* # mkdir /cdrom 
* # mount /dev/cdrom /cdrom

## 2.Configuration file: ##
### 2.1 Create the new repo file called cdrom.repo under /etc/repos.d directory. ##

* # vi /etc/yum.repos.d/local.repo
![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11902285_806118416175181_6233568462655196513_n.jpg?oh=a3a0b61083b39e043f1b83995d8d34fb&oe=566A3463)
### 2.2 Add the following details. ###

![](https://fbcdn-sphotos-c-a.akamaihd.net/hphotos-ak-xft1/v/t1.0-9/11889432_806118582841831_2404090978941577719_n.jpg?oh=9f7799b5075d13d1aaed9b47e3f64ecc&oe=56761AC1&__gda__=1446653771_768a65e75c61ca374673f9bf8ffa596b)
## 3.Installation: ##
### 3.1 Before installing clear the repository cache by issuing the following command. ###


![](https://fbcdn-sphotos-d-a.akamaihd.net/hphotos-ak-xpt1/v/t1.0-9/11891108_806118549508501_3295868242412009169_n.jpg?oh=69d4c254966e2d086419e66e80e520dd&oe=5672D522&__gda__=1446748198_35316cce8bfec456cd417871c71c0141)

### 3.2 Install the package using the yum command, let’s install the vsftpd package from the local repository. ###


![](https://fbcdn-sphotos-a-a.akamaihd.net/hphotos-ak-xlf1/v/t1.0-9/11951985_806118556175167_2806002091464304348_n.jpg?oh=263838418a2d2c8aeb553ed36025ac85&oe=567825CB&__gda__=1451108532_25509ef2685f83489e7617dbf9d44550)




![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpt1/v/t1.0-9/11222409_806118766175146_3913017548181966489_n.jpg?oh=a6f1892e8f7496683b9f214ed5e61ab2&oe=5639E911)




![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11923616_806118786175144_1613458176350278080_n.jpg?oh=6795d8e97e25f252d02c255fb260c325&oe=567089FC)

# Install OwnCloud 7 on CentOS 7 #

## 1.Prerequisites: ##
### 1.1 it is based on PHP and database combination, database can be any of the above four. So install PHP, Apache web server and MySQL server on CentOS 7. ###


![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11914103_806118739508482_1266274103089505153_n.jpg?oh=d4f595c2782502d903a84ed2c4d76258&oe=566E22B0)




![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11887947_806118872841802_1269801906272980544_n.jpg?oh=3ce7d24e31922cfd23b0ea34b6233767&oe=5675741C)

### 1.2 Set SELinux to allow OwnCloud to write the data. ###



![](https://fbcdn-sphotos-g-a.akamaihd.net/hphotos-ak-xlf1/v/t1.0-9/11953170_806118916175131_2382775379921055029_n.jpg?oh=7fa88c83a0cc0543872365e2add1ab85&oe=567F6E47&__gda__=1450238008_4fd29ecd9153e838d10ed59904d60aae)
### 1.3 Allow apache in firewall. ###




![](https://fbcdn-sphotos-c-a.akamaihd.net/hphotos-ak-xfp1/v/t1.0-9/11900042_806119012841788_9185370686883375601_n.jpg?oh=988571284cfe92e3362d74315e32efe4&oe=566A4FC1&__gda__=1450311240_a8037ad36a6cc523ae70cc6d54a6c663)

### 1.4 Start Apache and MariaDB. ###



![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11880485_806119092841780_3856409984104122171_n.jpg?oh=af00581a5004a34ba22e1ffd3b82af27&oe=5681837C)

### 1.5 Auto start the service at system start-up. ###




![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xtf1/v/t1.0-9/10629848_806119132841776_2073701507223935729_n.jpg?oh=656d60ff0b615ea2c17c81260de8ebc8&oe=5668F8DD)

## 2.Download and Setup: ##
### 2.1 Download ownCloud from official website or enter the fallowing command on terminal. ###


### 2.2 Extract the archive. ###


![](https://fbcdn-sphotos-d-a.akamaihd.net/hphotos-ak-xpf1/v/t1.0-9/11889583_806119389508417_8689046781902882222_n.jpg?oh=f63cae3936f5fb37310484f281528a1e&oe=56389D6C&__gda__=1449529862_abbeac49b71613f24d55f39585ce01fd)







![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11913986_806119412841748_8773187601331277733_n.jpg?oh=b5adfe577f54040033665bcce794704a&oe=567ED599)

### 2.3 Allow the web server to read and write the files on cloud directory. ###



![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11892017_806119356175087_5466025860009396505_n.jpg?oh=78fe6f2b9397dd9f6e3a9d6f8645bd3f&oe=56762E88)




![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xtp1/v/t1.0-9/11947498_806119556175067_8127624608695454968_n.jpg?oh=2a9b338ee3576d313080217032a441fb&oe=567E164A)




![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11885332_806119596175063_8326478995585813781_n.jpg?oh=756c868f4643eeedee7e21644fb4fa3a&oe=5672699D)

## 3.Create Database: ##
### 3.1 If you are setting up a MariaDB for the first time, here is the tutorial on Securing MariaDB.  MariaDB server must be started before creating the database, login to MySQL server. ###

![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11915762_806119606175062_3560734186956330350_n.jpg?oh=8afa6bbd05aea4425bfb6cd0e7a2291a&oe=567EB41B)
### 3.2 Create database called “clouddb” ###
### 3.3 Allow “clouddbuser” to access the “clouddb” database on localhost with predefined password. ###



![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xap1/v/t1.0-9/11949346_806119662841723_234316384189116888_n.jpg?oh=9e78f447177b3231d97c1f87cf0e45a9&oe=567ED793)

## 4.Configure Apache server: ##
### 4.1 While configuring Apache web server, it is recommended that you to enable .htaccess to get a enhanced security features, by default .htaccess is disabled in Apache server. To enable it, open your virtual host file and make AllowOverride is set to All. ###







![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xfl1/v/t1.0-9/11954754_806119799508376_5074842529370724278_n.jpg?oh=27dbde4a6bfaba64d5587d53a6a1e091&oe=566AA694)

* Add the following.

![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11899747_806120002841689_1928204457519798057_n.jpg?oh=4da2de853dab9d42e5eda85a6bb5fde0&oe=5680437D)
### 4.2 Remember to restart all services related to Apache server. ###

![](https://fbcdn-sphotos-h-a.akamaihd.net/hphotos-ak-xfp1/v/t1.0-9/11902452_806120042841685_4229404238293265990_n.jpg?oh=4dfa413ce27375f10566d6d41a3782f7&oe=567AD253&__gda__=1451108826_77dda75111c47e0e9df7047d067ceefb)
## 5.Configure ownCloud: ##

* Open up web browser, point a URL to http://your-ip-address/owncloud ( http://Your-custom-domain). Browser will automatically take you to ownCloud setup page where it must be configured before going to live. Enter admin user name, password, data folder location and database details. You can choose any one of the database from SQLite or MySQL. If you choose SQLite database, you do not require to enter database details. where as MySQL database requires database user, password and data base name.

* Alternately you can download ownCloud client to upload the files.
![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11899743_806120072841682_3837671419808085099_n.jpg?oh=65417b1fbc5bfeffb439f494d4614427&oe=56668E11)

* Alternately you can download ownCloud client to upload the files.
![](https://scontent-sin1-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11904693_806120112841678_4844633882914781596_n.jpg?oh=e84d4cd229b93f47336207a58a3cb654&oe=5637A70C)

