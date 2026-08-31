# Home Assistant Motion Light Blueprints

Reusable Home Assistant blueprints for motion-controlled lights.

`motion_light_auto_ownership.yaml` uses an `input_boolean` ownership flag so
only lights switched on by the automation are automatically switched off.
It supports separate guard lights and target lights for cases where an area
must be dark before only a subset of its lights is switched on. Turn-off
commands are retried up to three times; the ownership flag clears only after
all controlled lights report off.
