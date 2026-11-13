---
layout: post
title: "J01: Getting Past the WiFi Login Page"
---
I visited my girlfriend for the weekend, who goes to UC Davis, there she lives in an apartment complex which is privately owned and is exclusively for students and staff. I needed to complete and turn in assignments due at 11:59 that night, and since I got there later (around 9PM), I was scrambling towards starting since I had no idea how long they would take. 

I've used WiFi with a login page numerous times at hotels, airports, and coffee shops. Usually, a page pops up instantly, I agree on some terms, says I'm connected, the page closes, and I'm online in about 30 seconds. But with their network, my girlfriend told me I needed to log in with her username and password, which seemed simple enough. 

Opening the WiFi list, there were multiple networks with a bunch being private networks from other units, plus 2 or 3 that had the apartment complex's name with extra words, like "Temp" and "West Village WiFi".

<img    src="{{ '/assets/wifi-list.png' | relative_url }}" 
        alt="WiFi List" 
        width="190"
        style="display: block; margin: 0 auto;">

It wasn't clear which one I was suppose to join and use, so I picked the one with just the complex's name (Sol at West Village), since that seemed like that main network. 

The login page didn't pop up on its down and didn't fully show up until I opened my browser. When it finally did, it was a basic page asking for a username and password.

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap; wrap; margin-bottom: 20px;">
    <img src="{{ '/assets/login-page.png' | relative_url }}"
        alt="Log In Page"
        width="400">
    <img src="{{ '/assets/invalid.png' | relative_url }}"
        alt="Invalid Creds"
        width="400">
</div>


I typed in her info and got an "Invalid Credentials". We double checked every input and made sure that it was exactly correct. Without changing anything, I just pressed Enter again, and it magically and eventually went through. That's a problem with **feedback**, which is how a system responds to what you do so you know whether it worked. When the same input is "wrong" one second and "right" the next, the feedback isn't telling you anything useful. We wasted time doubting her log in information when it was correct the whole time.

Next, I got a welcome page with a big header that said "Login Successful". 

<img    src="{{ '/assets/success.png' | relative_url }}" 
        alt="Connected" 
        width="475"
        style="display: block; margin: 0 auto;">

Based on my **mental model**, the popup should've closed itself at this point. But it didn't, it just fully stayed opened. The only way I could close it was hitting the "Cancel" button, but clicking it asked whether I wanted to use a different network instead. 

<img    src="{{ '/assets/other-net.png' | relative_url }}" 
        alt="Other Network" 
        width="375"
        style="display: block; margin: 0 auto;">

I started to feel worried at this point. I couldn't leave the pop up without making a choice I didn't want to make. This goes against **user control and freedom**, the idea that users should always have a clear way to exit or undo something without consequences. 

When I finally got it to close, the WiFi icon indicated that I was connected and online, but nothing would load. My laptop kept switching between "Connected" and "No Internet Connection". 

<img    src="{{ '/assets/not-connected.png' | relative_url }}" 
        alt="Not Connected" 
        width="375"
        style="display: block; margin: 0 auto;">

This is a problem with **visibility of system status**, the idea that a system should always let you know what's actually and currently going on. Between the welcome page and the WiFi icon, I was told I was connected two different ways, and neither were true. 

Additionally, the login page also had a surprising amount of information that an average user wouldn't need or want to know. Things like data usage, connected devices, and addresses were all over the page. All I wanted was to get online, instead, all the extra stuff just made the page harder to make sense of. 

<img    src="{{ '/assets/dashboard.png' | relative_url }}" 
        alt="Dashboard" 
        width="550"
        style="display: block; margin: 0 auto;">

For the next 30 to 40 minutes, my girlfriend and I troubleshooted and tried everything we could think of. We forgot the network and rejoined it, and restarted and fully shutdown my laptop multiple times. Here, I went from confused to frustrated to ready to pull my hair out. Then, at some point, it just worked. I still don't know what we did that fixed it but I was relieved. I lost alot of time I needed for my assignments that could've been prevented with a simpler process.  

To be fair, once I was connected and actually online, the WiFi speed was pretty fast. The login page itself was also simple, with just two fields (username and password). The problems were everything around it.

If I could change this process I would:
- Add a guest login option so visitors don't need to borrow a resident's username and password. Which would make it easier for both the guests and residents, as well as safer for residents in regards to sharing their credentials. 
- Make the login page pop up right away when you join the network, without needed to open a browser. 
- Close the pop up automatically once you're connected, or at least give a clear "Done" button that doesn't redirect you towards another network.
- Label the networks clearly so its obvious which one to join.
- Keep the login page focused on LOGGING IN, and move usage and device details somewhere else.

All I needed was to sign in and get to work on my assignments. Each of these implementations and changes would remove a step where I got stuck, and when fully working together could have turned 40 minutes into about 1. 