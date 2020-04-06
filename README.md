# Как переопределить постоянные ссылки для VST вручную через XML (How to override generic link manually via XML)

## Пример файла с постоянными ссылками

```xml
<?xml version="1.0"?>
<flcontrolmap version="1">
  <link>
    <ctrlparam>13</ctrlparam>
    <window><![CDATA[Fruity Wrapper - SH-101]]></window>
    <windowparam>0</windowparam>
    <windowid>3</windowid>
    <channel>0</channel>
    <smoothing>0</smoothing>
    <smoothspeed>469</smoothspeed>
  </link>
</flcontrolmap>
```

`ctrlparam` - это айдишник контрола миди-контроллера
`window` - это имя VST-плагина
`windowparam` - это айдишник контрола у вст-плагина
`windowid` - это айдишник плагина внутри студии

## Айдишники контролов на Korg Nanokontrol (v1)
![korg_map](./map.png)

## Айдишники VST (SH-101)
![korg_map](./map-vst.png)

## SH-101 VST MIDI-CC
#### VCF
- CC3 = VCF_FREQ
- CC9 = VCF_RES
- CC81 = VCF_ENV
- CC82 = VCF_KYBD
- CC83 = VCF_A
- CC84 = VCF_D
- CC85 = VCF_S
- CC86 = VCF_R

#### BOTTOM
- CC5 = PORTAMENTO_TIME
- CC41 = BEND_RANGE
- CC110 = VOLUME
- CC116 = MODE

#### EFFECTS
- CC12 = EFFECTS_CRUSHER
- CC13 = EFFECTS_TIME
- CC91 = EFFECTS_REVERB
- CC94 = EFFECTS_DELAY

#### SOURCE_MIXER (1 to 5 == FROM LEFT TO RIGHT)
- CC16 = SOURCE_MIXER_1
- CC17 = SOURCE_MIXER_2
- CC18 = SOURCE_MIXER_3
- CC113 = SOURCE_MIXER_4
- CC19 = SOURCE_MIXER_5

#### MODULATOR
- CC26 = MODULATOR_VCO
- CC28 = MODULATOR_VCF
- CC29 = MODULATOR_RATE
- CC35 = MODULATOR_WAVEFORM

#### VCO
- CC47 = VCO_DIGITS
- CC50 = VCO_PULSEWIDTH
- CC60 = VCO_MOD

#### VCA
- CC69 = VCA_TONE
- CC89 = VCA_A
- CC90 = VCA_D
- CC96 = VCA_S
- CC97 = VCA_R
- CC117 = VCA_ENV_TRIG
- CC119 = VCA_MODE
