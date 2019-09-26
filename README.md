Hi Daniel,

Recently my mind has returned to an old thought.. of how people can extend trust to each other with the exchange of goods/services.

I see the workable system structured as this:

People carry around 'bags' of signed attestations that look like this:
```
    Let A,B be public keys representing two entities.
    M = ((A owes B, N dollars, <timestamp>) signed_by_B) signed_by_A)
```
Eventually, a new attestation is signed (if all goes well):
```
    ((M, resolved, <timestamp>) signed_by_B) signed_by_A)
```
That basic system can exist on its own amongst a "small" community.

As long as I personally know or trust a given public key (say, I know you personally, or there is a large merchant that I frequent).. any stranger who presents a bag of resolved attestations (that are signed by that public key pointing to their public key).. I know a few things:
```
    1. I know how long it took to resolve their "debts".
    2. I know the period of time these interactions occurred during.
```
What do we NOT have to worry about?
```
    1. The initial debts and subsequent resolutions are unique and timestamped.. no one can
     "double assert (spend)" a debt or resolution assertion.
```
How does one get screwed in this system?
```
    1. An unknown comes to me with a big bag of resolved attestations from someone I trust,
     BUT they are only going to show "their good side" (a lake of unresolved debts they've
     been running up all over town is something they prefer not to admit).

    2. Private key (identity) theft:  someone steals my private key and goes on a spending
     spree.. using my good name buying hookers and blow but never intending to resolve the debts.
```
How are these things mitigated?
```
    1. In the least, I can reach out to the public keys that have signed their resolved
     attestations to find out if there are any other signed attestations that they are hiding.
     I can also randomly check with other people I've had trusted interactions with.

    2. For theft, I'm a little screwed.. I'll need a trusted way (in person, a multi-factor
     protected Twitter account) to tell everyone in my circle that my shit was stolen.. give
     them my new public key, and ask them to spread the word warning others.
```
All of these parts deal only with entity to entity interactions.

There are incentives in this system.. that would drive people to want to send big batches of these attestations to some dependable persistence store.
```
    1. Creditors want it known that a bunch of people owe them money.. so other merchants
     can know who may be running up big tabs.

    2. Debtors want it known that they are paying their debts back on time.. even if it isn't
     someone they're directly working with (maybe its just the big merchants who care.. that
     people know Credit/Debt is flowing).
```
I'd suggest they batch them up and broadcast them in Bitcoin transactions.

Then an interaction between two strangers would go like so:
```
    1. We show each other our bags.  (One sees how punctual the other is at "resolving" attestations
     on time.  The other sees that the other is dependable at being satisfied with resolved debts.)

    2. We ask around what other's know about this stranger.

    3. We check the global persistence store.
```
Again, the system doesn't give a fuck how debts are resolved.  If A owes B, no one gives a shit if B resolves the debt due to:
```
    1. Government Currency
    2. Cryptocurrency
    3. Barter
    4. Good Vibes
```
All you have to consider is.. what do I think about the community of people who are cryptographically signing attestations that this stranger is square with them.



Other features:
```
    1. Debt Jubilee == generate a new key pair.. and get back to work establishing yourself as
     a good player, and try not to fuck your shit up this time.

    2. Vouching:

        "A backs B, up to N dollars, expiration_timestamp"
```
etc..  All of the settlement happens outside of the technical system.

What if A refuses to back B when push comes to shove?  That's A's problem.. if they are an established identity.. it behooves them to not overextend themself.. lest people not trust them.

What if a bunch of people you trusted don't make good?  Well.. try to be a little more discerning in who you trust.. OR be more flexible in how you accept payment.

This is just a magnification of normal human interaction.



Also.. nothing restricts what the attestations say.. two interacting parties just need to agree on the particular protocol.


Anyway, your mind moves farther and faster than mine.. so let me know your thoughts.  I see the biggest risk being protecting your private key.. or dealing with it being stolen.  I see that as potentially manageable because.. the TRUE value of your identity is in YOU (it isn't like a savings account).

Someone can steal my private key (or yours), but there is NO WAY IN HELL they can be us [If they could, then we aren't much use as a humans].

We just need to tell the people who know us.. "This is my new fucking key, some dink stole the old one."
