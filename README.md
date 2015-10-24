This is an example to realize some ideas of "actors model" at the Frontend. Each variable region may be present as separate Backbone model (and View - use your favorite render). I think it looks as React/Flux, but the main idea is to build common Message Bus between frontend actors and backend actors.

In this example you can see some events in frontend backbone ("radio") bus. The next step is to forward them to websocket gate to actors-based application on the backend, and to forward backend events through websocket back to our backbone bus.

In the result we want to achieve two-way exchange of messages (events) between backend actors and frontend models/regions.
