# Using jax for computational materials science!
This is a collection of Jupyter notebooks showing how to combine jax with various computational material science algorithms in an easy-to-read fashion. This is not meant to be production-ready code, but rather serve as an entry-point into how jax can be leveraged for efficient simulations. If looking for a full fledged MD package using JAX, please see https://github.com/jax-md/jax-md. If you are unfamiliar with JAX in general, I'd recommend going to the start page of their readthedocs here: https://jax.readthedocs.io/en/latest/beginner_guide.html#beginner-guide. 

## Description of Notebooks

1)   Simple_Classes.ipynb | This notebook shows & documents a simple class using jax that leverages various capabilities. While jax is meant to be a functional programming approach, it can still be leveraged with custom datastructures! This procedure requires the use of functool's partial operator, and there are some specific limitations that must always be considered when using custom classes with JAX.

2)   Hard_Spheres.ipynb | A simple notebook showing a system of hard sphere particles. This generally covers some of the basic functions (i.e., intitalizing a system and starting a simulation). However, this is a very simple implementation, and this is not meant to be a production-code level class.
