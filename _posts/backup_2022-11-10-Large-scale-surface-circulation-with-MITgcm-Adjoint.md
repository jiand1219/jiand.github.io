---
layout: single
classes: wide
category: 
tag: 
author_profile: false
---

The regional sea level off Southwest Australia (Southern Ocean Indian Sector) is more variable, as shown by satellite observation. We thus use ocean models to evaluate how ocean surface drivers affect sea level variation in this region, including **east-west winds**, **north-south winds**, **surface heat**, and **freshwater flux**.

We have two approaches using an ocean model (e.g., <a href="http://mitgcm.org/">MITgcm </a>).

The first one is called Forward Perturbation Experiments. We perturb one element, such as winds, at an initial time and then compare sea level changes at the end between the perturbed and reference runs. Such difference may refer to the Sensitivity of sea level to winds. But it is very expensive if we have many inputs (e.g., winds, heat, and freshwater fluxes) in the forward model. We also have to consider the perturbation time, location, and magnitude, which we do not necessarily know. For every change we made, we had to rerun the model.
{% include figure image_path="/assets/Post_pics/adjoint.png" alt="this is a placeholder image" caption="" %}
Luckily, we can use the Adjoint model to estimate sensitivities with one simulation, which reveals the underlying dynamical processes that affect sea level variation. Contrary to the forward model, the adjoint model runs backward in time, driven by a cost function, **a three-year mean sea level height averaged over the region**. The outputs of adjoint model are sensitivities to model variables.

We can identify oceanic processes, such as the **Rossby waves**, **coastally trapped waves**, **Ekman pumping** and **ACC mean flows**, indicated by the sensitivity pattern and pathway.

{% include figure image_path="/assets/Post_pics/Sensitivity_to_winds.png" alt="this is a placeholder image" caption="The red box is the region where we define the cost function" %}
{% include figure image_path="/assets/Post_pics/Sensitivity_to_buoy.PNG" alt="this is a placeholder image" %}
Positive/Negative sensitivities mean a positive perturbation of this element at this lag time and location can increase/decrease the value of the Sea-Level variation in the end.

Note that sensitivities have a different unit. So how can we compare their relative importance? First, we can multiply the sensitivities with its forcing uncertainty/variability. In other words, we estimate the response of sea level to forcing. Then, focusing on the leading factor winds, we can further carry out sensitivity-like forward perturbation experiments in which the initial wind stress forcing is perturbed, and its pattern is distributed like sensitivity.

Now we show the animation of SSH anomaly in response to sensitivity-like wind perturbation. Finally, we see how wind-driven ocean circulation affects Sea-Level variation.

{% include video id="IMHYVRroZgo" provider="youtube" %}


<a href="https://github.com/oceanography-rookie/Adjoint-sensitivity/blob/main/MSc_thesis.pdf"> Master Thesis </a>


<a href="https://github.com/oceanography-rookie/Adjoint-sensitivity/blob/main/adjoint%20sensitivity_defense_slide.pdf"> Defense slide </a>