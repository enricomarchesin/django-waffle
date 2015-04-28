.. _starting-autocreation:

==========================
Autocreation with defaults
==========================

It is possible to autocreate flags. For flags, switches and samples there are
the respective ``WAFFLE_FLAG_AUTOCREATE``, ``WAFFLE_SWITCH_AUTOCREATE`` and
``WAFFLE_SAMPLE_DEFAULTS``. 

``WAFFLE_FLAG_AUTOCREATE``:
    Whether new Flags will be created automatically when used. Defaults to
    ``False``.

``WAFFLE_FLAG_DEFAULTS``:
    A dictionary of defaults for flags. Defaults to ``{}``. below.

``WAFFLE_SWITCH_AUTOCREATE``:
    Whether new Switches will be created automatically when used. Defaults to
    ``False``.

``WAFFLE_SWITCH_DEFAULTS``:
    A dictionary of defaults for flags. Defaults to ``{}``. below.

``WAFFLE_SAMPLE_AUTOCREATE``:
    Whether new Samples will be created automatically when used. Defaults to
    ``False``.

``WAFFLE_SAMPLE_DEFAULTS``:
    A dictionary of defaults for flags. Defaults to ``{}``. See below.


For each type, there's also a defaults settings.
For example for samples:
```
    WAFFLE_SAMPLE_DEFAULTS = {
        'special_sample': {
            'percent': Decimal(0.15)
        }
    }
```
It is a dictionary where every key is the name and value a dictionary with
model field defaults.
