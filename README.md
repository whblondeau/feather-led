# feather-led
An extremely lightweight remote monitoring system for unix CLI servers.

feather-led is a simple system. It's not a 100% solution; it's not even intended as a pareto 80% solution. It's minimalist all the way.

feather-led consists of two sets of simple behavioral specifications:
 - The **client**, a CLI utility which conducts measurements and maintains a log of measurement history;
 - The **display**, which is a server that communicates with clients and provides two representations of the client information:
  - at-a-glance summary display, by default color-coded but modifiable to accommodate non-color representation;
  - drill-down capability to expose the detail and / or historical information underneath the summary.

This repository will provide the specifications, and an implementation using Python and Flask for the display.
