# Bound

This is curcuitous story. 

At the beginning of March 2022, I sent an email to Prof. Tsai asking if he intended to enroll a student for the summer research. He rejected it since there had already been four students in his lab. But he was welcome for my physical questions. And we, therefore, have kept in touch. 

Initially, I just tried to follow [his work about the unitary bound](../files/ubound.pdf), which I found interesting since I used to take it as granted. Meanwhile, I have consulted him many times the questions about the electroweak theory. During this period, I also sent him my idea about the GUP, although we did not elaborate on it since there are some peculiar traits hard to justify. 

The question-and-answer exchange lasted for several months, and the collaboration began in July. 

The energy of photons coming from the decay of scalars, like axions, emitted from PBHs lies in the scope of detection of current experiments, and in this way we hope to bound the aboundance of PBHs, hence the bound on the possibility of the being DM. The crux is the calculation of the massive scalars spectra of PBHs for the whole energy-scale, which is oblivious in the traditional context of particle physics. There are some analytical works for the low-energy limit; the conventional code, [BlackHawk](https://blackhawk.hepforge.org/), for producing Hawking radiation is designated for massless particles; and the rare complete works showing the complete spcetra are scattered miscallaneously in several areas on different aspects with various notions. 

We hope to not only to set the bound on PBHs but also make a systematic and comprehensive work integrating these, offering the particle physics shpere a handy reference. 

First, the Hawking emission, which I have learned a lot in the first research but overlooked the detailed calculation of the rate. (I usually feel confused about the Page curve, wondering how to evaluate the vaporating time.)

I first read two papers by [Unruh](../files/Unruh.pdf) and [Page](../files/Page.pdf) for a basic picture. Their analytical derivation is both on the low-energy scale. Although Unruh discussed the massive scalars in Schwarzschild spacetime, but he did not plot the whole diagram covering the region of interest. 

After research, I found a [paper](../files/carolina.pdf) talking about the complete spectra of massive scalars in RN BHs, which then became our basis of studying. 

To develop a through understanding of the subject, I have read [Hawking's original paper](../files/Haw75.pdf) and [Guth's famous note](../files/Guth76.pdf). They corrected my naive understanding about Hawking radiation that it originates merely from the coordinate transformation and Bogoliubov transformation. 

All I have learned was included in the [report](../files/hawkingppt.pdf) I gave to Prof. Tsai and the postdoc Tao in the meeting. 

When the prepartion was done, I began the calculation by numerical methods. The basic method is the partial wave decomposition and equivalent-potential trick. This has been a challanging and interesting task since I am not proficient at MMA or other numerical tools. In the half month, I have read through a textbook about MMA. Eventually, by NDSolve with the help of the document, the circuitous road leads me to the right spectra.

To be continued. 

---