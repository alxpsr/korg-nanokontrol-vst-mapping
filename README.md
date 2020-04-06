# Пример файла с постоянными сслыками

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

# Айдишники контролов на Korg Nanokontrol (v1)
![korg_map](./map.png)

# Айдишники VST (SH-101)
![korg_map](./map-vst.png)


How to override generic link manually via XML
