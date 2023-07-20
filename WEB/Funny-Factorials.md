Web/Funny-Factorials

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/3cc50354-3666-4985-806e-19140bd2800e)

Let go ahead and download the python code given before visiting the website.

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/6d8c0552-7388-4fb3-9617-99e7cb186422)

By analysing the python code thoroughly we can see that ```../``` has been filter which means the challenge is probably LFI. 
Let check out the URL given.

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/a6581124-1455-4a4a-a7ae-aac5744ac52e)

Since we know the parameter as theme which is shown in the pyton code or you can decided to click the available themes in the webserver.

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/30fcf246-1a63-43ea-a4f8-2203bbd57030)

Since the server remove every / so I decided to make it double so let check source code. 

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/ecde4a8b-0089-446f-a573-d9731e92188d)

Cool let go ahead and read the content of our flag by trying //flag.txt.

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/f571e93a-f50c-4dea-a109-db39178848f3)

Flag: amateursCTF{h1tt1ng_th3_r3curs10n_l1mt_1s_1mp0ssibl3}

