# McRobot
This repo is intended to hold all of the components needed for a robot. Currently it holds libraries related to making a decision.

### s-lang
Allows a modeller to define whats important to our bot or agent, hence forth agent, plain language criteria (tags) for how to achieve important things, goals, through actions. Goals, tags and actions are link through triples and quads.

Later this modelling step can be adjusted so just narratives through LLM like chatGPT allow for agent definition.

It is also the starting point for orchestration of state processing and graph initialisation. The graph is populated and the processes service generates tags, based on state (a snapshot of the world).

### knowledge
Knowledge is responsible for some data scraping, graph definition, graph recomputation based on state and path finding to the best decision.

### processes
Processes polls for the latest state, generates tags based on the snapshot of the world based on some predefined functions and updates knowledge with tags which are presently applicable.

## Note
This project is a work in progress and is an example of a decision making tool, it shouldn't be used for anything risky right now.