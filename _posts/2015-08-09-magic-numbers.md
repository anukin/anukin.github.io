---
layout: post
title: Magic numbers
---
The master was seen petting the dragon.Not an enjoyable work any day as dragons in the Dojo were pretty huge and filled with scales.The apprentice was still practicing the art of better programming.His fist was almost accustomed to the practice models.He was bored and thought that at this time Master Gates had built microsoft.He was nowhere near to that and the Master kept on emphasising the importance of practice.He decided to go to the master.
<p>Master was still petting the dragon.Almost an hour had he spent on petting dragons.This was unusual.There was news of war somewhere south east.One of the masters had ridden a dragon there.The siding had to be done, so there was balance in place.Show of force is a must in a war and sometimes war itself can be avoided with just a show of force.</p>
>The supreme art of war is to subdue the enemy without fighting.

Master was tensed and was confused about what should be taught to the student in logical progression.He decided to consult Oracle.

<figure>
  <img src="/images/oracle.jpg" style="width:300;height:300;" alt="Its time for some magic">
  <figcaption style="color:#ggg;">Ugh the way she says things! you would imagine neo to be the architect.</figcaption>
</figure>

Master smiled as he heard the oracle's remark.The apprentice felt like she was on drugs.There was something definitely wrong with the woman.

The master requested the apprentice to write a code for a book.The student was surprised at this sudden request.It was abrupt and foolish.Even then the student went to the dojo and tried writing the code.After few minutes he came up with code.

{% highlight ruby %}
class Book
  def initialize
    @pages = 100
    @current_page = 0
  end

  def turn_page_forward
    @current_page += 1
  end

  def turn_page_backward
    @current_page -= 1
  end
end
{% endhighlight %}
The master was smiling when he saw the code.He smiled at the fact that Oracle saw this coming.He patted the student and started explaining.

A <i>Magic Number</i> is something which is a constant on which the whole program is in turn dependant.Imagine in the above code instance the pages be 2000 then what would happen? Should it stop or should it continue turning pages? 

Also the class assumes that turning of page happens with 1 page at one time.This could be 3 or 4 or even 100 pages at a time. <i> 1 </i> in this context means nothing.These constructs are popularly called Magic numbers or magic number antipatterns.Avoid using them at all costs.
 
