Computational Neurobiology is about building computational models in the field of Neurobiology. Neurobiology is Biology that studies brain. Thus usually it is all about models of neurons but other brain cells might be included too.
It really takes a lot of fancy words to describe what "building computational models" means so I'd prefer to do it by example. Lets take some neuron. You can see that it is not a usual cell. It branches a lot and still it is a single cell.
(TODO Picture of neuron and usual cell, both beautiful and from open sources)

Now lets think about why do we need a model. Probably most of us know that neuron passes electricity through itself. So lets build a model that shows how electricity flows in and out of neuron. For example if inject current in the point A will it get to the point B? What other points will receive current too?
(TODO Picture of the neuron from above with points and icon of current)

To answer those questions we represent neuron as an electric circuit. It's very convenient cause we know a lot about circuits, especially how current passes through them. I'm leaving all the laws and theorems that prove such neuron representation aside. But the main point is that neuron can be represented as electric circuit. In this case circuit is the model that shows neuron's electric properties and neglects others.
Enough of words, lets build! First of all we simplify the neuron by representing it as a bunch of cables.
(TODO Picture of the neuron transformation to cables http://slideplayer.com/slide/6975345/24/)
The trick here is that these cables are not simple conductors. To show what are they exactly lets look only at a part of neuron.
(TODO Picture of transformation to circuit https://commons.wikimedia.org/wiki/File:Original_neuron,_a_cable_model_%26_a_compartmental_models.png?uselang=en-gb)
So, now we can entirely replace our neuron with an electric circuit and show how current passes between any points. This model answers our previous questions. But we don't stop here. We have other important questions to ask. Why neuron's branches are not simple conductors? Why there are capacitors? What neuron's current is made of? To answer these we need to look deeper into neuron's structure and inner workings that are made of proteins, lipids, ions and other molecules.
(TODO Picture of the neuron's inside)
Lets look at neuron's membrane. Remember neuron is a cell, so it has a membrane. Membrane is impermeable but it has little holes which allow molecules to pass through. These holes are not just holes. They are special gates that allow only some particles to pass. Usually they are called channels. There are many different types of channels. Each type is responsible for its own group of molecules.
(Picture of 3d membrane http://jonlieffmd.com/category/blog/neuronal-plasticity-blog)
(Picture Membrane to circuit http://slideplayer.com/slide/4232029/)
Now let me remind you that current is a motion of charged particles. In usual cables particles are electrons but in neuron they are ions like K, Na or Cl. These ions move along neuron branches creating current but remember about those holes (channels) prepared for them. For each type of ion there is at least one channel that allows it to pass. In this way current goes not only along the membrane but also across it. The cross current makes a capacitor out of the membrane. Such current propagation depends heavily on the number and types of holes, the membrane thickness and other parameters. That is why it is very important to build models of neuron's branches in order to determine the properties of electric circuit.

Ok, so we know how current goes along the neuron and what it is made of. Can current go from one neuron to another? Of course it can! Just not directly ;-) If neurons behave as usual cables then one electrified neuron would charge all neighbours. In turn neighbours would electrify their neighbours and so on. The never ending cycle. To prevent this most of neurons are not directly connected. They are connected through a special mechanism called synapse. Synapse is a place where two neurons are very close to each other. The thin space between them is a synapse. So, once current achieves a synapse, it makes synapse release special molecules that may or may not elicit current on the opposite neuron. Such transmission allow neuron to choose whether to pass current further or not. It's very useful in situations when you are thinking hard about something and other thoughts can't disturb you. Other thoughts are just inhibited at their synapses.
(Synapse is in the inline image https://camo.githubusercontent.com/eda8fefbbd8d96edfc15fa6f36a286539b883695/687474703a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f332f33302f4368656d6963616c5f73796e617073655f736368656d615f63726f707065642e6a7067)
How model synapse? Well, it's complicated. You can think of it as a switch between two electric circuits. This switch turns on when current in the first scheme passes some threshold but you understand that in real life the threshold is a dynamic value that depends on many parameters. For now the switch is enough for you to know.
(draw an electric scheme of gap junction like where two simple cicruits are connected through a switch)

When we can model neurons and connections between them, we can model a group of them or even groups of groups of them.



To summarize. We can distinguish three important types of models for neurons: neuron inner workings, neuron as a circuit, network of neurons. And usually, Computational Neurobiology is about them.
