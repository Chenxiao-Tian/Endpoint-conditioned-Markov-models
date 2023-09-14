# Endpoint-conditioned-Markov-models
# Endpoint-conditioned Markov models

## Project Summary

Using endpoint-conditioned Markov models allows the representation of origin-destination paths as higher-order networks.

## Project Meetings

### [2023-09-12 Tue] Meeting

- **Participants**: Juergen Hackl (JH), Chenxiao-Tian (CT)

- **Minutes**:

  - Discussed the initial idea of having endpoint-conditioned Markov models to better describe physical processes that follow an origin-destination assumption

  - Highlighted potential challenges associated with the discrete model where $n$ steps are given:

    1. $n$ might be shorter than the shortest path i.e., walker will stop in the middle of the path

    2. $n$ is a number which cannot reach the target node at step $n$ e.g., On an x-axis, start from the 0, odd number target node can not be reached by even number steps 

  - A continuous model might be better for capturing time-related processes like road transportation

  - The model can have two flavors:

    1. When the walker reaches the destination node, the process ends

    2. The walker will continue his walk even after he visited the destination node

  - the parameters $n$ and $t$ could be interpreted as indicators of how efficient a process is. i.e., if $n$ is close to the shortest path, processes might be optimized（i.e. more restrictions and less choices and randomness for possible walking paths) while $n$ increases, more randomness can be observed. in the extreme case where $n \to \infty$ a "classical" random walker process can be observed(i.e.,no extra restriction on the random walker when n is infinite)

  - There might be a phase transition when the regime shifts from a "random walker" to a "shortest path walker".

    - We do not know how this transition would look

    - We do not know how topology influences this transition
   
    - The most common phase transition timepoint may happen when the timepoint is "closed" to n and t, maybe exist other phase transition timepoint preference in real-world datasets.

- **Tasks**
