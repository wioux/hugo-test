---
title: Creating Strong Passwords
date: "2017-01-29T19:20:04-07:00"
---

# Creating Strong Passwords

Because remembering many different passwords is difficult, people often reuse a small number of passwords across many different accounts, sites, and services. Today, users are constantly being asked to come up with new passwords—many people end up reusing the same password dozens or even hundreds of times.

Reusing passwords is an exceptionally bad security practice, because if an attacker gets hold of one password, she will often try using that password on various accounts belonging to the same person. If that person has reused the same password several times, the attacker will be able to access multiple accounts. That means a given password may be only as secure as the least secure service where it's been used.

Avoiding password reuse is a valuable security precaution, but you won't be able to remember all your passwords if each one is different. Fortunately, there are software tools to help with this—a password manager (also called a password safe) is a software application that helps store a large number of passwords safely. This makes it practical to avoid using the same password in multiple contexts. The password manager protects all of your passwords with a single master password (or, ideally a passphrase—see discussion below) so you only have to remember one thing. People who use a password manager no longer actually know the passwords for their different accounts; the password manager can handle the entire process of creating and remembering the passwords for them.

For example, KeePassX is an open source, free password safe that you keep on your desktop. It's important to note that if you're using KeePassX, it will not automatically save changes and additions. This means that if it crashes after you've added some passwords, you can lose them forever. You can change this in the settings.

Using a password manager also helps you choose strong passwords that are hard for an attacker to guess. This is important too; too often computer users choose short, simple passwords that an attacker can easily guess, including "password1," "12345," a birthdate, or a friend's, spouse's, or pet's name. A password manager can help you create and use a random password without pattern or structure—one that won't be guessable. For example, a password manager is able to choose passwords like "vAeJZ!Q3p$Kdkz/CRHzj0v7,” which a human being would be unlikely to remember—or guess. Don't worry; the password manager can remember these for you!

### Syncing Your Passwords Across Multiple Devices
You may use your passwords on more than one device, such as your computer and your smart phone. Many password managers have a password-synchronizing feature built in. When you sync your password file, it will be up to date on all of your devices, so that if you’ve added a new account on your computer, you will still be able to log into it from your phone. Other password managers will offer to store your passwords “in the cloud,” which is to say, they will store your passwords encrypted on a remote server, and when you need them on a laptop or mobile, they will retrieve and decrypt them for you automatically. Password managers that use their own servers to store or help synchronize your passwords are more convenient, but the trade-off is that they are slightly more vulnerable to attack. If you just keep your passwords on your computer, then someone who can take over your computer may be able to get hold of them. If you keep them in the cloud, your attacker may target that also. It's not usually a compromise you need to worry about unless your attacker has legal powers over the password manager company or is known for targeting companies or internet traffic. If you use a cloud service, the password manager company may also know what services you use, when, and where from.

### Choosing Strong Passwords
There are a few passwords that do need to be memorized and that need to be particularly strong: those that ultimately lock your own data with cryptography. That includes, at least, passwords for your device, encryption like full-disk encryption, and the master password for your password manager.

Computers are now fast enough to quickly guess passwords shorter than ten or so characters. That means short passwords of any kind, even totally random ones like nQ\m=8*x or !s7e&nUY or gaG5^bG, are not strong enough for use with encryption today.

There are several ways to create a strong and memorable passphrase; the most straightforward and sure-fire method is Arnold Reinhold's "Diceware."

Reinhold's method involves rolling physical dice to randomly choose several words from a word list; together, these words will form your passphrase. For disk encryption (and password safe), we recommend selecting a minimum of six words.

<aside class="tip">
Try making a password using Reinhold’s “Diceware” method.
</aside>

When you use a password manager, the security of your passwords and your master password is only as strong as the security of the computer where the password manager is installed and used. If your computer or device is compromised and spyware is installed, the spyware can watch you type your master password and could steal the contents of the password safe. So it's still very important to keep your computer and other devices clean of malicious software when using a password manager.

### A Word About “Security Questions”

