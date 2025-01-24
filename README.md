# Using jax for computational materials science!
This is a collection of Jupyter notebooks showing how to combine jax with various computational material science algorithms in an easy-to-read fashion. This is not meant to be production-ready code, but rather serve as an entry-point into how jax can be leveraged for efficient simulations. If looking for a full fledged MD package using JAX, please see https://github.com/jax-md/jax-md. If you are unfamiliar with JAX in general, I'd recommend going to the start page of their readthedocs here: https://jax.readthedocs.io/en/latest/beginner_guide.html#beginner-guide. 

## Description of Notebooks

1)   Simple_Classes.ipynb   | This notebook shows & documents a simple class using jax that leverages various capabilities. While jax is meant to be a functional programming approach, it can still be used with custom datastructures to work in a more class-friendly format (while still leveraging the functional programming benefits). This procedure requires the use of functool's partial operator, and there are some specific limitations that must always be considered when using custom classes with JAX.

2)   Hard_Spheres.ipynb     | A simple notebook showing a system of hard sphere particles. This generally covers some of the basic functions (i.e., intitalizing a system and starting a simulation). The general step function of the simulation is inefficient, but there is also some benchmarking of using a non-jitted vs jitted update to the sphere positions and velocities. Also shows how one could use vmap for particle-based (in this case, sphere-based) systems. There is also a derivation of elastic hard sphere collision and a mathematical derivation of how to update hard sphere velocities when collisions occur.

3)   Lennard_Jones.ipynb    | Introduces the lennard jones potential to update the particle positions. This notebook still uses the Newton scheme discussed in hard spheres for position and velocity updates, but now we include a potential which contains a weak attractive at certain distances but a strong repulsive force at others.

4)   Time_Integration.ipynb | Different numerical schemes are investigates to ensure that the simulator is properly conserving energy throughout the simulation. A comparison is shown between 2nd and 3rd order Taylor Expansions, Verlet velocity, and Stormer-Verlet
