#main.py- SiaOS
from kivy.app import App
from kivy.uix.button import Button
from kivy.uix. label import Label
from kivy.uix.boxlayout import BoxLayout
from jnius import autoclass

class SiaApp (App)
    def build(self):
        box = BoxLayout (orientation='vertical')
        self.lab = Label (text='Sia0S Ready Say Hey Sia')
        btn = Button(text='START Hey Sia Listener', size_hint_y=0.3)
        btn.bind(on_press=self.start_service)
        box.add_widget(self.lab)
        box.add_widget (btn)
        return box
    def start_service(self, x):
        Service = autoclass('org.test.siaos.ServiceSiaos') 
        Service.start(self.mActivity, '')
        self.lab.text = 'Listening... Say Hey Sia'
SiaApp().run()
