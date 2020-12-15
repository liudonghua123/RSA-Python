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

![image](https://user-images.githubusercontent.com/7680591/59566357-3a722d00-902d-11e9-991c-b67e5f369722.png)

And this is what a code says….
![rsa](https://user-images.githubusercontent.com/7680591/59566011-0e07e200-9028-11e9-9f54-449d0ff23a28.jpg)

Note that you may have to setup an external dependency environment in some cases, it would create a big chunk of files that are not here due to exceeding the maximum number of files to upload.
