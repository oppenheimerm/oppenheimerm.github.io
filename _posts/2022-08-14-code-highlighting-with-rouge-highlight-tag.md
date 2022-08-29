---
layout: post
description: A banana is an edible fruit – botanically a berry – produced by several kinds of large herbaceous flowering plants in the genus Musa.
tags: python maths fruit banana
---

<div class="post-image">
    <img src="/assets/images/row-elechon-form.jpg" alt="Row elechon form cover photo">
</div>

To make my code snippets more readable i'm using [Rouge](https://github.com/rouge-ruby/rouge)Rouge highlighter,
which is Jekyll's default syntax highlighter.  You only need to run this command to get running:

```gem install kramdown rouge```


To use, just surround your code snipped with ```{% raw %}{% highlight language %}{% endraw %}``` and  ```{% raw %}{% endhighlight %}{% endraw %}```.

*Remembering to replace the languageCode with your code language*.  For more help,  
[have a look here](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers) for the list of 
supported languages.


### Example

```
import numpy as np
np.random.seed(27)
A = np.random.randint(1,10,size = (3,3))
B = np.random.randint(1,10,size = (3,2))
print(f"Matrix A:\n {A}\n")
print(f"Matrix B:\n {B}\n")
```

<p class="post-footer">Thanks for reading! <img src="/assets/images/assets/mo-144x144-white.png" alt="MO"></p>