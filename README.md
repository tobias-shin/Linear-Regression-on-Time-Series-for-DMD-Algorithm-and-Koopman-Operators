This is a directed reading program (DRP) project done with an undergraduate at the University of Chicago.
The project focuses on understanding the trading strategy described by the paper "Dynamic Mode Decomposition for Financial Trading Strategies" 
by Jordan Mann and J. Nathan Kutz (2015). The idea of the paper is to linearly approximate the next sample state in a nonlinear dynamical system.
This is done in theory with composition (Koopman) operators. The trading strategy is to apply this to time series data, using the dynamic mode decomposition (DMD) algorithm.
One takes two data matrices $X$ and $X'$, where $X'$ is the data of $X$ shifted forward in time, and tries to find the best-fit linear approximation $A$ such that
$AX = X'$. This is done with linear regression, and computationally made efficient by taking pseudo-inverses and doing dimensionality reduction onto the leading principal components.
