<!--
Add here global page variables to use throughout your
website.
The website_* must be defined for the RSS to work
-->

@def website_title = "My blog"
@def website_descr = "雑記"
@def website_url = "https://sasuseso.github.io/"

@def author = "sasuseso"

@def mintoclevel = 2

<!--
Add here files or directories that should be ignored by Franklin, otherwise
these files might be copied and, if markdown, processed by Franklin which
you might not want. Indicate directories by ending the name with a `/`.
-->

@def ignore = ["node_modules/", "franklin", "franklin.pub"]

<!--
Add here global latex commands to use throughout your
pages. It can be math commands but does not need to be.
For instance:
* \newcommand{\phrase}{This is a long phrase to copy.}
-->

\newcommand{\R}{\mathbb R}
\newcommand{\scal}[1]{\langle #1 \rangle}
\newcommand{\definition}[2]{
@@definition
\label{#1}
**Definition**: (_!#1_)\\
#2
@@
}

\newcommand{\theorem}[3]{
@@theorem
\label{#1}
**Theorem**: (_!#1_)\\
#2
~~~<details>~~~
~~~<summary>~~~
**Proof**
~~~</summary>~~~
#3
~~~</details>~~~
@@
}
