# Meeting notes

## Meeting Notes (19th August, 2021)
### Chapter 1: Optimal Stopping

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

## Meeting Notes (9th September, 2021)
### Chapter 2: Sorting
* Most compute power spent on sorting: Interesting to analyze how important to analyse and optimize sorting
* Most social-media is sorting content for the user - sorting might be based on different paramters (most recent, most viewed, etc.)
* Entire media experience is also affected by how the content is sorted
* Dinner table example was good
    * Interesting to read about dinner-table examples
    * Relatables examples which are relatable
* Recommendation systems - maximize hit-score
* Library based book-sort involves Bucket-sort
* Web v/s Email:
    * Email: search less → sorting less useful
    * Web-search: Sorting is more useful
    * Can't distribute emails over multiple data-centers unlike other web-content because incomplete emails being accessible to user is unacceptable
* Search can be efficient with sorting → reduce search space
* Hiring: Remove the junk applicantions
    * Elimination versus Selecting
    * JEE and B-Schools: Elimination needs to be adapted to manage the volume of applicants
* Oxford mathematician: Great to know the pen-name of Lewis Carroll
    * 2nd position is false
* Comparing-counting sorting
* Premier League and other sport leagues: 
  * Many leagues play more games than are required to either make the competition more interesting or just sell more tickets
  * Main reason why many matches or games can be not so interesting towards the end of the tournament

## Meeting Notes (16th September, 2021)
### Chapter 2: Caching
* Different techniques can be used to cache data or objects: LRU, FIFO, Random
  * Different techniques can perform better fot different scenarios & applications
* Some CDNs may optimize for performance by sometimes showing older content when the most readily available server may not be synchronized with the latest updates
  * URLs are used as keys, and the content as Objects. If the name doesn't match then the cache is replaced or updates: 'Stale while revalidate' e.g. Online courses
* Caching associated data: Video streaming buffers next possible consumable content, but can lag when the video is randomly browsed through
* Human forgetfullness is also analogous to a cache-miss e.g. Old people might forget memories childhood memories
  * Memory loss can (e.g. in sclerosis) can be due to signal loss in the chain of neurons when the insulation layer on the neurons wears off or is inadequate
* Forgetting Curve & spaced repitions -> interesting to note that the sample-size for the study was '1'. Thus not optimal and not fully random.
* Good memory is not always a virtue:
  * E.g. Anxiety -> humans almost relive the moments when anxious
  * Since the human focuses on anomalies and invokes emotions the associations can be strong
  * Disassociating anxiety triggers is difficult -> (1) decay (2) exact same triggers but opposite result
* Meditation
  * Is more about sorting out the thoughts or being mindful than being without any thoughts at all
  * Headspace app example: Sitting by the road letting the traffic(cars == thoughts) pass by
  * Thoughts: Analogous to finding a way through a maze, not knowing what the next turn (next thought) will be