# Chapter 1: An introduction to Unity ML-Agents with WallJump

The article "An introduction to Unity ML-Agents" is published [here](https://towardsdatascience.com/an-introduction-to-unity-ml-agents-6238452fcf4c)

You can see the agent performing after 300,000 training timesteps [here](https://youtu.be/BeVhuZNW1pM).

## How to

- Move your model file into `UnitySDK/Assets/ML-Agents/Examples/WallJump/TFModels`.
- Open the Unity Editor, and select `WallJump` scene.
- Select the `WallJumpArea` prefab object and open it.
- Select `Agent`.
- In Agent `Behavior Parameters`, drag the `SmallWallJump.nn` file to `Model` Placeholder.
- Drag the `SmallWallJump.nn` file to `No Wall Brain` Placeholder.
- Drag the `SmallWallJump.nn` file to `Small Wall Brain` Placeholder.
- Drag the `BigWallJump.nn` file to `No Wall Brain` Placeholder.
- Press the ▶️ button at the top of the Editor.
- Enjoy !

## The different saved models

As explained in the article, I tried 3 different training configurations.

- `First Training [BEST]`: PPO with default configuration provided by Unity.
- `Second Training`: PPO with a gamma of 0.95.
- `Third Training`: PPO with hidden Units of 512.

--> The best result is the `First Training`.

