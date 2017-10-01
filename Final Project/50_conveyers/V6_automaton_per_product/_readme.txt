Each box is modeled by means of a separate automaton
- each box automaton keeps track of its position on all conveyers

The first model (system_perbox1.cif) declares each sensor as an algebraic variable by means of a function

The second model (system_perbox2_sensorgroup.cif) introduces a group definition for each sensor 

The only difference between conveyer.svg and ../conveyer.svg is in the initial position of the products, 
and in the absence of the grey entry and exit rectangles.
The conveyer drawing in this directory positions all products at the same (initial) position, before the first conveyer.