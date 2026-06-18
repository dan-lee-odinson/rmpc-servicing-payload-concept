# Concept Brief — Robotic Servicing Validation Payload

> Working draft. Everything here is preliminary and will be refined by the team against the official RMPC technical guidelines, spacecraft interface requirements, and safety rules.

## One-line summary

A compact, ORU-style (Orbital Replacement Unit) robotic servicing validation payload that demonstrates **repeatable, observable robotic manipulation tasks** in low Earth orbit.

## Why this concept

Future spacecraft and orbital platforms will need to be serviceable, modular, inspectable, and upgradeable. In-space servicing, assembly, and manufacturing (ISAM) is the broad infrastructure push behind this. A focused, low-complexity payload that a robotic arm can grapple, move, reseat, and inspect is a credible, demonstrable step toward that future — and it keeps scope realistic for a small first-time team.

## Target capabilities (demonstration tasks)

| # | Task | What it shows |
| --- | --- | --- |
| 1 | Robotic grapple and release | Basic manipulability and a standard interface |
| 2 | Payload relocation | Controlled move between two known positions |
| 3 | Alignment verification | Closing position/orientation tolerance |
| 4 | Reinstallation / reseating | Repeatable mate into a receptacle |
| 5 | Visual fiducial inspection support | Machine-readable targets for vision systems |
| 6 | Simple power/data validation | Confirming a connection after a mate |
| 7 | Repeatable manipulation cycles | Reliability across multiple attempts |
| 8 | Telemetry / observable success criteria | Measurable, reportable pass/fail |

## Design principles

- **Low complexity first.** Prefer passive features, simple interfaces, and clear pass/fail criteria over mechanisms.
- **Observable success.** Every task should produce data or imagery that proves it happened.
- **Interface-driven.** The grapple feature, fiducials, and any connectors should match (or clearly map to) the host arm and spacecraft interface requirements in the official guidelines.
- **Budget-aware.** Mass, power, thermal, and volume are hard constraints — track them from day one.

## Open questions for the team

- What grapple/interface standard does the host system expect?
- What are the mass / volume / power / thermal envelopes from the technical guidelines?
- What fiducial scheme (e.g. ArUco/AprilTag-style) is compatible with the host vision system?
- What counts as a "successful" manipulation cycle for evaluation purposes?
- What environmental qualification (vibration, thermal/vacuum) is required, and who can run it?

## Explicit non-goals (for now)

- No propulsion, no free-flying maneuvers.
- No crewed interaction.
- No high-rate mechanisms or deployables unless a clear case emerges.

*All of the above is subject to the official RMPC technical guidelines, evaluation criteria, and rules.*
