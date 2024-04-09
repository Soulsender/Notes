"How radio waves travel through space."
- absorption occurs
- objects get in the way (buildings, mountains, etc.)
- **ionosphere** - effected by solar winds
- **ionosphere wave** (skip, sky-wave)
- **line of sight** (direct wave, direct path) - literally what it sounds like
- **surface wave** (ground wave) - follows curve of earth
- satellite comms must be higher frequency waves so they do not reflect on ionosphere
- 15 degrees best for longest distance generally
- skips bounce better over water
- lower freqs travel longer distances than higher
- **absorption/inverted scatter is not real**

| Name                     | Description                                                                                                               |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------- |
| Skip distance            | transmitter to nearest point where sky wave returns to eath. Determined by height of ionosphere & angle of waves          |
| Skip zone / dead zone    | Point where no waves will reach (too close to groundwave, too far from skywave)                                           |
| Multihop                 | Can reflect again and cause multihop where waves reflect multiple times (3000km per hop)                                  |
| Path loss                | Waves diminishing over time                                                                                               |
| Multipath                | Waves getting somewhere simultaneously by bouncing or travelling directly                                                 |
| Polarization             | VHF and UHF band antennas must have same polarization as transmitting/receiving **(not caused by parabolic interaction)** |
| Selective fading         | phase differences between radio wave components of same transmission                                                      |
| Solar flux               | Radio energy emitted by sun; index is measure of solar activity that is taken at specific freq                            |
| Critical freq            | Highest frequency where radio is reflect to earth                                                                         |
| Lowest usable freq (LUF) | Lowest freq which will support comms over circuit (tx/rx)                                                                 |
| Maximum freq (MUF)       | Highest freq that will reach destination                                                                                  |
| Scatter                  | weak, distorted signal, above and near MUF                                                                                |
|                          |                                                                                                                           |

### Good & Bad Conditions
- Rain can block radio waves
- Night looses D layer, E layer is diminished, night is better for long range comms
- Sun is out, ionosphere is lower (F, E, D layers), better for short comms
### Ionosphere Layers
- `F > E > D` *(highest to lowest)*
- F layer hangs around
- splits into two (F1 and F2) at daytime
### Solar Activity
- 11-year solar cycle
- coronal mass ejection (CMEs)
	- can shut down electronics
	- influences all radio comms beyond ground way or line of sight
- more sun spots, greater ionization
### Software
- [HamClock](https://www.clearskyinstitute.com/ham/HamClock/)
- [VOACAP](https://www.voacap.com/hf/)
- [WSPR](https://www.arrl.org/wspr)