Conveyor models with algebraic variables for sensors

Controller can be selected by means of import.
Two types are available:
- ../C1  (low throughput)
- ../C2  (high throughput)

The version with the high throughput leads to incorrect behavior for initialization with init_4_3.cif.
This incorrect behavior is only visible directly after starting up when the first box leaves the first conveyer.

Note:
====
Plotting sensors gives non-straight edges, especially when the non-real-time mode
is used (simulation as fast as possible), because then time steps are
usually bigger than in real-time mode (where you have usually 20 or more frames per second).
The time point that the sensor becomes active is precisely determined
by the root finding algorithm,
but the time point immediately before the root is used only in the
root finding algorithm, and not sent to the output.

Remedy: plot more frames, e.g. by using real-time option.
