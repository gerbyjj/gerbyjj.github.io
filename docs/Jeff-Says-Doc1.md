---
layout: default
title: Jeff Says
nav_order: 20
languages: ["en","client2"]
---

# This is a one hashtag markup

  <div class="post">
    <div align="right">
      Translate: 
      <!-- Adds links to other languages on the post -->
      {% for lang in page.languages %}
        {% unless site.lang == lang %}
          {% if lang == site.default_lang and site.default_locale_in_subfolder != true %}
            <a href="{{ site.baseurl_root }}{{ page.url }}" >{% t langs.{{ lang }} %}</a>
          {% else %}
            <a href="{{ site.baseurl_root }}/{{ lang }}{{ page.url }}" >{% t langs.{{ lang }} %}</a>
          {% endif %}
          
          {% assign next = forloop.index | plus: 1 %}
          
          {% if forloop.last != true and page.languages[forloop.index] != site.lang or page.languages[forloop.index] == site.lang and next < forloop.length %}
            <span class="separator"> &bull; </span>
          {% endif %}
          
        {% endunless %}
      {% endfor %}
    </div>
  </div>

This page has only two translations

## This is a two hashtag markup

Jaguar shark! So tell me - does it really exist? I was part of something special. They're using our own satellites against us. And the clock is ticking. You know what? It is beets. I've crashed into a beet truck. Yes, Yes, without the oops! Eventually, you do plan to have dinosaurs on your dinosaur tour, right?

Remind me to thank John for a lovely weekend. Forget the fat lady! You're obsessed with the fat lady! Drive us out of here! Is this my espresso machine? Wh-what is-h-how did you get my espresso machine? God help us, we're in the hands of engineers. Jaguar shark! So tell me - does it really exist?

### This is a three hashtag markup

Did he just throw my cat out of the window? So you two dig up, dig up dinosaurs? You know what? It is beets. I've crashed into a beet truck. I gave it a cold? I gave it a virus. A computer virus. So you two dig up, dig up dinosaurs? We gotta burn the rain forest, dump toxic waste, pollute the air, and rip up the OZONE! 'Cause maybe if we screw up this planet enough, they won't want it anymore!

