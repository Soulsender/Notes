#fhrp 
### Priority
- determines active router
- default 100 (range 0-255)
- numerically highest IPv4 address is tiebreaker
- once device becomes active router, it will remain active router
### States
- `inital` - state is entered through config change/when interface becomes available
- `learn` - router has not determines virtual IP, has not seen hello message from active router (AR). Router waits to hear from AR.
- `listen` - router knows virtual IP; is not AR or SR. Is listening for hello messages from AR and SR.
- `speak` - router sends periodic hello messages, participates in election
- `standby` - router is candidate to become next AR
- `active` - router is AR