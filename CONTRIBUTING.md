# Contributing

This guide was written from a single lamp, so the most useful contribution is
a report from another one.

## Board reports

If you open your lamp and the board differs from the
[photo](images/lamp-board.jpg), or you finish the mod and it works, open a
**Board report** issue with a photo. Wire colours, colour order and board
markings from other units all help the next person.

## Fixes and improvements

Pull requests are welcome for:

- corrections to the guide;
- config changes that keep the default behaviour for existing builds;
- new effects.

Before opening one:

1. Copy `secrets.yaml.example` to `secrets.yaml` and fill it in.
2. Run `esphome config projection-lamp.yaml` and `esphome compile projection-lamp.yaml`.
   The same two commands run in CI on every pull request that touches the config.
3. If the change affects hardware behaviour, say whether you tested it on a
   real lamp.

Never commit `secrets.yaml`. It is git-ignored; keep it that way.

## Questions

For general ESPHome or Home Assistant help, the
[Home Assistant community forum](https://community.home-assistant.io/c/esphome/)
is the better place. Open an issue here when the problem is specific to this
lamp or this config.
