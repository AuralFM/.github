# AuralFM

**Radio chosen by people. Found by place.**

A globe you listen to. Spin the Earth, pick a place, and hear what is on the
air there right now: 60,000 live radio stations in 12,000 places, and shortwave
through public receivers that people leave open for anyone to borrow.

- **Listen:** [listen.auralfm.xyz](https://listen.auralfm.xyz), in any browser.
  On an iPhone, add it to the Home Screen and it opens like an app.
- **Mac:** in beta.
- **About:** [auralfm.xyz](https://auralfm.xyz) ·
  **Docs:** [docs.auralfm.xyz](https://docs.auralfm.xyz)

Free, with no advertising.

## What it stands for

- **Chosen by people.** Every station is programmed by the people who run it.
  Nothing you hear was picked by a machine.
- **No algorithm.** Nothing is ranked or recommended, and nobody can pay to be
  heard. Nothing about what you play is kept.
- **The underground, at full size.** A community station gets the same dot as a
  national one.
- **Nobody in the middle.** Each station plays from its own server, straight to
  you. No account to listen.

---

## If you run a station

Your station is on the globe because it is on the air. You can correct it,
remove it, or claim its page and add your own donation link:
[docs.auralfm.xyz/stations](https://docs.auralfm.xyz/stations/).

Or write to **hello@auralfm.xyz** and say which station. Removal needs no
reason.

---

## If you run a KiwiSDR and found this in your logs

Connections from the app identify themselves:

```
User-Agent: AuralFM/0.1.0
```

**A connection only ever happens because a person clicked your receiver.** The
app does not scan, does not probe, and does not connect to anything on its own.

What it will never do:

- **Connect on its own.** No background checks, no availability polls.
- **Hold more than one receiver at a time**, anywhere in the app.
- **Retry a receiver that refused it.** If you are full, it offers a different one.
- **Fight your timeouts.** If you drop it, it stays dropped.
- **Squat a slot.** If somebody pauses and walks away, the connection closes
  after ninety seconds, not the thirty minutes your Kiwi would allow.

**Where the list comes from:** the same public list everyone else reads,
`rx.linkfanel.net/kiwisdr_com.js`. A list ships inside the app, and the app
reads the public one again at most twice a day: one request, to one aggregator,
for the whole list. Never to your machine.

### If you would rather not be included

**Ask, and you are out. No reason needed.** Open an issue here, or write to
hello@auralfm.xyz, and say which host.

You are left out when the app's list is built, so the next version of the app
never learns you existed. The app's own refresh cannot add you back: it only
updates receivers that were in the list it shipped with. No list of who opted
out sits inside anybody's software.

**You should not have to firewall us to make it stop.** That costs you work,
and costs every other listener your receiver.

### If something is wrong

If the app has misbehaved (connected when it should not have, held a slot,
hammered you), that is a bug, and the logs you already have are the evidence.
Send them.

This project took three receivers offline in the past through careless probing
during development. That is why the rules above are written down and checked by
the build, and why the app says its own name instead of arriving as a browser.

---

## Contact

**hello@auralfm.xyz** for everything: stations, receivers, problems, press.

- Copyright notices: see the [Terms](https://docs.auralfm.xyz/terms/).
- Security problems: write to the same address. Please do not open a public issue.

The application source is not public yet. These commitments are, and they are
the ones that affect you.
