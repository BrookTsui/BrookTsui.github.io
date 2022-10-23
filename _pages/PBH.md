This is curcuitous story. 

At the beginning of March 2022, I sent an email to Prof. Tsai asking if he intended to enroll a student for the summer research. Unfortunately, he said sorry for having already been mentoring four undergraduates then, but still welcome for physics questions. And we, therefore, have kept in touch since then. 

Initially, I tried to study his work about the [unitary bound](https://arxiv.org/abs/2103.13396), which I found interesting since in the undergraduate study we always simply assume theories are unitary, taking it as granted. I'm curious about what is the mechanism and "aftermath" of violating it.  

At the time, I had learned QFT for a semaster, covering part-I of Peskin, but the question they discussed in the paper is the lepton physics and the Stueckelberg limit, neither of which are familiar for me. It took 



consulted him many times the questions about the electroweak theory. During this period, I also sent him my idea about the GUP, although we did not elaborate on it since there are some peculiar traits hard to justify. 

The question-and-answer exchange lasted for several months, and the collaboration began in July. 

The energy of photons coming from the decay of scalars, like axions, emitted from PBHs lies in the scope of detection of current experiments, and in this way we hope to bound the aboundance of PBHs, hence the bound on the possibility of the being DM. The crux is the calculation of the massive scalars spectra of PBHs for the whole energy-scale, which is oblivious in the traditional context of particle physics. There are some analytical works for the low-energy limit; the conventional code, [BlackHawk](https://blackhawk.hepforge.org/), for producing Hawking radiation is designated for massless particles; and the rare complete works showing the complete spcetra are scattered miscallaneously in several areas on different aspects with various notions. 

We hope to not only to set the bound on PBHs but also make a systematic and comprehensive work integrating these, offering the particle physics shpere a handy reference. 

First, the Hawking emission, which I have learned a lot in the first research but overlooked the detailed calculation of the rate. (I usually feel confused about the Page curve, wondering how to evaluate the vaporating time.)

I first read two papers by [Unruh](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.3251) and [Page](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.16.2402) for a basic picture. Their analytical derivation is both on the low-energy scale. Although Unruh discussed the massive scalars in Schwarzschild spacetime, but he did not plot the whole diagram covering the region of interest. 

After research, I found carolina [paper](https://arxiv.org/abs/1404.0687) talking about the complete spectra of massive scalars in RN BHs, which then became our basis of studying. 

To develop a through understanding of the subject, I have read [Hawking's original paper](https://link.springer.com/article/10.1007/BF02345020) and [Guth's famous note](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.870). They corrected my naive understanding about Hawking radiation that it originates merely from the coordinate transformation and Bogoliubov transformation. 

All I have learned was included in the [report](../files/hawkingppt.pdf) I gave to Prof. Tsai and the postdoc Tao in the meeting. 

When the prepartion was done, I began the calculation by numerical methods. The basic method is the partial wave decomposition and equivalent-potential trick. This has been a challanging and interesting task since I am not proficient at MMA or other numerical tools. In the half month, I have read through a textbook about MMA. Eventually, by NDSolve with the help of the document, the circuitous road leads me to the right spectra.

To be continued. 

---