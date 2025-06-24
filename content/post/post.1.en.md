+++
title = 'Fission Product Yields: A Primer on My PhD Thesis'
slug = 'primer-thesis'
image = 'images/pic03.jpg' #I'll have to change this eventually
date = "2019-04-18T00:00:00" #This, too
description = 'Fission Product Yields are at the center of addressing a mystery within nuclear reactors. A mystery with massive implications for new physics, nuclear energy, and national security.'
disableComments = true
+++
Example of post with missing date property but with pic.

![img](/images/favicon.png)

Within a nuclear reactor's core, a series of highly energetic interactions are happening over and over in quick succession. Neutrons fly, strike nuclei, and ignite an exothermic process that can deliver massive quantities of power at scale. This process, nuclear fission, is considered to be self-sustaining through a chain reaction, like dominoes falling. Essentially, when a nucleus fissions, it doesn't split cleanly in half, making two different isotopes, or "fission products." These new isotopes, both the heavier and the lighter one, are generally pretty unstable. For many of these, the most likely path to stability lays in beta decay, wherein they can convert a neutron into a proton by emitting an electron and a tiny, mysterious particle called a neutrino (more on them later). Through beta decay, the previous (parent) isotope becomes a new, ideally more stable (daughter) isotope. Generally, though, it takes a few tries, about three for each original fission product. So you have this chain of new isotopes: parent -> daughter -> granddaughter -> great-granddaughter, where each "->" represents a beta decay. All of these are considered fission products, though. After all, none of them would be there if not for the initial fission. Some of these fission products, are also key to the larger nuclear reaction's functioning. Remember earlier that I mentioned neutrons flying around? Some of these neutrons are released as a part of fission themselves, called prompt neutrons. But some of them, arguably the most important, come from the beta decay chain. Every now and then, you get a fission product that can release a neutron *before* it beta decays. These "delayed" neutrons are the life blood of the nuclear chain reaction. They come in just in time to propagate the reaction just as the prompt neutrons die down. Think of this as a gentle nudge when a domino doesn't immediately topple over in the chain.

So if you were trying to build a nuclear reactor, you might have a vested interest in knowing how often these neutron precursors occur. Knowing that would greatly help you model the behavior of your reactor, and determine how much fuel would be necessary for success. You might also want to know what percentage of your fission products are not precursors. Or you may even want to know what percentage of your fission products are a "neutron poison," isotopes that eat up neutrons thereby slowing the fission process. So for any fission product, you may ask yourself: after one fission, what are the odds that I produce the fission product X? The "odds" in this case are what we call the fission product yield of X!

## Fission Product Yields, National Security, and New Physics

I believe by now the importance of fission product yields (FPYs) in nuclear energy may be clear. However, there's a bit more to the motivations behind studying them. Feel free to skip this if it doesn't sound particularly interesting! I'm just providing more context for why they matter and where the issue we're trying to solve originates.

I promised that I would talk about this later and here we are. There's a character in this story that is often neglected in the telling of nuclear reactors: the neutrino.

The neutrino is a wonderfully mysterious particle. Almost massless, electrically neutral, it eluded physicists for a long time. The important take away about them, though, is that neutrinos tend to pop up after fission happens, since they are a natural byproduct of beta decay. any time you have fission, you will see neutrinos. In fact, you will see a *spectrum* of neutrinos, eseentially different quantities of neutrinos at different energies. This spectrum is unique to the source of the fission process, or rather, to the fuel involved. So these neutrino spectrums can then act as a signature of the fuels within a nuclear reactor. If you had 20% Plutonium-239 and 80% Uranium-235, the signature of your reactor would look like a weighted average of the Plutonium-239 and Uranium-235 signatures. This is a *big* deal. After all, neutrinos are famously impossible to shield. They hardly interact with anything at all, so it's impossible to stop them with any material. 

Importantly, nuclear reactors can be used as a tool for quickly enriching uranium. They can also be used to decommission nuclear warheads. So let's say there's a nuclear nonproliferation treaty between two countries. Let's also say one country already had nuclear warheads and the other was hoping to start a nuclear program. As part of the treaty, one country could use their nuclear reactors to decommission their warheads, while the other promises to never use its reactors to build warheads. Your most sure bet in monitoring these countries is to use neutrino detectors. Since the neutrino signature of a reactor is unique to the fuel composition, unhidable, and abundant, you would be guaranteed that each country is complying with the treaty. But to achieve this you must know the neutrino signatures of nuclear fuels extraordinarily well!

