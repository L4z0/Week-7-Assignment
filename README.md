# Week-7-Assignment

* For finding the XSS exploit, I used wpscan and used the reference: http://klikki.fi/adv/wordpress2.html. From there I read the overview of the stored XSS adn how an unauthenticated attacker can inject JavaScript in WordPress comment. On the Proof of concept the injection command was provided along with a nice short demo on how to execute the command.

![lab 7 - xss](https://user-images.githubusercontent.com/36518965/41494170-80eb577c-70c4-11e8-8739-72c6bf591f70.gif)


* For the Username Numeration exploit, since it is obvious that anything that is input in the username/password box and it displays some message verifying the information, in this example all I did was show that by typing an incorrect username and password and taking note of the message, followed by an a correct username and wrong password, I was able to show that there was a vulnerability.

![username enumeration](https://user-images.githubusercontent.com/36518965/41494346-e0c15ea6-70c6-11e8-9ecc-e33025131df8.gif)


* For the sql injection, the one that wpscan provides is called a "potential sql injection" which I guess it can be a potential injection if the admin accidentally approves of the injectoin. For this one I had to pull the code from https://github.com/WordPress/WordPress/commit/70128fe7605cb963a46815cf91b0a5934f70eff5 and use the [wp-include/post.php] code. 

![potential sql injection](https://user-images.githubusercontent.com/36518965/41495808-d39845d2-70e4-11e8-91df-6dd60805e3ac.gif)
