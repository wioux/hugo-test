---
title: Communicating with Others
date: "2017-02-01T19:20:04-07:00"
---

# Communicating with Others

Telecommunication networks and the Internet have made communicating with people easier than ever, but have also made surveillance more prevalent than it has ever been in human history. Without taking extra steps to protect your privacy, every phone call, text message, email, instant message, voice over IP (VoIP) call, video chat, and social media message may be vulnerable to eavesdroppers.

Often the safest way to communicate with others is in person, without computers or phones being involved at all. Because this isn’t always possible, the next best thing is to use end-to-end encryption while communicating over a network if you need to protect the content of your communications.

### How Does End-to-End Encryption Work?

When two people want to communicate securely (for example, Akiko and Boris) they must each generate crypto keys. Before Akiko sends a message to Boris she encrypts it to Boris's key so that only Boris can decrypt it. Then she sends the already-encrypted message across the Internet. If anyone is eavesdropping on Akiko and Boris—even if they have access to the service that Akiko is using to send this message (such as her email account)—they will only see the encrypted data and will be unable read the message. When Boris receives it, he must use his key to decrypt it into a readable message.

End-to-end encryption involves some effort, but it's the only way that users can verify the security of their communications without having to trust the platform that they're both using. Some services, such as Skype, have claimed to offer end-to-end encryption when it appears that they actually don't. For end-to-end encryption to be secure, users must be able to verify that the crypto key they're encrypting messages to belongs to the people they believe they do. If communications software doesn't have this ability built-in, then any encryption that it might be using can be intercepted by the service provider itself, for instance if a government compels it to.

You can read Freedom of the Press Foundation's whitepaper, Encryption Works for detailed instructions on using end-to-end encryption to protect instant messages and email. Be sure to check out the following SSD modules as well:

 * An Introduction to Public Key Cryptography and PGP
 * How to: Use OTR for Windows
 * How to: Use OTR for Mac

### Voice Calls
When you make a call from a landline or a mobile phone, your call is not end-to-end encrypted. If you're using a mobile phone, your call may be (weakly) encrypted between your handset and the cell phone towers. However as your conversation travels through the phone network, it's vulnerable to interception by your phone company and, by extension, any governments or organizations that have power over your phone company. The easiest way to ensure you have end-to-end encryption on voice conversations is to use VoIP instead.

<aside class="warning">
Beware! Most popular VoIP providers, such as Skype and Google Hangouts, offer transport encryption so that eavesdroppers cannot listen in, but the providers themselves are still potentially able to listen in. Depending on your threat model, this may or may not be a problem.
</aside>

Some services that offer end-to-end encrypted VoIP calls include:

 * WhatsApp
 * Signal
 * Jitsi 
 * Silent Phone
 * Zphone

In order to have end-to-end encrypted VoIP conversations, both parties must be using the same (or compatible) software.

### Text Messages

Standard text (SMS) messages do not offer end-to-end encryption. If you want to send encrypted messages on your phone, consider using encrypted instant messaging software instead of text messages.

Some end-to-end encrypted instant messaging services use their own protocol. So, for instance, users of Signal on Android and iOS can chat securely with others who use those programs. ChatSecure is a mobile app that encrypts conversations with OTR on any network that uses XMPP, which means you can choose from a range of independent instant messaging services.

### Instant Messages
Off-the-Record (OTR) is an end-to-end encryption protocol for real-time text conversations that can be used on top of a variety of services.

Some tools that incorporate OTR with instant messaging include:

 * Pidgin (for Windows or Linux)
 * Adium (for OS X)
 * ChatSecure (for iPhone and Android)
 * Jitsi (Linux, Windows, Mac OS)

### Email

