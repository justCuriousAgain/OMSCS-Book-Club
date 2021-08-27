# Meeting notes

## Meeting Notes (19th August, 2021)
### Chapter 1: Optimal Stopping
$~$

## Meeting Notes (26th August, 2021)
### Chapter 2: Explore/Exploit
* Difference in Optimal Stopping and Explore/Exploit
  * Explore-exploit is closely related to reinforcement learning in how each state has a set of inputs and a function that produces the outputs which can in-turn produce the new state
  * While Optimal-stopping included making a decision to choose only once, Explore-Exploit involves making a decision multiple times and each time, the experiences or results from the previous decisions affect the likelihood of success.
  * Thus we can either explore new options or exploit the options we previously had success with.
* While Exploit gives us a better probability of success, Explore can result in better outcomes if it is known that the results from that explore deicision will be used as an input to many future decisisons
  *  Hence, the interval over which we plan to take on repeating the decisions plays an important role when deciding to explore or exploit.
* Gittin's index structures the problem with the assumption of 99% geometric 'discounting' of successes in the future
* Examples:
  * Job-changes and hunts:
    * A person changes jobs every N years throughout the career
    * A single-instance of job-hunting can be an Optimal Stopping problem (when to stop exploring jobs and take the best one I get)
    * Each decision of changing a job after N years, can be an Explore-Exploit (should we re-apply to places where we were successful earlier or explore newer places)
  * Online recommendation systems e.g. Spotify:
    * The recommendation function can choose to exploit previously liked or consumed content or 'explore' by suggesting newer content
    * In these cases, it is the computing system instea of the human making the 'explore-exploit' decision
* Explore-exploit can be approached also from the Minimal regret approach where higher stake deicisions like drug-trials which impact human lives need to be taken
$~$