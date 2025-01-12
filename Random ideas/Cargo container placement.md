Placing cargo containers on ships is hard, you have to:
+ balance left and right side of the ship
+ balance front and back of the ship
+ can't have too much weight on the top
+ can't have too much weight on a specific row
+ must place containers that require power (i.e. refrigerated) near outlets
+ cannot place certain chemicals too close to each other
+ cannot place explosives near almost anything
+ cannot place flammables and explosives near the edges if you are about to traverse waters where there may be pirates
+ optimize for minimum number of unnecessary crane lifts when the ship is being unloaded partially (the container you need is under one or more you don't need)
+ optimize for availability (the container you would like to load first is under many others at the port)
+ maybe partial loads/reloads?

this feels like some sort of minimization problem where some things have a weight of +inf, while others have other degrees of importance, merged with some problem of choosing some sort of formal language to specify the requisites in a flexible yet precise way