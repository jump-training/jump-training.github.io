# 4-legged-walking

## Team Unity: 
* Ko Kanghyuk, 2010009536, over2ture@gmail.com 
* Kim Gihyun, 2014005341, progkim8@naver.com
* Ha Dongsu, 2014005687, gkehdtn4218@gmail.com

## Ⅰ. Introduction
* Motivation: We wanted to see how the machine learning works by using Unity Platform. By using the Unity, it is easy to see the progress while doing machine learning cause unity helps with visualizing the whole progress. Throughout this experience we can see the actual training process entirely.

* The main objective: To get **4-legged-walking** model simulating.

## Ⅱ. Dataset
* We created our own Trained Model File so there's no external dataset.

## Ⅲ. Methodology
* The algorithm we're going to use mainly is DRL, Deep Reinforcement Learning. Deep reinforcement learning (DRL) uses deep learning and reinforcement learning principles in order to create efficient algorithms that can be applied on areas like robotics, video games, finance and healthcare.[1] Implementing deep learning architecture (deep neural networks or etc.) with reinforcement learning algorithms (Q-learning, actor critic or etc.), a powerful model (DRL) can be created that is capable to scale to previously unsolvable problems. You must decide policy so that you can define reward and negative function. DRL can dramatically improve the result by the appropriate setting, especially in Reward and Negative function part.

* Explaining features or code 

## Ⅳ. Evaluation & Analysis
* Unity Engine  
It is a tool for creating interactive content such as 3D video games, architectural visualizations, and simulations. Unity is a 3D engine used by many companies, professionals and practitioners. For this reason, the public resources and community are vast andeveryone can download and use freely available resources and various libraries and resources for development.
* ML-Agents(https://unity3d.com/how-to/unity-machine-learning-agents#how-it-works)  
This solution is called Unity Machine Learning Agents(ML-Agents) and is a beta version of the SDK.The ML-Agents SDK allows researchers and developers to transform games and simulations created using the Unity Editor into environments where intelligent agents can be trained using Deep Reinforcement Learning, Evolutionary Strategies, or other machine learning methods through a simple to use Python API.  
![Structure](./image/ml-agents.png)
* The three main kinds of objects within any Learning Environment are: Agent, Brain, Academy
## Ⅴ. Process


Step 1. Install Cuda

![Picture1](https://user-images.githubusercontent.com/46990290/70840194-02b93600-1e54-11ea-81d6-9ffab3ae821b.jpg)
  
  1)Go to https://developer.nvidia.com/cuda-downloads
  
  2)Download and Install

Step 2. Install Anaconda

![Picture2](https://user-images.githubusercontent.com/46990290/70840205-1b295080-1e54-11ea-857d-0ef34bfacfa3.jpg)

  
  1)Go to https://www.anaconda.com/distribution
  
  2)Download and Install
  
  3)Have python set

Step 3. System Environment variable Path set

![Picture3](https://user-images.githubusercontent.com/46990290/70840216-2e3c2080-1e54-11ea-8361-03da6ad43e68.jpg)

  
  1)Approach to System environmentvariable
  
  2)Edit Path
  
  3)
    C:\ProgramData\Anaconda3\Scripts
    C:\ProgramData\Anaconda3\Scripts\conda.exe
    C:\ProgramData\Anaconda3
    C:\ProgramData\Anaconda3\python.exe

Step 4. Install Tensorflow

![Picture4](https://user-images.githubusercontent.com/46990290/70840251-5b88ce80-1e54-11ea-8ede-7b9f8ed362db.jpg)

  
  1)Execute Anaconda CMD
  
  2)conda create -n ml-agents python=3.6
  
  3)activate ml-agents
  
  4)pip install tensorflow==1.7.1

Step 5. Git download

![Picture5](https://user-images.githubusercontent.com/46990290/70840264-765b4300-1e54-11ea-9a8a-d5b11e9d69a9.jpg)

  
  1)cd directory set in Anaconda CMD
  
  2)git clone https://github.com/jump-training/jump-training.github.io.git


Step 6. Launch Unity with ml-agents project

![Picture6](https://user-images.githubusercontent.com/46990290/70840273-83783200-1e54-11ea-8ce3-2f2e8211e162.jpg)

  
  1)Open Unity project ml-agents/UnitySDK  



