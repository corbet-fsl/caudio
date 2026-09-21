# caudio

Semantic PipeWire control plane for local and network audio devices:
a D-Bus daemon over `pw-dump`/`pw-link`/`wpctl` (`src/graph.rs`,
`src/fabric.rs`), a `ksni` tray, and an operator CLI — with an
integration harness (`tests/daemon.rs`) that runs a real daemon against
a fake PipeWire and a fake JackTrip.

Origin: extracted with full history from
`corbet-nix/nixaudio-corbet-ch` (crate `nixaudio` 0.2.0). The NixOS
modules, JackTrip packaging, and host wiring stay in that repository;
this one owns the reusable mechanism. Crate and binary identifiers are
unchanged in this move; any rename is a separate, explicitly reviewed
change.

## Licence

Outbound licence is FSL-1.1-ALv2 (converts to Apache-2.0 two years after
each release). See `LICENSE.md` and `LICENSES/FSL-1.1-ALv2.txt`;
`REUSE.toml` is authoritative for per-path identifiers.

## Contributing

Default instructions are in the organization health files. External
contributions must carry the CLA affirmation against
[`cla-v1.0`](https://github.com/corbet-libs/.github/blob/cla-v1.0/CLA.md).
