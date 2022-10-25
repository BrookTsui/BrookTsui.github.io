It is a circuitous story. 

At the beginning of March 2022, I emailed Prof. Tsai asking if he intended to enroll a student for the summer research. Unfortunately, he said sorry for having already been mentoring four undergraduates then, but still welcome for physics questions. And we, therefore, have kept in touch since then. 

Initially, **I tried to study his work** about the [unitary bound](https://arxiv.org/abs/2103.13396), which I found interesting since, in undergraduate, we always sloppily assume theories are unitary, taking it for granted. I'm curious about the mechanism and "aftermath" of violating it.  

At the time, I had learned QFT for a semester, covering part-I of Peskin, but the question they discussed in the paper is the lepton physics and the Stueckelberg limit, neither of which are familiar to me. It took time to understand and was the beginning of my neutrino journey. 

I collated my thought and confusion in an email and sent it to Prof. Tsai. I waited in the anxiety of being criticized as naive or stupid. Surprisingly, he answered me with patience, kindness, and clearness. Since then, we have talked about physics several times. During this time, I learned about electroweak theory and neutrino physics. 

---

One day, I **came to the paper about the generalized uncertainty principle** [(GUP)](https://arxiv.org/abs/gr-qc/9904026), whose motivation is that the uncertainty principle should be, at least phenomenologically, corrected for quantum gravity. At first glance, I thought the new formula could produce negative temperature for BHs, hence poring it in interest. Although the imagination is wrong, I still found something there: the way of correcting it not satisfies my taste. The meaningful physics argument may also lead to another extrapolation, which seems more, I would say, simple and elegant. And it can produce the same result as before. 

I sent it to Prof. Tsai, and although we then discussed it some times, we finally did not elaborate on it since GUP has essentially some traits hard to explain. 

I don't know if I will back to it in the future, but I still like it. What is good physics? What is good taste? I have no idea. Ever heard a story that a physicist of not-so-good taste will measure and study the falling of pears once he saw an apple falling. A good-taste one, in contrast, will ask why does it fall?  

---

Such a question-and-answer exchange lasted for several months, and one day in July, Prof. Tsai asked me whether I was interested in the Hawking emission, and **he found a problem maybe we can collaborate on**. I said yes readily since having long been curious about the detail of Hawking radiation. The Page-curve always befuddled me.

The energy of photons coming from the decay of scalars, like axions and pions emitted from PBHs lies in the scope of detection of current experiments. By it, we hope to demarcate the abundance of PBHs, hence the bound on the possibility of the being DM. However, the **widely used code**, [BlackHawk](https://blackhawk.hepforge.org/), for particle physicists to produce Hawking radiation suits for massless particles, which **not suits our proposal**. Asides, some works indeed discuss massive particles from BHs but are scattered miscellaneously in various aspects with various notions, the energy scope and the target problems of interest are different, and, most importantly, they do not post the code. 

Therefore, firstly, I **should write a new code** to produce the emission spectra for massive particles. We hope to not only achieve our academic goals but also **make a systematic and comprehensive work to proffer** particle physicists studying BHs a **handy reference**. 

I read the papers of [Unruh](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.3251) and [Page](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.16.2402). They both showed **analytical derivation for low-energy cases**. Such work partly affirmed my thought that the BH area is essentially the cross-section: $\sigma$ of all massless particles equals BH area on a low energy scale, which is a universal conclusion. 

However, for massive particles, the cross-section blows up. It seems strange to me initially. Days later, I found a satisfactory explanation from the Penrose diagram from which one can see all massive particles eventually coalesce with BHs. 

To deepen the understanding, **I also read [Hawking's original paper](https://link.springer.com/article/10.1007/BF02345020) and [Guth's famous note](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.870)**. It is always astonishing to know that Hawking derived the emission from physics guess. These papers corrected my naive understanding of quantum fields in curved spacetime and Hawking radiation. In my first research of BH thermodynamics, I did learn Hawking radiation, but to me, it seems to originate merely from the coordinate change and the Bogoliubov transformation. With the knowledge of QFT and QM, this time it appears much more sophisticated. 

After research, I found Carolina's [paper](https://arxiv.org/abs/1404.0687) showing clear diagrams of massive scalars (in a limit region) in RN BHs, which then became our standard of cross-checking. 

What I learned during that month was **included in the [report](../files/hawkingppt.pdf)** I gave to Prof. Tsai and the postdoc Tao.  

---

Then the calculation. With the redefinition of variables, the radial equation of fields in BH spacetime is tantamount to the Shrodinger equation with an equivalent potential. However, I'm **not familiar with numerical methods**, so after research, I **tried to write the iterative functions** like the Numerov or Runge-Kutta method by the Nest function of MMA from scratch.  

It cost me a whole week. The formula works barely but requires an insane amount of time. Seeing my frustration, Prof. Tsai suggested trying a comparatively straightforward way of using the **NDSolve of MMA**. It works but **not very precise**. 

After several days, I realized the **boundary condition** applied makes the function stiff. Amending it yields the same result as Carolina. 

I used to classify myself as a somewhat old-school physicist, enjoying deriving formulas brutally by hand, spotting key points with unaided eyes, and avoiding using numerical tools as possible. 

The successful derivation of the emission spectra changed the mindset. In hindsight, I was too conservative and narrow-minded. Many chances eluded away. When I was typing this text, AI had mightly seduced hundreds of thousands of Hubbard equations into FOUR ! ([the report from Simons Foundation](https://www.simonsfoundation.org/2022/09/26/artificial-intelligence-reduces-a-100000-equation-quantum-physics-problem-to-only-four-equations/)) I would say, WOW. 

**Another issue** came when I input the **extreme parameters**, like the mass of PBHs and scalars, into the code. It seems to go beyond the precision limit of MMA. I tried several ways to increase the accuracy, but nothing else than making the code slower. At the moment, I believed numerical methods are hopeless and began to search for possible ways of analytical derivation. I came to the [paper of Parsides](https://aip.scitation.org/doi/abs/10.1063/1.1666431?journalCode=jmp), which used several **ODE tools**, including Wroskian and Frobenius method, to discuss field equations in curved spacetime **in a semi-analytical way**. I made a report about such an informative viewpoint. Nonetheless, the semi-analytical method can do little more than restrict the relationship between parameters, and the function is still unsolvable. I also thought of relapsing to the explicit Numerov or Runge-Kutta method then. 

But two days later, staring at the equation, I suddenly realized by **redefinition of parameters**, such extreme parameters go away, and the formula becomes even neater. 

Here are some examples of the spectra for [massive](../files/massive.pdf) and [massless](../files/massless.pdf) particles. 

To be continued. 

---