# Practice-ML " Practice from 2024 KRICT Hackathon"

## Background 
Thermoelectric (TE) materials can either harvest waste heat as electrical power via the Seebeck effect or, conversely, pump heat when an electric current is applied through the Peltier effect. Their performance is quantified by the dimensionless figure of merit $ZT(T) = \frac{S(T)^{2}\sigma(T)T}{\kappa(T)}$, where S is the Seebeck coefficient, σ the electrical conductivity, T the absolute temperature, and κ the thermal conductivity. An ideal TE material therefore combines high σ, a large S, and a low κ. Because each transport coefficient changes with temperature, the full ZT(T) curve reveals not only the temperature at which a material reaches peak efficiency but also how robust that performance remains across an operating window. Careful analysis of these trends sheds light on the underlying carrier-transport mechanisms and long-term stability—insights that are indispensable for engineering high-efficiency thermoelectric generators, particularly multi-stage devices in which different compounds operate in distinct temperature ranges.

## Data set
The LitDX dataset, provided as an xlsx file (data/estm.xlsx), contains zT, S, σ, and κ values at different temperatures for various inorganic materials.

## Method
A composition-only neural network, CrabNet, was applied to refine the raw property predictions. Because CrabNet operates solely on the chemical formula, it remains agnostic to crystal structure details, making it ideal for large, heterogeneous datasets where full structural information is often missing.

## Purpose of machine learning
Practice aims to develop a multi-task model to predict the temperature dependence of the thermoelectric figure-of-merit (ZT) for different inorganic materials.