There are major scientific reasons for wanting to know these spectrums well, too. As I mentioned, neutrinos are mysterious. For one thing, they have already broken the standard model of particle physics. This model assumes that neutrinos are massless, like the light particles we call photons. And yet, they have mass! "Neutrinos" is a word that technically refers to three different particles, electron neutrinos, muon neutrinos, and tau neutrinos. Each of these corresponds to a slightly different mass. Incomprehensively, neutrinos are able to "oscillate." That is, if I fire an electron neutrino in your direction, you may not receive an electron neutrino when it arrives, but rather a muon or a tau neutrino. If you fire it back to me, I may then also receive something different from what you sent. How are they able to change their masses like that? How does this "oscillation" even work?

In the 2010s, several neutrino oscillation experiments set out to determine exactly that. The experiments were simple in concept, go to a nuclear reactor, measure the neutrinos you receive at different distances from the reactor. That's it, right? Well, you also have to know what the original amount and composition of these neutrinos looked like. In other words, the neutrino spectrum of the nuclear reactor, that signature from earlier. Well, easy, you just detect the spectrum yourself, compare it to theoretical predictions to make sure things aren't crazy out of alignment, and get going.

But what if when you measure the spectrum and compare it to the theoretical predictions, things *are* out of alignment? And no matter how many times you check, no matter how many different experiments you try, you keep getting the same result? Well, that means the theory is wrong! And it was! In the original models, it turns out the scientists behind them incorrectly estimated the amounts of certain types of fission products (very rare ones, admittedly), and these fission products are then beta decaying and producing some high energy neutrinos that no one was prepared to see!

So to do some pretty high-level, fundamental physics, and to better study the particle with the most potential to show us physics beyond the standard model, you first need to improve your FPY measurements. Not to mention, these FPYs play a significant role in determining the exact signature of different nuclear fuels. So if you want to better monitor nuclear reactors, you also need to have accurate FPYs.

## Solving the Problem

So you need to have accurate FPYs for physics research, you need them for reactor monitoring, and you need them to succesfully build functional, safe nuclear reactors. What's the issue? Don't we already have these? We've built reactors before, right? 

Well, yes. But could those reactors have been more efficient? What about advanced reactors, they may require more accuracy in FPYs as well. One of the key things about FPYs is that *many* of them are calculated theoretically! In particular, the ones that seem to contribute most to the reactor spectrum anomaly are severely lacking in data. And if you want to build successful reactor monitoring models, you're also going to want as much accuracy as possible.

So how do we do this?

You take nuclear fuels, and make them fission. No, I'm serious.

The traditional way to do this takes a long time. You take milligrams of fissile materials, let's say U-235 for simplicity, then you hit it with a neutron beam and then... you wait. You wait long enough that the excessive nuclear radiation fades, and then you can transport your U-235 to a detector where you can take a look at what's in there. In order to not poison yourself or any other radiation worker, you do have to wait a long time, though. Which means that a lot of the short-lived fission products (seconds to minutes) are totally gone. These tend to be the most unstable, so they cause most of the hefty radiation. They also happen to be more likely to be those kinds of isotopes that have FPYs calculated from theoretical approximations, not from data.

So my lab developed a solution. A RApid, Belt-drIven, Target Transport System, or RABITTS (it's a stretch, I know). This thing is basically a conveyor belt that can travel extremely fast and with a ton of precision. So now, we can irradiate a target and almost immediately put it in front of our detectors. We can then use the detectors to figure out how much of each isotope we're looking at. I won't get super into the physics of how this whole thing works, but here's a quick overview. I lied when I said that fission products always beta-decay. Usually, the first thing they do is emit a gamma ray. Then they beta decay. The daughter isotope then also tends to gamma emit, and then beta-decay. So I can use a detector to pick up on the gamma rays coming off of my fissioning U-235. These gamma-rays are essentially unique barcodes. It's extremely rare that two different isotopes should each emit a gamma-ray of the same energy. So I can look at a large range of energy and see different gamma-rays. Then I just have to count the gammas and that tells me how much of each isotope I made. Easy! We also have a fission detector set up behind our U-235 target. It essentially counts the number of fissions there were. With these two things in mind, an FPY is just a ratio: amount of isotope X/number of fissions. Just like that, I have an FPY.

## Conclusion

There's loads of data analysis that goes into this stuff. It's not half as simple as I'm making it sound, to be honest. But my interest here is more in making sure more people understand what my science is! I think treating it simply is the best way to not get lost in the statistical noise of all of it. I do some complex data analysis on some fairly complex nuclear data. But fundamentally that data and analysis tell a bigger story than just "using likelihood maximizing models to determine the quantities and temporal behavior of fission spectral data." So if you skipped all the way down here for a TL;DR, here it is:

Fission product yields are the probability of producing a given isotope from fission or subsequent decay. They play an important role in nuclear energy development and particle physics, and they can one day play a massive role in nuclear monitoring and nonproliferation efforts worldwide. Traditional methods of determining FPYs are severely lacking, so we developed a novel measurement set up. It was a success, but that success brought new challenges to data analysis that did not previously exist. These challenges require novel analytical approaches to better determine these crucial values.

That's all folks.








