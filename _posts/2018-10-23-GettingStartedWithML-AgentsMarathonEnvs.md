---
layout: rlpost
title: Getting Started With MarathonEnvs v0.5.0a
subtitle: Quick tutorial to get you up and going with MarathonEnvs
date:
  '2018-10-23 11:30:00 +0800': null
author: Joe Booth
published: true
category: rl
---
![Banner](/images/MarathonEnvsBanner.gif)
## TL;DR
* TODO add download link!

## About MarathonEnvs

## Setting up your development repository (the fast way)

If you are adding MarathonEnvs to an existing ML-Agents project, or want to customize your install, see Setting up your development repository (the slow way) below

### Install Unity 2017.4 or above 

Download [Unity](https://store.unity.com/download) from the Unity Store


### Setup Your Repository

Goto [GitHub MarathonEnvs 0.5.0a Release](https://github.com/Unity-Technologies/marathon-envs/releases/tag/0.5.0a) and download the `QuickStart_xxx.zip`. 

Quick Start includes the following in a single zip.
   * marathon-envs-0.5.0a
   * ml-agents-0.5-3.0a
   * TensorFlowSharp
   
Unzip to you development folder.


### Setup Up Python

Follow excelant [ML-Agents Documentation](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md#install-python-and-mlagents-package) on how to set up your python development enviorment.


## Running the pre-trained models

### Open Unity And Your Project
   ![v0.5OpenProject](/images/v0.5OpenProject.png)


### Open The Walker Scene
   * Open `UnitySDK⁩\Assets⁩\MarathonEnvs⁩\Environments⁩\DeepMindWalker⁩\Scenes⁩\DeepMindWalker.unity`
   ![v0.5OpenWalker](/images/v0.5OpenWalker.png)

### Press Play
   * This will run the pretrained model `DeepMindWalker108-1m.bytes` 
   * ... This model was trained using 16 agents over 1m simulation steps

| Walker |
|--|
| ![DeepMindWalker108-1m.gif](/images/DeepMindWalker108-1m.gif) |


### Check Out Humanoind, Hopper and Ant
| Humanoid |
|--|
| ![DeepMindHumanoid102-2m.gif](/images/DeepMindHumanoid102-2m.gif) |

| Hopper | Ant |
|--|--|
| ![DeepMindHopper101-1m.gif](/images/DeepMindHopper101-1m.gif) | ![OpenAIAnt102-1m.gif](/images/OpenAIAnt102-1m.gif) |


# Training hopper
* switching to training mode

* Training the walker
* Training the ant
* Training the humanoid

 * Reward Function
 * Termination
 * Observations



## Setting up your development repository (the slow way)
* Ensure you have Unity 2017.4 or above

1. download ML-Agents Beta 0.5.0a ([GitHub](https://github.com/Unity-Technologies/ml-agents/releases/tag/0.5.0a)) ([zip](https://github.com/Unity-Technologies/ml-agents/archive/0.5.0a.zip))
   * Unzip `ml-agents-0.5a` to your `Development` folder 
   ![folder](/images/v0.5ml-agents-0.5a.png)
1. download MarathonEnvs 0.5.0a ([GitHub](https://github.com/Unity-Technologies/marathon-envs/releases/tag/0.5.0a)) ([zip](https://github.com/Unity-Technologies/marathon-envs/archive/0.5.0a.zip))
   * Unzip `⁨marathon-envs-0.5.0a⁩`
   * Copy `⁨marathon-envs-0.5.0a⁩/config/marathon_envs_config.yaml` to `ml-agents-0.5a⁩/config⁩`
   ![folder](/images/v0.5config.png)
   * Copy `⁨marathon-envs-0.5.0a⁩/MarathonEnvs` to `Development⁩/ml-agents-0.5a/UnitySDK/Assets/⁩`
   ![folder](/images/v0.5assets.png)
1. download TFSharpPlugin ([zip](https://s3.amazonaws.com/unity-ml-agents/0.5/TFSharpPlugin.unitypackage))
   * Open your project with Unity
   ![v0.5OpenProject](/images/v0.5OpenProject.png)
   * Add the package
   ![InstallTFsharp](/images/v0.5InstallTFsharp.png)
   * To let ML-Agents know TensorFlowSharp is installed, goto the Player settings:
   ![InstallTFsharp](/images/v0.5PlayerSettings1.png)
   * ... and add `ENABLE_TENSORFLOW` to Scripting Define Symbols
   ![InstallTFsharp](/images/v0.5PlayerSettings2.png)
