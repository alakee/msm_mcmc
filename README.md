#msm_mcmc

#Estimating Multi-State Models for Panel Data via Markov Chain Monte Carlo Methods

###Introduction

This repository provides a set of R methods which allow the user to
1)	Simulate panel data from time homogenous Markov multi-state processes, and
2)	Estimate time homogenous Markov multi-state models via Markov Chain Monte Carlo methods such as Metropolis – Hastings and Hamiltonian Monte Carlo (second is in progress).

###Multi-state models

Multi-state models are used to model the movement of subjects from one state to another through continuous time. These states can either be absorbing, where no transition occurs, or transient, where transitions can be in or out. Panel data is obtained when observations of a continuous-time process are made arbitrarily. 

###Assumptions

The assumption of time homogeneity implies that transition intensities are constant through time. The Markov assumption implies that future transitions are independent of the past, conditional only on the current state. While the Markov assumption can be restrictive, it is required to compute the likelihood for panel data. The set of methods available in this repository assume that the observation times are non-informative. This means that the time in which the observations are made are assumed to contain no information about the parameters of interest (i.e. the transition intensities).

