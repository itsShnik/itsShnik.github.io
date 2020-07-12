---
layout: default
permalink: /
---
<br>

{% include landing.html %}





## **About Me**

Hi I'm Nikhil Shah. I am a third-year undergraduate student of the Department of Computer Science and Engineering, IIT Kharagpur. <br> 
I have really enjoyed my stay at IIT Kharagpur. I am fond of photography (specially Sunsets!) and I often click anything new that I see. In my free time I like to play basketball (contact me for a 1-on-1). Unlike most I do not like to watch movies and TV shows leave apart a few. I'll rather go for a long walk or just sleep or maybe write something (and throw that in trash very soon).<br>

I love to spend time on solving problems, playing kids games on mobile and throwing ball here and there. 

<br>
<br>
<br>
<br>
<br>


<div class="row">
{% include about/timeline.html title="Experience" source=site.data.education-timeline %}
</div >
*details of projects can be found* [here](projects/)

<br>
<br>
### Curated Projects      

{% include projects/index.html %}
{% include elements/button.html link="projects/" text="Read More " block=true %}
###### You can check out the other things I do [here](Random/)



<br>
<br>
<br>




<div style="text-align: center;font-size:180%;">
<b> Lets have a chat :mailbox_with_mail:</b>
</div>

<div style="text-align: center;font-size:140%;">
  {% if site.ajaxify_contact_form %}
  <br>
  <br>
    <form class="form-stacked">
      <label>
        Email
        <input type="text" name="email" class="field-light" placeholder="{{ site.text.contact.email | default: "Email Address" }}">
      </label>
        <br>
    
      <label>
        Content
        <textarea type="text" name="content" rows="5" placeholder="{{ site.text.contact.content | default: "What would you like to say?" }}" style="resize: vertical"></textarea>
      </label>
    
      <input type="text" name="_gotcha" style="display:none" />
    
      <button type='submit' class="button button-blue button-big mobile-block">{{ site.text.contact.submit | default: "Say Hello" }}</button>
    </form>
  {% else %}
    <form action="https://formspree.io/myynpjpw" method="POST" class="form-stacked">
      <label >
        Email
        <br>
        <input type="text" name="email" style="field-light" placeholder="{{ site.text.contact.email | default: "Email Address" }}">
      </label>
      <br>
      <label>
        Content
        <br>
        <textarea type="text" name="content" class="field-light" rows="5" placeholder="{{ site.text.contact.content | default: "What would you like to say?" }}" style="resize: vertical"></textarea>
      </label>
    
      <input type="hidden" name="_next" value="{{ site.baseurl }}/thanks/" />
      <input type="hidden" name="_subject" value="{{ site.text.contact.subject | default: "New submission!" }}" />
      <input type="text" name="_gotcha" style="display:none" />
      <br>
      <input type="submit" class="button button-blue button-big mobile-block" value="{{ site.text.contact.submit | default: "Say Hello" }}">
    </form>
  {% endif %}

 {% if site.ajaxify_contact_form %}
  {% include ajaxify_content_form.html %}
{% endif %}

</div>

<br>
<br>
<div align="center" style="font-size: 80%">
	<i>shnikisme@gmail.com</i><br>
	<i>+91 8094219905</i>
</div>

