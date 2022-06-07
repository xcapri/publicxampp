# publicxampp
How to make localhost accessible from another device
- Open XAMPP
- On Apache click Config<br>
![image](https://user-images.githubusercontent.com/43540712/172327548-211d641b-efb4-46e6-ac45-144927b81430.png)
- Then click httpd.conf<br>
![image](https://user-images.githubusercontent.com/43540712/172327791-60908412-1b21-42f1-91af-a0ce15731eb1.png)
- Change ```Listen 80``` to  ```192.168.***.1:80``` and comment ```#Listen 80```. Then Save & close notepad <br>
![image](https://user-images.githubusercontent.com/43540712/172328152-f6b04859-8c38-428a-ae9f-3b2a3e3e5015.png)
- Back to step 3 but click httpd-xampp.conf 
- Search D:/xampp/phpMyAdmin, then edit ```Require local``` to ```Require all granted```. Then Save & close notepad<br>
![image](https://user-images.githubusercontent.com/43540712/172328987-9d33666d-1de8-4905-9faf-c444c5d33dbc.png)
- Next go to Windows defender firewall with advanced security > double click on the one I marked with the number 2 <br>
![image](https://user-images.githubusercontent.com/43540712/172329708-043d746d-b2a4-488d-9c59-1af3fd685130.png)
- Then select **Allow the connection** > Apply > OK > Close <br>
![image](https://user-images.githubusercontent.com/43540712/172330095-acf4f5a8-a326-4255-a974-044947217c8c.png)
- Open XAMPP again start Apache & MYSQL 
- Last Access ip on mobile 

## Refrensi 
- https://stackoverflow.com/questions/5524116/accessing-localhost-xampp-from-another-computer-over-lan-network-how-to
- https://ourcodeworld.com/articles/read/1093/how-to-access-the-htdocs-directory-of-xampp-from-a-computer-or-mobile-device-in-the-same-local-area-network-lan

