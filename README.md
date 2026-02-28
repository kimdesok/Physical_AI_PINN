# Physical_AI_PINN
**Introduction to PINN**<br>
-Assisted by the chatbots such as Gemini, ChatGPT, and Claude

1. From data-driven to physics-informed 
In manufacturing, if a "black box" AI predicts a robotic arm should move through a solid steel wall because that's the "fastest path," you have a multi-million dollar disaster, whereas in computer vision, if an AI predicts a normal for a cancer, the consequence is a wrong label that may have some room for a human intervention. 

Physics-Informed Neural Networks (PINNs) solve this by embedding physical laws—like the laws of thermodynamics, gravity, or fluid dynamics—directly into the model's loss function. 
>* Traditional AI: Learns purely from examples (patterns).<br>
>* PINN: Learns from examples plus equations (e.g., or Navier-Stokes). 
If the AI suggests a move that violates these equations, the model penalizes itself during training.

2. Build bridge between math and physical reality
* Instead of relying on 'big data', we use sensor data (temperature, pressure, velocity, etc) and combine it with a math model of the machine.
* First we train the model in high-fidelity simulation (so called Sim to Real transfer)

3. What advantages using PINNs offers
* Transparency : since the model follows known physics, its choice can be explained.
* Sample efficiency : because the model is aware of gravity exists, it does not required to be shown numerous videos of things falling.  This saves lots of time and effort
* Safety : less halluciations. even a hallucinated choice can be regulated by physical laws.
