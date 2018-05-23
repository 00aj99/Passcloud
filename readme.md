# What is Passcloud?

For most people, passwords are a real problem. Remembering passwords is a pain and using the same password everywhere will eventually lead to disaster. While traditional password managers attempt to solve this with randomized passwords they sacrifice your security by saving your passwords to a database.

**This makes your passwords vulnerable to interception and hacks!**

Passcloud deals with this problem by _never storing your passwords_. Instead, Passcloud generates repeatable pseudo-random passwords based on the [Mersenne Twister PRNG algorithm](http://www.math.sci.hiroshima-u.ac.jp/~m-mat/MT/emt.html). Passcloud uses this stateless algorithm to free you from the danger of storing your passwords, as long as you can remember the same repeatable information you will always get the same unique password. It's amazing, really.

## Nothing to Hack

With Passcloud there is no risk of hacking since it uses client-side JavaScript and your passwords are never saved. Contrary to other password solutions, Passcloud doesn't need to send your passwords over the network to make them ubiquitously available. Since Passcloud generates your passwords based on your repeatable information, you don't have any fragile dependencies. Just remember your repeatable information on any device and your passwords will be available instantly. By default Passcloud doesn't rely on a cloud server, doesn't rely on syncing backups, and there is no data connection. _Unless you choose to use the convenient sync feature_ your information is never backed up or synchronized between devices.

## Convenience of Sync

Sometimes security must be sacrificed for convenience, this is why Passcloud has an optional and unique sync system. Even with the sync feature enabled Passcloud remains one of the most clever and secure password managers available on the market. 

Passcloud only stores your repeatable information used to generate your passwords and never your passwords, master password, or your sync key. Your repeatable information is uniquely anonymized and encrypted using a huge key derived from your master password and sync key based on the AES256 protocol. Using this over the top methodology you can rest easy knowing your data, even if breached, can _never be used to expose you to any risk_. Without knowing your sync key and your master password, your data is inaccessible, indecipherable, and unusable. **There is simply no way to extract useful information.**

### What data is stored?

Only the following repeatable information is stored:
- Site name
- User profile
- Length of the password 
- Seed number
- Password type
- If the password uses alpha numerics
- If the password is removes ambiguous characters
- If the password uses special characters
- If the password uses extended characters
- If the password uses only unique characters
- If the password changes yearly
- The year the password was created 

## For Any Purpose

Passcloud comes with a variety of built-in password types. These types make the user's password look different, become more secure or more compatible with a site's password policy.
Passcloud also implements a solution that allows you to save custom information in the app.

By using Passcloud for every site you visit you're less vulnerable to security breaches, even if one password is compromised all of your other passwords generated by Passcloud remains secure!

## Licensing Information

Passcloud is free software (GPLv3), its algorithm, dependencies, and code have been extensively documented for nearly 10 years. You can view the code for Passcloud yourself over at it's [GitHub](https://github.com/spencerthayer/Passcloud) page, where you are able to provide feedback, submit issues, or even contribute to the code yourself! 

Development testing, which means it's likely broken, can be found at https://passcld.herokuapp.com.

### Run Your Own Passcloud

Passcloud was made to with strict security culture in mind. As such you shouldn't implicitly trust Passcloud. The Passcloud creator encourages users to deploy their own versions of Passcloud to their own servers. Security starts with taking responsibility so just click the button below to begin.

 [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/spencerthayer/Passcloud)

### Version Information

- v2.0.3 - General fixes.
- v2.0.2 - Updates to the Material CSS interface.