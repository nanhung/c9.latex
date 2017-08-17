# Using LateX in Cloud9

I'm trying to find the free software to replace the MS office. 
Latex seems to be a better choice to do my work. 
Also, I want to use the cloud based IDE and version control system to manage my documents, efficiently. 
Here is my simple way to install and use latex in cloud9.

---

1. In the terminal, update the package list

```
sudo apt-get update 
```

2. Install the TexLive package 

```
sudo apt-get install texlive
```

3. Install thetexlive-latex-extra package 

```
sudo apt-get install texlive-latex-extra
```

4. (Optional) Check all install packages by using following command

```
apt list --installed
```

Here is the total list of the install packages

![Imgur](http://i.imgur.com/82wDFGh.png)


5. Now, create the simple test.tex file to test

```
\documentclass{article} % Define documentclass

\title{Hello \LaTeX{}!} % The article title
\author{My name}        % Your name

\begin{document} 
\maketitle
Hello!                  % The content
\end{document}
```

![Imgur](http://i.imgur.com/nkScMg6.png)

6. Then type following command in the terminal
```
pdflatex test
```

And we can "preview" the pdf file like this
![Imgur](http://i.imgur.com/SI1028c.png)

Also, we can use git to do version control for our documents. (check my [previous post](https://nanhung.github.io/Using-GNU-MCSim-in-web-based-IDE-and-combine-with-version-control/))

That's it! 
Happy texting!