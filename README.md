Dr. Chuck's Web Components Experiment
=====================================

This is a place where I will develop code to figure out how I want to use
web components in my own development.  
I see the future of web applications as increasingly web components based.
I see web components and JSON APIs as a great coding pattern regardless of your
front-end approach and back-end approach.

If web components are truly ready
for the "big time" they should work in static HTML and you should be able
to view source and understand what is going on.

You can see my playground at https://www.dr-chuck.com/wc-experiment/

It is simple, static, and crude.  I will add more sample code over time as I learn more
about the way *I* want to use web components.
I don't want to adopt a framework - I want to use browser functionality as it comes from the browser.
In a way all I see all of the front end and back end frameworks as doing research in how web components
need to function and informed the design and development of web component 
implentation in modern browsers.  So that is a good thing.

But I do not want to develop code to any framework.   I want to develop a pattern that can work with 
PHP, JQuery, and Bootstrap 3 or Java and Velocity.   I support far too much code that cannot afford 
to rewrite itelf completely every time a framework development team sneezes.

How I want to go about this
---------------------------

* I want it all in the markup

* It is OK to download a static asset from a CDN - like a polyfill for older browsers - this needs
to be pretty static - if it did not change for a year things won't break

* I am OK with extending *one* thing like LitElement or HTMLElement - as long as that code is 
so old and boring that it is in maintenance mode and will only issue new releases if something
in browsers breaks it.  (kind of like JQuery).

* I could tolerate a simple templating library that is old and rusty and not
changing much anymore like Handlbars.   Cool, hip, recent and getting better rapidly are
all negative aspects of any framework

JQuery is mature enough for me - but I want to move to vanilla JavaScript becaue JQuery did its job
and fixed vanilla JavaScript.

No Thanks
---------

Many interested in web components are advocates of one or more "crutch" technologies that to me
are fine ways to "prototype" web applications but not a good way to build a web application that
needs to last 5-10 years without major rewrite.  If you are a VC-funded startup - you are trashing and 
rewriting your code constantly - I can't afford to waste that kind of money on my software.  So I avoid
quick "feel-good" solutions.

* Please don't suggest that I use React or any other client side framework. Backbone and Angular 1
are probably mature enough for me - but that only makes my point.

* Please don't suggest that I use Polymer, Node, or any other slick way to "manufacture" web components.
If we are still at the point where it is *impossible* to do web components without these
"helper" technolgoes - I will wait.

* No npm, bower, or other component manager - eventually I might be willing to so some kind of
server side packaging / path patching to make a large number of web components easier to maintain
and more efficient to download.  But for my experiments, I want to see simple solutions that
you see and fully understand when you "view source" in a browser.

* Please don't suggest I use your webcomponent library like PatternFly. Patternfly 3 was
markup or React based based - PatternFly 4 is React based - because they got lazy.  I don't
want to depend on a framework builder remaining aligned with my philosophy over time.
I don't want a framework I adopt to force me to do a complete rewrite on their schedule.

* Please don't suggest I use a CSS library like Material Design - the approach should
work with any markup themeing.   It won't surprise you that I like Bootstrap 3 and think
Bootstrap 4 is a complete waste of time.

* Please don't suggest I rewrite everything in Ruby on Rails and use HAML.  I am 
similarly disinclined to use Scala or Rust.  The server side should not matter.

* Don't mention GraphQL or Apollo - the markup should be data store agnostic.

* Even though I like PHP - don't tell me to use Laravel and Blade - they are dang impressive but they
need write access to the htdocs folder to work because they compile their templates for performance.
Giving the Apache process write access to the htdocs folder - what could go wrong?

* I am not interested in the *amazing* web components you already have. I am sure you have the worlds
most impressive button.  I already have buttons.  I use Bootstrap 3 to style them.  
I want to make my higher-order own extendible web
components with a focus on those adopting my approach to be able to extend my web components
to add their own flavor.  I am guessing that your component library is a bunch of brittle spaghetti code
that you update furiously and in non-upwards compatible ways every time a new browser is released.

If it is not possible to build web components without resorting to these approaches - I will just
keep waiting.  But I am actually quite confident that web components are mature enough for
me to adopt and use in long-lived applications.


