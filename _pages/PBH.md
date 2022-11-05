 
# Phase 1

At the beginning of March 2022, I emailed Prof. Tsai asking if he intended to recruit a student for the summer research. Unfortunately, he had already been mentoring four undergraduates, and so there was no room for me. But he said welcome for my physics questions. Therefore, I began to study his work and communicate with him.   

Initially, **I tried to study his work related to [unitary bound](https://arxiv.org/abs/2103.13396)**, which is interesting to me since, in undergraduate, the unitarity is always (though sloppily) assumed as right. I used to take it for granted. So the mechanism and "aftermath" of violating it seems intriguing.  

At the time, I had learned QFT for a semester, covering part-I of the Peskin, but the question they discussed is the lepton physics and the Stueckelberg limit, neither of which are familiar to me. It took time to understand. 

I collated my thought and confusion in an email and sent it to Prof. Tsai. To be honest, I waited in the anxiety of being chided as naive or stupid. Surprisingly, he answered me with kindness. Since then, we have talked about physics several times. During this time, I learned about electroweak theory.  

---
# Phase 2
One day, I **came to the paper about the generalized uncertainty principle** [(GUP)](https://arxiv.org/abs/gr-qc/9904026), whose motivation is that the uncertainty principle should be, at least phenomenologically, corrected due to quantum gravity effect. It seems interesting to me. At first glance, I thought the new relationship could produce negative temperature for BHs. Although the imagination is wrong, I still found something there: the way of correcting it not satisfies my taste. The meaningful argument may also lead to another extrapolation, which seems more simple and elegant, and can produce the same result as before. 

I shared it with my friend, and he believed it is indeed more beautiful and encouraged me to inquire professors studying it. I did, but the professors at the school weren't even going to listen to me. It was so disappointing. But still, I cherished the little idea that I found independently, and wondered if it made sense. So I sent an email to Prof. Tsai, hope at least he would listen to me. 

It really touched me that he read my note and aksed me the reference although it was not the field he specialized in. We then discussed it several times. I did many research to justify it, and even tried to give it a connection with BH/String transition. But my passion eventually gradually faded away, and there was always some intrinsic issues of GUP. We finally did not elaborate on it.

I don't know if it is a good physics. And I also don't konw if I will back to it in the future. It could be a mere interlude in my academic life. Or maybe I will hone it when I become more matured. In retrospect, I should not be angry about my school's professors, because they are not obliged for it, and maybe I should show them with a more systemetic and formal presentation. 

But there is somewhat melencholy in the heart. 

---
# Phase 3
The question-and-answer exchange lasted for months, and one day in July, Prof. Tsai asked me would I like to **do some research about the Hawking emission**, and I said yes since having long been curious about the detail of Hawking radiation. 

I was stunned by reading [Unruh's](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.14.3251) and [Page's](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.16.2402)  papers because in the study of QFT before, I had been viewing the field as a mere tool to produce particles, yet in the more general curved spacetime, it seems that the field is the real protagonist, and there is even no globally well-defined expansion for particles. We extract everything from the CLASSICAL field, like the flux. It was probabily **at this time that I understand what does the "field" mean**. 

Some ambiguous similarities between their papers intrigued me, so I chose to **study the [Hawking's original paper](https://link.springer.com/article/10.1007/BF02345020) to find a unification**. Although I was very slow, basically less than one page per day, it was very beneficial and I started to understand the physical meaning of Hawking's radiation transcending the mere Bogliubov transformation as before. Luckily, I got a clear picture of the whole framework, and found that the works of Unruh and Page are really two sides of the same coin. 

Also, by reading the [paper of Parsides](https://aip.scitation.org/doi/abs/10.1063/1.1666431?journalCode=jmp), I learned some **ODE tools**, including Wroskian and Frobenius method, to discuss field equations in curved spacetime **in a semi-analytical way**. It gives us physical intuition clearly, which later benefits the discussion about some issues in the calculation. 

At this time, I stumbled upon the field called BH-cloud, discussing the bound quantum fields outside of BHs. In another research with the advisor of ITP-CAS, a student in the same group who has been studying the axion cloud outside of RN BHs, and **I teached him how to make an analogy between the bound state electrons in atoms and the bound quantum fields in black hole spacetime**, which is very interesting. 

After doing background research, I found our previous thoughts for the topic is not precise, and what we initially hope to do was actually done by others. Based on the above work, I **made a [report](../files/hawkingppt.pdf)** to Prof. Tsai and Postdoc. Tao, and **we modified and formalized the original argument**, and then started the specific calculation. 

---

# Phase 4
The research firsly **requires a new code for producing the Hawking emission of massive particles**, beacause the widely used code, [BlackHawk](https://blackhawk.hepforge.org/), for calculating the radiation doesn't involve the particle mass parameters. It is a not-so-bad approximation, but not appropriate to our proposal. 

However, I was almost unversed in the numerical tools. I used to disgus it, treated it as a deception. But it is wrong, rejecting it is like the 19th century physicists rejecting calculus. I had **learned a lot of bottom-up numerical techniques** and wanted to write my own iterative function to integrate the field directly. Nonetheless, for two weeks without even a workable program, I got disappointed, and secretly believed I have no gift for it. **Prof. Tsai suggested me to use NDSolve** directly, and then the computation was gradually on track.

The code finally works with help of the document and the Stack Overflow forum. But **the result was very stiff**, yielding answers wrongly easily. And I even didn't know what went wrong. So I was under a great pressure then. But a few days later, I learned the *for function* and **realized the parameters can redefined**, making the equation very neat. Based on this, I eventually got a stable code producing the same result as that of papers. 

The great pleasure overwhelmed me that I thought the numerical work was done, and reported my progress too optimistically in the meeting. But then we found although the qualitative trend was right, but the **specific values were a bit off**. So I came back to the code, pored every line until fully understand the meaning of each part, and compared the existing literature with my code. It turned out that **the difference is in the notation**. 

Things just do not go as our expectations. When I began to vary the particle mass, there will be **some extreme parameters** appearing, breaking the code again, or at least making it unusually slow. I tried many ways to solve it, like the parallelize method or other notations, but none of them worked. Again a progressless week. 

In the meeting, Prof. Tsai told me the real reason why we focus on PBH and pions. In a specific interval, all mass parameters of these stuff are comparable, and under my notion are all unitary numbers. So it seems that the **sloppy values I googled are not suitable** for our research, and **within the specific scope we care about, the code behaves very well**. Then Postdoc. Tao joined the calculation, giving the reference and the formula to calculate the photon production rate from pions. We need to integrate our codes. 

---
# Phase 5
In this process, I found some subtle mistakes in Tao's code, and after communicating with him, we found it was actually something much more profound. I used the semi-analytical way to discuss the field's behavior, and realized the issue is in the curved spacetime without translantional invariance, the transition rate can only be rightly derived from the flux ratio, rather than sloppily observing the amplitude of asymptotic expansions. This is usually confusing for particle physicists especially who without too much GR training. 

So far, the basic work is done, and we are going to collate materials and begin to write the paper. 

To be continued. 