Most email providers give you a way of accessing your email using a web browser, such as Firefox or Chrome. Of these providers, most of them provide support for HTTPS, or transport-layer encryption. You can tell that your email provider supports HTTPS if you log in to your webmail and the URL at the top of your browser begins with the letters HTTPS instead of HTTP (for example: https://mail.google.com).

If your email provider supports HTTPS, but does not do so by default, try replacing HTTP with HTTPS in the URL and refresh the page. If you’d like to make sure that you are always using HTTPS on sites where it is available, download the HTTPS Everywhere browser add-on for Firefox or Chrome.

Some webmail providers that use HTTPS by default include:

 * Gmail
 * Riseup
 * Yahoo

Some webmail providers that give you the option of choosing to use HTTPS by default by selecting it in your settings. The most popular service that still does this is Hotmail.

What does transport-layer encryption do and why might you need it? HTTPS, also referred to as SSL or TLS, encrypts your communications so that it cannot be read by other people on your network. This can include the other people using the same Wi-Fi in an airport or at a café, the other people at your office or school, the administrators at your ISP, malicious hackers, governments, or law enforcement officials. Communications sent over your web browser, including the web pages that you visit and the content of your emails, blog posts, and messages, using HTTP rather than HTTPS are trivial for an attacker to intercept and read.

HTTPS is the most basic level of encryption for your web browsing that we recommend for everybody. It is as basic as putting on your seat belt when you drive.

But there are some things that HTTPS does not do. When you send email using HTTPS, your email provider still gets an unencrypted copy of your communication. Governments and law enforcement may be able to access this data with a warrant. In the United States, most email providers have a policy that says they will tell you when you have received a government request for your user data as long as they are legally allowed to do so, but these policies are strictly voluntary, and in many cases providers are legally prevented from informing their users of requests for data. Some email providers, such as Google, Yahoo, and Microsoft, publish transparency reports, detailing the number of government requests for user data they receive, which countries make the requests, and how often the company has complied by turning over data.

<aside class="tip">
If your threat model includes a government or law enforcement, or you have some other reason for wanting to make sure that your email provider is not able to turn over the contents of your email communications to a third party, you may want to consider using end-to-end encryption for your email communications.
</aside>

PGP (or Pretty Good Privacy) is the standard for end-to-end encryption of your email. Used correctly, it offers very strong protections for your communications. For detailed instructions on how to install and use PGP encryption for your email, see:

 * How to: Use PGP for Mac OS X
 * How to: Use PGP for Windows
 * How to: Use PGP for Linux

### What End-To-End Encryption Does Not Do

End-to-end encryption only protects the content of your communication, not the fact of the communication itself. It does not protect your metadata—which is everything else, including the subject line of your email, or who you are communicating with and when.

<aside class="warning">
Metadata can provide extremely revealing information about you even when the content of your communication remains secret.
</aside>

Metadata about your phone calls can give away some very intimate and sensitive information. For example:

 * They know you rang a phone sex service at 2:24 am and spoke for 18 minutes, but they don't know what you talked about.
 * They know you called the suicide prevention hotline from the Golden Gate Bridge, but the topic of the call remains a secret.
 * They know you spoke with an HIV testing service, then your doctor, then your health insurance company in the same hour, but they don't know what was discussed.
 * They know you received a call from the local NRA office while it was having a campaign against gun legislation, and then called your senators and congressional representatives immediately after, but the content of those calls remains safe from government intrusion.
 * They know you called a gynecologist, spoke for a half hour, and then called the local Planned Parenthood's number later that day, but nobody knows what you spoke about.

 If you are calling from a cell phone, information about your location is metadata. In 2009, Green Party politician Malte Spitz sued Deutsche Telekom to force them to hand over six months of Spitz’s phone data, which he made available to a German newspaper. The resulting visualization showed a detailed history of Spitz’s movements.

Protecting your metadata will require you to use other tools, such as Tor, at the same time as end-to-end encryption.

For an example of how Tor and HTTPS work together to protect the contents of your communications and your metadata from a variety of potential attackers, you may wish to take a look at this explanation.