# Phase 1
Our original argument is that if one considers the horizon radius $r$ as the position uncertainty of the singularity, there must be an energy uncertainty $\Delta E\sim \frac{1}{r}$, hence $E \Delta E\sim 1$ given $E\sim r$. One thus may consider the BH energy spectra as a band rather than a line. The appearance of the upper bound usually implies the possibility of negative temperature, hence the project. 

At that time, I was oblivious of the meaning of doing background research, and was more used to reading textbooks than looking up papers. Therefore I did not think about the correctness of the topic or whether it had been discussed. 

After studying BH physics and quantum mechanics, I **realized it was wrong**. The point is that $r$ is actually the maximum position uncertainty, and then $\Delta E$ is the minimum uncertainty. The energy spectra are exactly the complement of the so-called band. No upper bound. 

But still, I **decided to continue** the research because I found it a fascinating thermodynamical concept. We generally believe that $\frac{\partial E}{\partial S}>0$ is true for BHs, but out of the pure formal symmetry, there is **no reason to not discuss the opposite**. 

---
# Phase 2
Firstly, I **studied the regular negative temperature systems**, including the population inversion in Laser and nuclear-spin systems. Their common feature, the symmetrical configuration of the highest energy and the lowest energy, led me to **propose a general and simplified model** for negative temperature. 

It is the energy-bounded and number-limited quantum S. H. O. For example, N oscillators huddling in $E=0$ state or $E=E_{max}$ state both have zero entropy, and then a smooth transition must yield a fraction with $\frac{\partial E}{\partial S}<0$. 


Quantifying the entropy requires the restricted integer partition function. At the time, my understanding of number theory is very naive that the partition function of integer should be a precise formula whose outputs are rigorously integers. Therefore I did a partition of few dozen integers, and then drawed various diagrams to find the pattern. And also tried to studied it from a general perspective. Luckily, I **found out a recurrence relation, and independently proved it**. However, when communicating with others in such a great joy, my friend majoring mathematics told me that it's a rather special case that has been studied previously, and for integer partition function, mathematicians usually study the analytical approximation. Yuck. Nonetheless, With his help, I learned a lot of number theory. 
Somedays later, I found there is a [paper](https://arxiv.org/abs/1805.06108#:~:text=A%20generalized%20Hardy%2DRamanujan%20formula%20for%20the%20number%20of%20restricted%20integer%20partitions,-Tiefeng%20Jiang%2C%20Ke&text=We%20derive%20the%20asymptotic%20formula,to%20%5Csqrt%7Bn%7D.) showing a useful formula, and I modified it slightly with what just learned. 

---
# Phase 3
Then I began to connect it with BHs. During this period, I tried four ways: 

1. I followed the work of [Yuxiao Liu and Shaowen Wei](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.123.071103) on counting BH microstates via the Ruppeiner geometry, **discussing the entropy in the scheme of BH molecules**. However, it is virtually irrelevant to our proposal and mainly restricted to the van der Waals analogy. But from this line, I came to the RN-AdS BHs, the thermodynamical stable BHs whose phase space is similar to van der Waals liquid. I **studied the Large/Small BH phase transition** of such BHs and found that the [free energy](../files/LSBH.pdf) does implicate a second-order phase transition. To study its impact on the black hole shadow, the "visual picture" of BHs for an infinite-far-away observer, I **calculated the Lyapunov exponent** for [massless](../files/lya-massless.pdf) and [massive](../files/lya-massive.pdf) particles by MMA and **simulated the reaction of null- and time-like geodesics** respectively. [Click to see the code.](../files/3.0-Timelike%20geodesic.nb) The phase transition brings some interesting phenomena, but I did not continue since it diverges from the original goal. 

2. After the first attempt, I realized we should go beyond the familiar static BHs since negative T systems are out of equilibrium, and then found [M. Park's paper](https://arxiv.org/abs/hep-th/0610140) about the negative T appearing in exotic-BTZ black holes. I **reproduced the result**. But in the discussion with the mentor, we felt some arguments were skeptical. Therefore I did not follow the work. 

3. I considered the negative-entropy objects and **white holes (WH)**, which seem promising for the subject. I **independently proved that for WHs the temperature should be negative** by considering WHs as the time-reversed BHs. However, I then found [Volovik](https://arxiv.org/abs/2103.10954) has published a series of papers for this project, and the problem has been solved ably. Then the scheme aborted. 

4. Meanwhile, I began to consider the possibility of **mapping** a negative T quantum system on the boundary **to the bulk by AdS/CFT**. It requires many mathematical and physical preliminaries, but I was excited about it.  

---
# Phase 4
However, the **pandemic began to rage**. Quarantined at home without enough communication with the mentor, I cannot see any reason to continue the research, and hence becoming very lazy within the excessively comfortable environment. I cheated myself that I will resume after going back to school. However, a vicissitude happened to inflict upon my family that one of my dearest family members had a severe car accident. My family was involved in high medical bills and all sorts of hassles, and I was also helping out every day. Since having no calm mindset for studying, and seeing the project as grim, I eventually decided to quit the group. 

Months later, after dust settling, I concluded all my work in a [report](../files/BH-T.pdf) and submitted it to the National Undergraduate Innovation Program and won the University Award. 

When logging this period, I came to the [paper](https://arxiv.org/abs/1904.04843) written by T. Jacobson *et al*  on the negative temperature, in which they considered the BHs in the casual diamonds with the appearance of upper energy bound. Another interesting possibility I never thought of before. 

---
# Phase 5
In hindsight, I have learned a lot from this subject, which has led me into the palace of theoretical physics. I appreciate all of it in terms of this. However, this has also revealed my problems like being too timid to confer with the mentor, being oblivous of background research, and giving up easily. In a word, too student-like. 

Now, after a whole year, I believe I have been more matured. Hope this unsuccessful starting could be my toll ticking once I am on the verge of relapsing.