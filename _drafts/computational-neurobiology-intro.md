Computational Neurobiology is about building computational models in the field of Neurobiology. Neurobiology is Biology that studies brain. Thus usually it is all about models of neurons but other brain cells might be included too.
It really takes a lot of fancy words to describe what "building computational models" means so I'd prefer to do it by example. Lets take some neuron. You can see that it is not a usual cell. It branches a lot and still it is a single cell.
(TODO Picture of neuron and usual cell, both beautiful and from open sources)

Now lets think about why do we need a model. Probably most of us know that neuron passes electricity through itself. So lets build a model that shows how electricity flows in and out of neuron. For example if inject current in the point A will it get to the point B? What other points will receive current too?
(TODO Picture of the neuron from above with points and icon of current)

To answer those questions we represent neuron as an electric circuit. It's very convenient cause we know a lot about circuits, especially how current passes through them. I'm leaving all the laws and theorems that prove such neuron representation aside. But the main point is that neuron can be represented as electric circuit. In this case circuit is the model that shows neuron's electric properties and neglects others.
Enough of words, lets build! First of all we simplify the neuron by representing it as a bunch of cables.
(TODO Picture of the neuron transformation to cables)
The trick here is that these cables are not simple conductors. To show what are they exactly lets look only at a part of neuron.
(TODO Picture of transformation to circuit)
So, now can entirely replace our neuron with an electric circuit and show current passes between any points. This model answers our previous questions. But we don't stop here. We have other important questions to ask. Why neuron's branches are not simple conductors? Why there are capacitors? What neuron's current is made of? To answer these we need to look deeper into neuron's structure and inner workings that are made of proteins, lipids, ions and other molecules.

To summarize. We can distinguish three important types of models for neurons: neuron inner workings, neuron as a circuit, network of neurons. And usually, Computational Neurobiology is about them.
