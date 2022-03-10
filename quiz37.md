```.py
Screen:
    MDBoxLayout:
        orientation: "horizontal"
        size_hint: 1, 1
        pos_hint: {'center_x': 0.5, 'center_y': 0.5}

        MDTextField:
            id: USD
            hint_text: "USD"
            font_size: "32pt"
            size_hint: .15, .20

        MDRaisedButton:
            size_hint: .21, .25
            halign: "center"
            text: "Convert"
            font_size: "32pt"
            md_bg_color: 1, 0, 0, 1

        MDTextField:
            id: YEN
            hint_text: "YEN"
            font_size: "32pt"
            size_hint: .15, .20
            
from kivy.lang import Builder
from kivymd.app import MDApp

class quiz37(MDApp):
    def build(self):
        return

quiz37().run()
```
