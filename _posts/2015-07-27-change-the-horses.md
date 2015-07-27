---
layout: post
title: Your class should be a limousine
---
<figure>
  <img src="/images/limo.jpg" style="width:450px;height:300px">
  <figcaption style="color:#aaa">No we are not talking about class limousine, but yes it is good.</figcaption>
</figure>
<p>The master was reminiscing about the days he spent learning <em>The Pragmatic Programmer</em>.There was even more wisdom to be learned from the book, now more than ever.The apprentices were given hardcover copies of the book to posses the wisdom he now possessed.With young age, blunders come fast.Apprentices were gulping it down like it was some pulp fiction novel.Master was agonised over it.Just then an apprentice came for some advice.<p>
<p>He had implemented a code that could possibly fit the description of a spaghetti code(no offense to FSM ofcourse).There were dependencies which were not easy to percieve or understand.The master just concentrated on one specific set of issues.<p>

```ruby
    class Ninja
      def initialize(dressing, katana, shuriken, shoes, height, weight)
        @katana = katana
        @dressing = dressing
        @shuriken = shuriken
        @shoes = shoes
        @height = height
        @weight = weight
      end

      def efficiency
        @height * Weapon.new(katana, shuriken).rating
      end

      def fitness
        14400 - @height * @width
      end
    end

    class Weapon
      def initialize(sword, extra)
        @sword = sword
        @extra = extra
      end

      def rating
        sword_rating * extra_rating
      end

      def sword_rating
        case @sword
          when 'longsword'
            5
          when 'katana'
            9
          when 'indiansword'
            6
          else
            0
        end
      end

      def extra_rating
        case @extra
          when 'shuriken'
            7
          when 'knife'
            4
          when 'musket'
            8
          else
            0
        end
      end
    end
```

There were a lot of hidden dependancies in the code.If the `Weapon` class changed then the `Ninja` class also had to change.A matter of irreversibility, mused the master.Master asked the student to come with him to shrine.They took a normal oxen cart which had wooden wheels.At each of the gutters the apprentice feared the worst.When they reached the shrine, apprentice was left breathless.Master and apprentice came back from the shrine.Master had ordered a limousine this time.While there were still gutters, he did not face any issues.
<figure>
  <img src="/images/oxcart.JPG" style="width:300px;height:400px">
  <figcaption style="color:#aaa">Ox cart which master prefers</figcaption>
</figure>
<p>When they reached the dojo master asked the student about which mode of transport would he prefer next time.Student without hesitating replied `Limousine`.Master smiled and asked him why? Because it was more comfortable.Master asked the student why was it more comfortable? The student replied that it was because of the good tires.Master smiled and said <blockquote>Just like the vehicle's tires prevented the vehicle from depending on road your class must also prevent the external dependancies.Your class should be like the limousine.</blockquote></p>