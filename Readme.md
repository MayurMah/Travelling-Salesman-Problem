# Traveling Salesman Problem

## Objective & Summary

**Solve [Travelling Salesman Problem](https://en.wikipedia.org/wiki/Travelling_salesman_problem "Travelling Salesman Problem") for 48 state capitals in US using constraint generation**

Dantzig-Fulkerson-Johnson Formulation has 2^n-2 subtour elimination constraints which makes the problem computationally expensive to solve. For a problem of 48 cities, there will be 2^48 - 2 = 281,474,976,710,654 (281 trillion) subtour elimination constraints. Hence we use constraint generation approach to generate and add constraints to the problem until the a solution is found. <br/>
This approach converges to a solution within 2 minutes for 48-city (48 state capitals in US) tour using the mosel (Xpress) code. Using the same approach, a 26-city tour problem is also solved. 

## Files :

- TSP-DFJ-48.mos: Mosel code for 48 city tour
- TSP-DFJ-26.mos: Mosel code for 26 city tour
- US48.dat: Co-ordinates of 48 state capitals in US
- US26.dat: Co-ordinates of randomly selected 26 state capitals in US
- tourmap_48.png: Plot of the 48 city tour
- tourmap_26.png: Plot of the 26 city tour
- US48TourPlot.m: Matlab code to plot the 48 city tour generated using the mosel code
- US48.input: Input file for the 48 city tour matlab code 
- US48.output: Output file created by the 48 city tour matlab code 
- US26TourPlot.m: Matlab code to plot the 26 city tour generated using the mosel code
- US26.input: Input file for the 48 city tour matlab code 
- US26.output: Output file created by the 48 city tour matlab code 

## Execution:
Language: Mosel, Matlab

1. Download Xpress IVE (https://www.fico.com/en/products/fico-xpress-optimization)
2. Open the TSP-DFJ-48.mos in Xpress and run 
3. Run US48TourPlot.m for plotting the 48 city tour generated using the mosel code
4. Follow steps 2 & 3 for 26 city tour 