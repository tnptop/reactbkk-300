# State Management
> "It Depends" - Greatest Consultant Ever
> Deeply understand the problem you're solving to properly architect the code

## Information Articulation
> Google vs. Zendesk vs. Facebook
- one and only one thing
- one thing with little distraction
- lots of things at once

## Data Flow
- Engineering from the design (UI/UX)
- Architecture from amount/boundary of data
- Globally vs. Locality
  - Pass all data through parents vs. Give minimum data to each components

## Redux vs. MobX vs. Vanilla
- Global -> Local
- ! Most application fits inbetween globally and locality
  - Redux does not suit that kind of app well