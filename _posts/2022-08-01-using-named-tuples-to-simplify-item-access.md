---
layout: post
description: using named tuples to simplfy item access in python.
tags: python
---

Here we'll look at using named tuples to simplfy item access in python.

Let's continue looking at items in recipes.  The regular expression for parsing the string had three attributes:

1.  ingredient 
2.  amount
3.  unit

We used the following pattern with names for the various substrings::


<pre><code class="language-python">
#   rename image to that of the post slug
#   https://stackoverflow.com/questions/51570254/django-change-name-of-image-from-imagefield
def rename_image(instance, filename):
    filebase, extension = filename.split('.')
    return 'images/%s.%s' % (instance.slug, extension)

class PublishedManager(models.Manager):
    def get_queryset(self):
        return super(PublishedManager, self).get_queryset().filter(status='published')
</code></pre>

The resulting data tuple looked like this:

<pre><code class="language-python">
>>> item = match.groups()
('Kumquat', '2', 'cups')
</code></pre>

While the matching between *ingredient, amount,* and *unit* is pretty clear, using something like the following isn't ideal.  What does  **"1"** mean?  Is it really the quantity?


<pre><code class="language-python">
>>>Fraction(item[1])
Fraction(2, 1)
</code></pre>

We want to define tuples with names, as well as positions

<pre><code class="language-plaintext">
Just some plain old text here
</code></pre>

<p class="post-footer">Thanks for reading! <img src="/assets/images/assets/mo-144x144-white.png" alt="MO"></p>