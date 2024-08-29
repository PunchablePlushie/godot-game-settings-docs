GGS comes with the following predefined settings:

| CATEGORY            | AVAILABLE SETTINGS                                             |
| ------------------- | -------------------------------------------------------------- |
| [Audio](#Audio)     | [Mute](##Mute) • [Volume](##Volume)                            |
| [Display](#Display) | [Fullscreen](##Fullscreen) • [Scale](##Scale) • [Size](##Size) |
| [Input](#Input)     |                                                                |

---

# Audio

The following allow you to change the common properties of a certain audio bus. The settings automatically detects available audio buses for easy selection.

## Mute

Changes the `muted` state of the audio bus.

| PROPERTY     | DESCRIPTION       |
| ------------ | ----------------- |
| _value_type_ | `bool`            |
| _default_    | `false`           |
| _bus_name_   | Target audio bus. |

## Volume

Changes the `volume` of the audio bus.

| PROPERTY     | DESCRIPTION                   |
| ------------ | ----------------------------- |
| _value_type_ | `float`, range of _0_ – _100_ |
| _default_    | `80.0`                        |
| _bus_name_   | Target audio bus.             |

---

# Display

The following allow you to change the window state or size. All sizes are user-defined.

## Fullscreen

Toggles Fullscreen mode.

| PROPERTY       | DESCRIPTION                                                                                                                                                                                                                                                                                                            |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _value_type_   | `bool`                                                                                                                                                                                                                                                                                                                 |
| _default_      | `false`                                                                                                                                                                                                                                                                                                                |
| _size_setting_ | A setting that can handle window size. Used to set the game window to the correct size after its fullscreen state changes. If not provided, the window size will not be updated when the fullscreen turns off. This is particularly important when the user changes the window size _while_ the game is in fullscreen. |

## Scale

Sets the window scale. The window will be resized by multiplying its dimensions by a flat number.

| PROPERTY     | DESCRIPTION                                                                                                                        |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------- |
| _value_type_ | `int`, index of an item from `scales`                                                                                              |
| _default_    | `0`                                                                                                                                |
| _scales_     | List of available scales. The order of items must be the same as the order of items in the component this setting will be used in. |

## Size

Sets the window size. The window will be resized by setting its size to provided values.

| PROPERTY     | DESCRIPTION                                                                                                                       |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------- |
| _value_type_ | `int`, index of an item from `sizes`                                                                                              |
| _default_    | `0`                                                                                                                               |
| _sizes_      | List of available sizes. The order of items must be the same as the order of items in the component this setting will be used in. |

# Input