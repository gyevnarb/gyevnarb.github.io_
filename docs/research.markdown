---
title: Research
layout: page
permalink: /research/
---
This page is a collection of current and past research projects ordered by how recently I have worked on the project.

You can also navigate to a list of all my [publications](publications) and [presentations](presentations).


## Explainable AI for Trustworthy Autonomous Systems
While AI methods have shown impressive results in recent times, they are yet to be widely adopted by the public, especially in high-risk domains such as health care or transportation.
I am interested in combining technologies from explainable AI (XAI), causal reasoning, and natural language processing to support the creation of trustworthy AI systems, focusing especially on the domain of autonomous driving.
In my view, there are four main criteria that trustworthy AI should fulfill:

1. Be lawful. 
There is now a heightened interest from lawmakers to regulate AI technologies, and AI systems will have to adhere to the requirements set out in these laws.

2. Be ethical.
Novel technologies are often plagued by side effects --- AI is no different.
Biased and discriminatory decisions, subversive manipulation of people, and violations of privacy are some of the major concerns that need to be addressed urgently.

3. Be social.
The design of AI systems should consider human interactions as a core part of their workflow.
Conversations and understanding of people's cognitive models should help AI systems create relevant and targeted decisions.

4. Be correct and robust. 
All the above considerations are pointless if the AI systems produce garbage or cannot be deployed under real-life circumstances.
Therefore, the testing and validation of AI systems are essential.

My research focuses on building trustworthy AI for autonomous vehicles to support their wider public adoption.
Using XAI, we can reduce the opacity of our systems, enabling accountability, demonstrating legality, and improving testability.
In addition, cognitive modeling and NLP technologies allow us to address the social aspects of trustworthy AI.
I published an [opinion paper](https://arxiv.org/abs/2302.10766) about the above ideas at ECAI 2023 and begun [implementing it in practice](https://arxiv.org/abs/2302.10809) published at AAMAS 2024.


## Generating Human-Centric Causal Explanations in Natural Language for Autonomous Vehicles
The merits and drawbacks of autonomous vehicles are highly contentious topics.
On the one hand, they are predicted to improve transport safety and efficiency, while also making car-based transportation more accessible for people.
On the other hand, autonomous vehicles are complex and integrated systems which are opaque to a passenger.
This opaqueness can lead to concerns that the vehicle might fail in unexpected scenarios, fostering distrust and scepticism in people.

In this project, my goal is to build *trust* and *understanding* in people for autonomous vehicles through explanations.
I focus on explaining the complex high-level motion planning and prediction decisions of autonomous vehicles.
The system that provides these decisions is the transparent interpretable system IGP2.
I aim to build an automatic explanation generation method for IGP2 that is grounded in accurate causal attributions.
The final system should take into consideration the cognitive biases of people, while also being able to run a smooth conversation during its explanations process.
This social nature is to guarantee that the generated explanations are as beneficial for our passengers as possible.
I gave a detailed outline of my vision for this project in an award-winning [essay](assets/IEEE_ITS_Essay.pdf) and a [blog post](https://agents.inf.ed.ac.uk/blog/explainable-autonomous-vehicle-intelligence/).


<br />

# Archive:


## Communicative Efficiency or Iconic Learning: Do developmental and communicative pressures interact to shape colour naming systems?

Language evolution is driven by pressures for simplicity and informativity; however, the timescale on which these pressures operate is debated.
Over several generations, learners' biases for simple and informative systems can guide language evolution.
Over repeated instances of dyadic communication, the principle of least effort dictates that speakers should bias systems towards simplicity and listeners towards informativity, similarly guiding language evolution.
At the same time, it has been argued that learners only provide a bias for simplicity and, thus, users must provide a bias for informativity.
To what extent do languages evolve during acquisition versus use?

In our [submission](https://psyarxiv.com/9zx7u) to the journal Entropy, we address this question by formally defining and investigating the communicative efficiency of acquisition trajectories.
We illustrate our approach using colour-naming systems, replicating the communicative efficiency model of Zaslavsky et al. (2018) and the acquisition model of Beekhuizen and Stevenson (2018).
We find that to the extent language is iconic, learning alone is sufficient to shape evolution.
Concerning colour-naming systems specifically, we find that incorporating learning biases into communicative efficiency accounts might explain how speakers and listeners trade off communicative effort.

## GRIT: Fast, Interpretable, and Verifiable Goal Recognition with Learned Decision Trees for Autonomous Driving
Goal recognition for autonomous vehicles is a crucial aspect of reasoning about the longer-term behaviour of traffic participants.
Performing this quickly and accurately is challenging on its own; however, for the sake of safety, we also require a method to be interpretable and verifiable.

I helped develop and evaluate [GRIT](https://github.com/uoe-agents/GRIT), which fulfils all of the above criteria.
It uses learnt decision trees to infer a probability distribution over possible goals in the neighbourhood of autonomous vehicles from real-world driving data.
We can formally verify the properties of the learnt decisions which gives safety assurance about the correctness of the method.
GRIT is also accurate enough to match the performance of deep learning-based methods while offering transparency about its workings.

## Interpretable Goal-based Prediction and Planning for Autonomous Driving (IGP2)
I am one of the main developers and the primary maintainer of the official code repository of [IGP2 on GitHub](https://github.com/uoe-agents/IGP2) with more than 47 stars and 10 forks.
Our code provides the full functionality of IGP2 and is tightly integrated with the [CARLA driving environment](https://carla.org/) to support high-fidelity simulations.

[IGP2](https://www.five.ai/igp2) is a transparent goal-based prediction and planning module for autonomous vehicles.
It uses a library of high-level driving behaviours called macro actions, such as Exit and Continue, that have intuitive interpretations.
This allows us to give explanations of the generated plans of IGP2 in terms of rationality principles.
IGP2 does not only discover non-trivial opportunities by reasoning about the behaviour of other vehicles, but its inherent interpretability is a hugely desirable property in the safety critical world of autonomous driving.

## Master's Thesis -- Comparison of Account Survival on Twitter During the First Wave of COVID-19 in Four Countries

User accounts on online social networks (OSNs) are constantly changing. 
New ones are created at an increasing pace, while others are deleted by users, protected from public view, or suspended by online service providers. 
    
The study of OSN account survival can shed light on aspects, such as OSN adoption and abandonment, the incidence of bots, or enforcement of OSN platform rules; however, the ongoing pandemic has significantly altered the online behaviour of people. 
In my [thesis](https://project-archive.inf.ed.ac.uk/ug4/20212123/ug4_proj.pdf), I compared the extent to which the first wave of the COVID-19 pandemic between March and April 2020 affected account survival patterns in four countries with different approaches to managing COVID-19: the United States, the United Kingdom, Singapore, and New Zealand. 

I scraped a data set from the Twitter Streaming API between March 10 and April 29, 2020, consisting of 17.3M unique tweets in English by 15.3M unique accounts. 
The thesis revealed significant and consistent differences among patterns of account survival and, most interestingly, a steady decrease in interest over time.
I concluded that account survival types should be taken into account when examining how the pandemic is discussed on Twitter. 
