# **Skynet portal migration guide**

As you probably already heard, Skynet Labs is shutting down and with it also its portals, siasky.net, skynetfree.net and skynetpro.net. This means that if you were using them and want to keep your data online you should migrate them before those data disappear.

## **Skynet lives, only Skynet Labs shut down?**

That's correct. There are two completely different things, Skynet Labs and Skynet. 

Skynet Labs is a developer behind Skynet. Even when the company is no longer active, its licenses and work continues living.

Skynet is the technology that Skynet Labs created and also used for own portal operations and user base. The technology is open-source and permission-less so anyone agreeing with its license can use it.

## **What happens to my data if I do nothing?**

Skynet portals store data at Sia hosts they form storage contracts with. Your data are safe until the contracts expire (Skynet portals usually form them for 2 months). Normally a portal keeps renewing those contracts so your data stay pinned (pinning is like saying "I want to pay for these data staying online") but when a portal goes down the data are no longer pinned which means that contracts won't be renewed and some time later the Sia hosts remove your content as they are no longer paid to keep it.

## **How can I preserve my data?**

Thanks to the nature of truly decentralized technologies like Sia and Skynet, the decision is yours. If such shutdown happened to a centralized storage provider, your data would be lost permanently but this time you some multiple options.

### **1) Migrate to [web3portal.com](https://web3portal.com) (aka Lume)**
- web3portal is your next best portal to go. It's **community oriented** and the Lume project recently received a grant from Sia Foundation so you can expect a lot more for people seeking decentralized internet.
- if you want to use this portal you **need an account**. That's because accounts are the only thing effectively reducing amount of abuse reports as the abusers prefer to stay completely anonymous. But since "accounts" are basically just an email + password, no fair user should have issue with that. Accounts are needed by the portals so they know which data are important to you and should stay pinned. If you wish to learn more about why this is important and why portals allowing anonymous uploads are impossible to operate long term, check this article from Skynet Labs about [scope of censorship on the internet](https://blog.sia.tech/the-worrying-depth-and-scope-of-censorship-on-the-internet-ffd4bc5a5486).
- keep in mind that web3portal offers only **10 GB for free** users (Skynet Labs offered 100 GB) so if you're storing more data make sure to look into the paid tiers
- once ready to migrate to web3portal [you can use this tool](https://github.com/SkynetLabs/webportal-skylinks-migration).

### **2) Set up your own portal**
- main advantage is that you are your own master, you decide if to use it only personaly, for a closed community (friends, family or even bigger communities) or publicly.
- main disadvantage is that you need to run it yourself which means your time and resources.
- learn more about running a web portal [here](https://support.skynetlabs.com/the-technology/running-a-web-portal)

And that's it. Further instructions are meant only for site operators or if you still have doubts and need more assistance.

## **I'm site operator storing content on Skynet but it doesn't work.**

That's because there are few extra steps. Without those users without account cannot download the content.

1) Register on [web3portal](https://web3portal.com) and get sponsor key following this [guide](https://docs.skynetlabs.com/skynet-topics/portal-accounts/api-and-sponsor-keys). These keys allow others to download specific files on Skynet through a portal that only allows traffic from account holders.
2. Setup `DNS` in your domain hosting setting. See the `Using Sponsor Keys` section in the guide above.
3. It should start working pretty quickly (CF is nearly instant for example). If not, wait a bit and then make sure your setting is correct.

## **I still need some help.**

If you need general help with the migration, best way is to ask directly in `#help` channel on [Skynet discord](https://discord.gg/skynetlabs).

If you need more `DNS` and Lume specific help, join [Lume discord](https://discord.gg/nVWC8jMepz).
