# RSA-Python
The RSA algorithm coded in Python

Created in collaboration with [Unnikrishnan Menon](https://github.com/7enTropy7)

**RSA Algorithm**
* Pick two large primes <a href="https://shlappas.com/github-math/#p,q" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=p,q" title="p,q" /></a>
* Compute <a href="https://shlappas.com/github-math/#n=pq" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=n=pq" title="n=pq" /></a> and <a href="https://shlappas.com/github-math/#\phi(n)=(p-1)(q-1)" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=\phi(n)=(p-1)(q-1)" title="\phi(n)=(p-1)(q-1)" /></a>
* Choose a public key <a href="https://shlappas.com/github-math/#e" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=e" title="e" /></a> such that <a href="https://shlappas.com/github-math/#1<e<\phi(n)" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=1<e<\phi(n)" title="1<e<\phi(n)" /></a> and <a href="https://shlappas.com/github-math/#\text{gcd}(e,\phi(n))=1" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=\text{gcd}(e,\phi(n))=1" title="\text{gcd}(e,\phi(n))=1" /></a>
* Calculate <a href="https://shlappas.com/github-math/#d" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=d" title="d" /></a> such that <a href="https://shlappas.com/github-math/#de\equiv1\mod%20\phi(n)" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=de\equiv1\mod%20\phi(n)" title="de\equiv1\mod \phi(n)" /></a>
* Let the message **key** be <a href="https://shlappas.com/github-math/#m" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=m" title="m" /></a>
* **Encrypt:** <a href="https://shlappas.com/github-math/#c\equiv%20m^e\mod%20n" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=c\equiv%20m^e\mod%20n" title="c\equiv m^e\mod n" /></a>
* **Decrypt:** <a href="https://shlappas.com/github-math/#m\equiv%20c^d\mod%20n" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=m\equiv%20c^d\mod%20n" title="m\equiv c^d\mod n" /></a>

| Message | H| e | l | l | o |
| --- | --- | --- | --- | --- | --- |
| ASCII Code | 72 | 101 | 108 | 108 | 111 |
| <a href="https://shlappas.com/github-math/#p%3D11%2C%20q%3D13" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=p%3D11%2C%20q%3D13" title="p,q" /><br/><a href="https://shlappas.com/github-math/#n%3D143" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=n%3D143" title="n" /><br/><a href="https://shlappas.com/github-math/#\phi(n)%3D120" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=\phi(n)%3D120" title="\phi(n)" /><br/><a href="https://shlappas.com/github-math/#e%3D77" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=e%3D77" title="e" /><br/><a href="https://shlappas.com/github-math/#d%3D53" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=d%3D53" title="d" /> | | | | | |
| **Encrypt:** <a href="https://shlappas.com/github-math/#c\equiv%20m^e\mod%20n" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=c\equiv%20m^e\mod%20n" title="c\equiv m^e\mod n" /> | 63 | 95 | 114 | 114 | 89 |
| **Decrypt:** <a href="https://shlappas.com/github-math/#m\equiv%20c^d\mod%20n" target="_blank"><img src="https://render.githubusercontent.com/render/math?math=m\equiv%20c^d\mod%20n" title="m\equiv c^d\mod n" /> | 72 | 101 | 108 | 108 | 111 |
| Decrypted Message | H | e | l | l | o |

And this is what a code says….

```shell
> python RSA_Python.py
Enter bit_length: 4
Running RSA...
Generating public/private keypair...
353 137
Public Key:  (9651, 48361)
Private Key:  (32123, 48361)        
Write msg: Hello
[72, 101, 108, 108, 111] 
Encrypted msg:
3048825169461814618124754
Decrypted msg:
Hello
```

Note that you may have to setup an external dependency environment in some cases, it would create a big chunk of files that are not here due to exceeding the maximum number of files to upload.
