This is curcuitous story. 

At the beginning of March 2022, I sent an email to Prof. Tsai asking if he intended to enroll a student for the summer research. Unfortunately, he said sorry for having already been mentoring four undergraduates then, but still welcome for physics questions. And we, therefore, have kept in touch since then. 

Initially, I tried to study his work about the [unitary bound](https://arxiv.org/abs/2103.13396), which I found interesting since in the undergraduate study we always simply assume theories are unitary, taking it as granted. I'm curious about what is the mechanism and "aftermath" of violating it.  

At the time, I had learned QFT for a semaster, covering part-I of Peskin, but the question they discussed in the paper is the lepton physics and the Stueckelberg limit, neither of which are familiar for me. It took times to understand them, which is the beginning of my neutrino journey. 

I collated my thought and confusion in an email and send it to Prof. Tsai waiting for being criticized naive or stupid. Surpresingly, he answered in patience, kindness, and clearness. Since then, we have talked about physics several times, and the conversation is mainly that I asked him and he answered me. During this period, I learned a lot about the electroweak theory and neutrino physics. 

---

One day, I came to the paper named "generalized uncertainty principle," whose motivation is that the uncertainty principle should be, at least phenomelogically, corrected for quantum gravity. At first glance, I thought the new formula could produce negative temperature for BHs, therefore I pored it in interest. Although the imagination is wrong, I still found something I can do: I was not satisfied about the way of correcting it, the physics argument is meaningful, however, it may also lead us to another way of extrapolation, which seems more, I would say, elegant and simple. And it can produce the same result as before. 

I sent it to Prof. Tsai, although we then discussed it several times, but we did not elaborate on it, since GUP has essentially some traits hard to explain. 

I don't know if I will back to it future, but I still like it. What is the good physics? What is the good taste? I have no idea. So far, I have been roaming in the giant realm of physics, and interrogating with nature. I ever heared a story saying that the physicist of a bad taste will measure and study the falling of pears when he saw an apple falling down, a good taste, in contrast, will lead him to ask, why does an apple fall down?  

---

Back to the story. Such question-and-answer exchange lasted for several months, and on one day of July, Prof. Tsai asked me whether I interest in Hawking emssion, and he had found a problem maybe we can collaborate. I said yes since I have long been curious about the detail of Hawking radiation. The Page-curve befuddled me when I saw it first time. 

The energy of photons coming from the decay of scalars, like axions and pions emitted from PBHs lies in the scope of detection of current experiments, and in this way we hope to demarcate the aboundance of PBHs, hence the bound on the possibility of the being DM. However, the widely used, [BlackHawk](https://blackhawk.hepforge.org/), for particle physicists to produce Hawking radiation is designated for massless particles, which not suits our proposal. Asides, some works indeed discuss massive particles from BHs, but they are scattered miscallaneously in various aspects with various notions, and the energy scope and the target problems of interest are different, and, most importantly, they do not post the code. 

Therefore, firstly, I should write a new code to produce the emission spectra for massive particles. We hope to not only to acheive our academic goals but also make a systematic and comprehensive work to proffer particle physicists studying BHs a handy reference. 

I read the papers of [Unruh](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.3251) and [Page](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.16.2402) for a basic picture. They both showed analytical derivation for low-energy scale. Such work partly affirmed my thought that the BH area is essentially the cross section given the cross section of all massless particles equals BH area in low energy scale. However, for massive particles, the cross section blows up. It befuddled me initially. Days later, I found a satisfactory explaination from Penrose diagram from which one can see all massive particles eventually colaseace with BHs. 

To deepen the understanding, I also read [Hawking's original paper](https://link.springer.com/article/10.1007/BF02345020) and [Guth's famous note](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.870). It is always astonishing to know that Hawking derived the emission from physics guess. These papers corrected my naive understanding about quantum fields in curved spacetime and Hawking radiation. In my first research of BH thermodynamics, I did learn Hawking radiation, but at the time I thought it originates merely from the coordinate transformation and Bogoliubov transformation. This time, especially 

After research, I found carolina [paper](https://arxiv.org/abs/1404.0687) talking about the complete spectra of massive scalars in RN BHs, which then became our basis of studying. 

All I have learned was included in the [report](../files/hawkingppt.pdf) I gave to Prof. Tsai and the postdoc Tao in the meeting. 

When the prepartion was done, I began the calculation by numerical methods. The basic method is the partial wave decomposition and equivalent-potential trick. This has been a challanging and interesting task since I am not proficient at MMA or other numerical tools. In the half month, I have read through a textbook about MMA. Eventually, by NDSolve with the help of the document, the circuitous road leads me to the right spectra.





To be continued. 

---