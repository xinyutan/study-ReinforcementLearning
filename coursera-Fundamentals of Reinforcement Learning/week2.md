### Grading criteria

- That you have described an MDP and that it is different than your other two.
- That you have described the MDP's states.
- That you have described the MDP's actions.
- That you have described the MDP's rewards.

### Example 1

We can apply a MDP on a book recommendation system for a user in a library.

States: all the books this user has read at time point t

Action: Among all the books in the library, the book the system recommends to this user is the action. 

Rewards: if the user borrow the book at time point t + 1, then the reward is 2; if the user looks up the book, but does not borrow, the reward is 1; if the user does not look up and marks the recommendation as irrelevant, then the reward is -2.

### Example 2

Suppose we apply reinforcement learning to control the irrigation systems for a farm.

States: current weather, crop type, sensor input for soil dryness, immediate future's weather prediction

Action: {start the irrigation, stop the irrigation, continue the irrigation}

Rewards: If the soil dryness is within a optimal range, the reward is + 1, and if not, then the reward is -1. We define a negative reward if farmer adjust the control system manually.

### Example 3

We can also apply MDP on clinical decision system.

States: the history of the conversation which the system had with the current patient and all the other patients, and the question the patient asks at time t

Action: {continue to ask a question, give a recommendation for a medical diagnosis and procedure}

Rewards: The reward can be if the diagnosis is correct and procedure is reasonable. To discourage a uncontrained number of questions, we can add a negative reward for every question asked.  