Be aware of the “security questions” (such as “What is your mother’s maiden name?” or "What was your first pet's name?") that websites use to confirm your identity if you do forget your password. Honest answers to many security questions are publicly discoverable facts that a determined adversary can easily find, and therefore bypass your password entirely. For instance, US vice-presidential candidate Sarah Palin had her Yahoo! account hacked this way. Instead, give fictional answers that, like your password, no one knows but you. For example, if the password question asks you your pet’s name, you may have posted photos to photo sharing sites with captions such as “Here is a photo of my cute cat, Spot!” Instead of using “Spot” as your password recovery answer, you might choose “Rumplestiltskin.” Do not use the same passwords or security question answers for multiple accounts on different websites or services. You should store your fictional answers in your password safe, too.

Think of sites where you’ve used security questions. Consider checking your settings and changing your responses.

<aside class="warning">
Remember to keep a backup of your password safe! If you lose your password safe in a crash (or if you have your devices taken away from you), it may be hard to recover your passwords. Password safe programs will usually have a way to make a separate backup, or you can use your regular backup program.
</aside>

You can usually reset your passwords by asking services to send you a password recovery email to your registered email address. For that reason, you may want to memorize the passphrase to this email account also. If you do that, then you will have a way of resetting passwords without depending on your password safe.

### Multi-factor Authentication and One-time Passwords

Many services and software tools let you use two-factor authentication, also called two-step authentication or two-step login. Here the idea is that in order to log in, you need to be in possession of a certain physical object: usually a mobile phone, but, in some versions, a special device called a security token. Using two-factor authentication ensures that even if your password for the service is hacked or stolen, the thief won't be able to log in unless they also have possession or control of a second device and the special codes that only it can create.

Typically, this means that a thief or hacker would have to control both your laptop and your phone before they have full access to your accounts.

Because this can only be set up with the cooperation of the service operator, there is no way to do this by yourself if you're using a service that doesn't offer it.

Two-factor authentication using a mobile phone can be done in two ways: the service can send you an SMS text message to your phone whenever you try to log in (providing an extra security code that you need to type in), or your phone can run an authenticator application that generates security codes from inside the phone itself. This will help protect your account in situations where an attacker has your password but does not have physical access to your mobile phone.

Some services, such as Google, also allow you to generate a list of one-time passwords, also called single-use passwords. These are meant to be printed or written down on paper and carried with you (although in some cases it might be possible to memorize a small number of them). Each of these passwords works only once, so if one is stolen by spyware when you enter it, the thief won't be able to use it for anything in the future.

If you or your organization run your own communications infrastructure, such as your own e-mail servers, there's freely available software that can be used to enable two-factor authentication for accessing your systems. Ask your systems administrators to look for software offering implementations of the open standard “Time-Based One-Time Passwords” or RFC 6238.

### Threats of Physical Harm or Imprisonment

Finally, understand that there is always one way that attackers can obtain your password: They can directly threaten you with physical harm or detention. If you fear this may be a possibility, consider ways in which you can hide the existence of the data or device you are password-protecting, rather than trust that you will never hand over the password. One possibility is to maintain at least one account that contains largely unimportant information, whose password you can divulge quickly.

If you have good reason to believe that someone may threaten you for your passwords, it's good to make sure your devices are configured so that it won't be obvious that the account you are revealing is not the “real” one. Is your real account shown in your computer's login screen, or automatically displayed when you open a browser? If so, you may need to reconfigure things to make your account less obvious.

In some jurisdictions, such as the United States or Belgium, you may be able to legally challenge a demand for your password. In other jurisdictions, such as the United Kingdom or India, local laws allow the government to demand disclosure. EFF has detailed information for anyone travelling across U.S. borders who wishes to protect their data on their digital devices in our Defending Privacy at the U.S. Border guide.

Please note that intentional destruction of evidence or obstruction of an investigation can be charged as a separate crime, often with very serious consequences. In some cases, this can be easier for the government to prove and allow for more substantial punishments than the alleged crime originally being investigated.