Step 7. Train Agent via Deep Reinforcement Learning

![Picture8-1](https://user-images.githubusercontent.com/46990290/70840289-9ee33d00-1e54-11ea-9b9e-99a8aa75f77a.jpg)

![Picture8-2](https://user-images.githubusercontent.com/46990290/70840294-a99dd200-1e54-11ea-9646-33419ed0498a.jpg)

  1)Start train with pre-defined parameters and settings in Config/trainer_config.yaml file
  
  2)mlagents-learn config/trainer_config.yaml --run-id=firstRun –train
  
  3)Wait till step reaches max_steps variable that has been set in trainer_config.yaml (Force Abort Training with Ctrl  + C)
  
  4)Create Trained Model File(models/brain_name.nn)    

Step 8. End Training

![Picture9](https://user-images.githubusercontent.com/46990290/70840299-b4f0fd80-1e54-11ea-9a4c-c20fe06e022e.jpg)

  
  1)Abort Training with Ctrl  + C
  
  2)Create Trained Model File(brain_name.nn)

Step 9. Set the Learned Agent Model

![Picture10](https://user-images.githubusercontent.com/46990290/70840307-bf12fc00-1e54-11ea-9d3a-6fcb02dc02ad.jpg)

  
  1)Move Trained Model File to Project Folder
  
  2)Set it to the Brain Model  
 

Cf. Here's the entire tutorial video(Click to Play)

[![Video Label](http://img.youtube.com/vi/matu6cs7aBw/0.jpg)](https://youtu.be/matu6cs7aBw?t=0s) 



## Ⅵ. Related Work(e.g., existing studies)
* Hide / Escape - Avoidance of Pursuing Enemies.  
Training ML Agents to Avoid Traditional AI Using Curriculum-Based Reinforcement Learning.(https://connect.unity.com/p/hide-escape-avoidance-of-pursuing-enemies?_ga=2.134864823.771982053.1572239590-1717690672.1568966025)

* -37,8 +86,8 @@ Training ML Agents to Avoid Traditional AI Using Curriculum-Based Reinforcement
Pass the Butter / Pancake bot  
(https://connect.unity.com/p/pancake-bot?_ga=2.134864823.771982053.1572239590-1717690672.1568966025)

* Vehicle Environment Static Obstacles with Unity ML-Agent.  
(https://connect.unity.com/p/vehicle-environment-static-environment?_ga=2.100325208.771982053.1572239590-1717690672.1568966025)

* This simulator is simple vehicle environment. In this environment, Agent should evade obstacle and get stars while keeps center of the lane.  
Pass the Butter / Pancake bot  
(https://connect.unity.com/p/pancake-bot?_ga=2.134864823.771982053.1572239590-1717690672.1568966025)

## VII. Conclusion
* We could see that machine learning acutally acts as we predicted. It improved in performance as trained more.
* To See the acutal improvement of performance, we attached before&after video of it.

-Before(Click to Play)

[![Video Label](http://img.youtube.com/vi/9M_yeAVkCOs/0.jpg)](https://youtu.be/9M_yeAVkCOs?t=0s) 


-After(Click to Play)

[![Video Label](http://img.youtube.com/vi/YWVeRdl0A84/0.jpg)](https://youtu.be/YWVeRdl0A84?t=0s) 



## About ML-Agents
**The Unity Machine Learning Agents Toolkit** (ML-Agents) is an open-source
Unity plugin that enables games and simulations to serve as environments for
training intelligent agents. Agents can be trained using reinforcement learning,
imitation learning, neuroevolution, or other machine learning methods through a
simple-to-use Python API. We also provide implementations (based on TensorFlow)
of state-of-the-art algorithms to enable game developers and hobbyists to easily
train intelligent agents for 2D, 3D and VR/AR games. These trained agents can be
used for multiple purposes, including controlling NPC behavior (in a variety of
settings such as multi-agent and adversarial), automated testing of game builds
and evaluating different game design decisions pre-release. The ML-Agents
toolkit is mutually beneficial for both game developers and AI researchers as it
provides a central platform where advances in AI can be evaluated on Unity’s
rich environments and then made accessible to the wider research and game
developer communities.


