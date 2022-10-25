This is curcuitous story. 

At the beginning of March 2022, I sent an email to Prof. Tsai asking if he intended to enroll a student for the summer research. Unfortunately, he said sorry for having already been mentoring four undergraduates then, but still welcome for physics questions. And we, therefore, have kept in touch since then. 

Initially, **I tried to study his work** about the [unitary bound](https://arxiv.org/abs/2103.13396), which I found interesting since in the undergraduate study we always simply assume theories are unitary, taking it as granted. I'm curious about what is the mechanism and "aftermath" of violating it.  

At the time, I had learned QFT for a semaster, covering part-I of Peskin, but the question they discussed in the paper is the lepton physics and the Stueckelberg limit, neither of which are familiar for me. It took times to understand them, which is the beginning of my neutrino journey. 

I collated my thought and confusion in an email and send it to Prof. Tsai waiting for being criticized naive or stupid. Surpresingly, he answered in patience, kindness, and clearness. Since then, we have talked about physics several times, and the conversation is mainly that I asked him and he answered me. During this period, I learned a lot about the electroweak theory and neutrino physics. 

---

One day, I **came to the paper about the generalized uncertainty principle** [(GUP)](https://arxiv.org/abs/gr-qc/9904026), whose motivation is that the uncertainty principle should be, at least phenomelogically, corrected for quantum gravity. At first glance, I thought the new formula could produce negative temperature for BHs, therefore I pored it in interest. Although the imagination is wrong, I still found something I can do: I was not satisfied about the way of correcting it, the physics argument is meaningful, however, it may also lead us to another way of extrapolation, which seems more, I would say, elegant and simple. And it can produce the same result as before. 

I sent it to Prof. Tsai, although we then discussed it several times, but we did not elaborate on it, since GUP has essentially some traits hard to explain. 

I don't know if I will back to it future, but I still like it. What is the good physics? What is the good taste? I have no idea. So far, I have been roaming in the giant realm of physics, and interrogating with nature. I ever heared a story saying that the physicist of a bad taste will measure and study the falling of pears when he saw an apple falling down, a good taste, in contrast, will lead him to ask, why does an apple fall down?  

---

Back to the story. Such question-and-answer exchange lasted for several months, and on one day of July, Prof. Tsai asked me whether I interest in Hawking emssion, and **he found a problem maybe we can collaborate on**. I said yes since I have long been curious about the detail of Hawking radiation. The Page-curve befuddled me when I saw it first time. 

The energy of photons coming from the decay of scalars, like axions and pions emitted from PBHs lies in the scope of detection of current experiments, and in this way we hope to demarcate the aboundance of PBHs, hence the bound on the possibility of the being DM. However, the **widely used code**, [BlackHawk](https://blackhawk.hepforge.org/), for particle physicists to produce Hawking radiation is designated for massless particles, which **not suits our proposal**. Asides, some works indeed discuss massive particles from BHs, but they are scattered miscallaneously in various aspects with various notions, and the energy scope and the target problems of interest are different, and, most importantly, they do not post the code. 

Therefore, firstly, I **should write a new code** to produce the emission spectra for massive particles. We hope to not only to acheive our academic goals but also **make a systematic and comprehensive work to proffer** particle physicists studying BHs a **handy reference**. 

I read the papers of [Unruh](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.3251) and [Page](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.16.2402) for a basic picture. They both showed **analytical derivation for low-energy case**. Such work partly affirmed my thought that the BH area is essentially the cross section given the cross section of all massless particles equals BH area in low energy scale. However, for massive particles, the cross section blows up. It befuddled me initially. Days later, I found a satisfactory explaination from Penrose diagram from which one can see all massive particles eventually colaseace with BHs. 

To deepen the understanding, **I also read [Hawking's original paper](https://link.springer.com/article/10.1007/BF02345020) and [Guth's famous note](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.870)**. It is always astonishing to know that Hawking derived the emission from physics guess. These papers corrected my naive understanding about quantum fields in curved spacetime and Hawking radiation. In my first research of BH thermodynamics, I did learn Hawking radiation, but at the time I thought it originates merely from the coordinate transformation and Bogoliubov transformation. 

After research, I found carolina [paper](https://arxiv.org/abs/1404.0687) showing nice diagrams of massive scalars in RN BHs, which then became our standard of cross-checking. 

What I have learned in that month was **included in the [report](../files/hawkingppt.pdf)** I gave to Prof. Tsai and the postdoc Tao.  

---

Then the calculation. With redefinition of variables, radial equation of fields in BH spacetime is little more complicated than Shrodinger equation with an equivalent potential. However, I'm **not familiar with numerical methods**, so after research, I **tried to write the iterative functions** like Numerov or Runge-Kutta formula by the Nest function of MMA from scratch.  

It costed me a whole week. The formula works, but generally requires an insane amount of time. Seeing my frustration, Prof. Tsai suggested me to try a rather strightforward and simple way that to use the **NDSolve of MMA**. It works, but **not very precise**. 

After several days, I realized it is the **bounday condition** used that makes the function stiff. Amending it yields the right result as same as Carolina. 

I used to classify me as a somewhat old-school physicist, enjoying deriving formula brutally by my hands, spotting key points by unaided eyes, and aviod using numerical tools as possible as I can. The successful derivation of the emission spectra which I really interest in changes the mindset. In hindsight, I was too conservative and narrow-minded. Many chances eluded away. When I was typing this text, AI had mightly seduced hundards of thousands of Hubberd equations into FOUR !([the report from Simons foundation](https://www.simonsfoundation.org/2022/09/26/artificial-intelligence-reduces-a-100000-equation-quantum-physics-problem-to-only-four-equations/)) I would say, WOW. 

**Another issue** came when I input the **extreme parameters**, like the mass of PBHs and scalars, into the code. It seems to go beyond the precision limit of MMA. I tried several ways to increase the accuracy, but nothing else than making the code slower happens. At the moment, I believed numerical methods are hopeless and began to search for possible ways of analytical derivation. I came to the [paper of Parsides](https://aip.scitation.org/doi/abs/10.1063/1.1666431?journalCode=jmp), which used several **ODE tools**, including Wroskian and Frobenius method, to discuss field equations in curved spacetime **in semi-analytical way**. It is informative, and I made a report then. Nonetheless, in semi-analytical way I can do little more than restricting the relationship between parameters and the function is still unsolvable. I also thought of relapsing to explicit Numerov or Runge-Kutta method then. 

But two days later, staring at the equation, I suddenly realized by **redefinition of parameters**, such extreme parameters go away and the formula become even more neat. 

Here are some examples of the spectra for [massive](../files/massive.pdf) and [massless](../files/massless.pdf) particles. 

To be continued. 

---