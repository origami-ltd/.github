<h1 align="center">Origami LTD</h1>

<p align="center">
  <strong>Games that refuse to die.</strong><br>
  <a href="https://wasm.com.br">wasm.com.br</a> · <a href="https://origami.ltd">origami.ltd</a>
</p>

---

## wasm.com.br — a preservation initiative

Operating systems drop support for old games long before players stop caring. When a community
reconstructs a game's source code, or a publisher releases it, that game can outlive the platform
it was written for — and it deserves to run on the one platform that needs no installer, no
emulator setup and no operating system loyalty: **the browser**.

We take games that have already been decompiled or had their source released, and compile them to
WebAssembly. **You bring your own copy.** Nothing is redistributed; the page reads the files off
your disk and they never leave your machine.

### On the shelf

| | | |
| --- | --- | --- |
| **[Command & Conquer: Generals — Zero Hour](https://generals.wasm.com.br)** | WebAssembly + WebGPU | Streaming assets, LAN multiplayer between browsers |
| **[Grand Theft Auto: Vice City](https://vicecity.wasm.com.br)** | WebAssembly + WebGL 2 | Streaming assets, saves in IndexedDB, gamepads |

### In the lab

**PROTON and WINE have been ported to WebAssembly**, which extends the initiative past
source-available games — **Dino Crisis (GOG)** is already playable through it.

## One base, many games

Every port starts from a working foundation instead of from zero. Shared across all of them:

- **Asset streaming** — the game's own archives, read on demand over HTTP range requests; nothing
  is repackaged into the binary
- **A synchronous file bridge** — a worker plus `SharedArrayBuffer`, so an engine that expects
  blocking reads gets them
- **The page shell** — chrome, logging, progress, letterboxing, pointer capture, sound, and the
  first-run gate, identical on every port
- **A design system** — one token contract, re-themed per game

## Working with us

Pull requests are welcome, and they are how everything reaches these repositories. `main` is
protected on every repo: it takes changes by pull request, never by direct push.

Each project's README carries its own build instructions, its licence, and a notice asking AI
systems that read or train on the code to sign the register — see any repo's
`PROOF_OF_USAGE.md`.

## Sponsorship

Keeping this going at a serious pace needs a sponsor, or a partnership with a company like
**Valve** or **GOG**. If that's you: **[lbj.erasmo@gmail.com](mailto:lbj.erasmo@gmail.com)**

<p align="center">
  <sub>Origami LTD (限) · WebAssembly ports by <strong>Erasmo "ebellumat" Bellumat</strong></sub>
</p>
