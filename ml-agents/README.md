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

docker run --name test3 --mount type=bind,source="\$(pwd)"/unity-volume,target=/unity-volume -p 5005:5005 ml-agent:latest --docker-target-name=unity-volume ./trainer_config.yaml --env=newborn-lin.x86_64 --train --worker-id=1 --no-graphics;

1/ The web entity has the newborn infos.

2/ It Post via a FLASK api, the newborn infos.

3/ The flask generate a Docker image with the required parameter.

4/ The flask use the Unity build execute method to generate the newborn agent/brain/vector etc.

5/ The training flows.

---

Run the training locally => mlagents-learn trainer_config.yaml --train --newborn-id=00498364502827423045832 --api-connection

Usefull docker command for this project:

Create a docker container => docker build -t ml-agent .

List All all imgages => docker ps -a -q

Follow a launched images => docker logs --follow d3a4f72085b4

Delete all launched images => `docker rm -f $(docker ps -a -q)`

connect to ec2 => ssh -i ec2-test.pem ubuntu@ec2-34-205-63-195.compute-1.amazonaws.com

upload to ec2: scp -i ec2-test.pem newborn_communicator_api/unity-volume/newborn-lin.x86_64 ubuntu@ec2-34-205-63-195.compute-1.amazonaws.com: