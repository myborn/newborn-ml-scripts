# Unity ML-Agents Python Interface and Trainers

The `mlagents` Python package is part of the
[ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents).
`mlagents` provides a Python API that allows direct interaction with the Unity
game engine as well as a collection of trainers and algorithms to train agents
in Unity environments.

The `mlagents` Python package contains two sub packages:

- `mlagents.envs`: A low level API which allows you to interact directly with a
  Unity Environment. See
  [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Python-API.md)
  for more information on using this package.

- `mlagents.trainers`: A set of Reinforcement Learning algorithms designed to be
  used with Unity environments. Access them using the: `mlagents-learn` access
  point. See
  [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-ML-Agents.md)
  for more information on using this package.

## Installation

Install the `mlagents` package with:

```sh
pip install mlagents
```

## Usage & More Information

For more detailed documentation, check out the
[ML-Agents Toolkit documentation.](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Readme.md)

# Unity ML-Agents Python Interface

The `mlagents_envs` Python package is part of the
[ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents).
`mlagents_envs` provides a Python API that allows direct interaction with the Unity
game engine. It is used by the trainer implementation in `mlagents` as well as
the `gym-unity` package to perform reinforcement learning within Unity. `mlagents_envs` can be
used independently of `mlagents` for Python communication.

The `mlagents_envs` Python package contains one sub package:

- `mlagents.envs`: A low level API which allows you to interact directly with a
  Unity Environment. See
  [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Python-API.md)
  for more information on using this package.

## Installation

Install the `mlagents_envs` package with:

```sh
pip install mlagents_envs
```

## Usage & More Information

For more detailed documentation, check out the
[ML-Agents Toolkit documentation.](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Readme.md)
