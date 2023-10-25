# Voice chat
Plugin Simple Voice chat nám umožňuje hlasovou komunikaci mezi hráči, aby mohl hráč voice chat využívat, je nutné aby měl nainstalovaný mod ve svém klientovi, jinak to nebude fungovat. Vše si v tomhle návodu ukážeme.

## Server
Jako první stáhneme plugin [zde](https://www.curseforge.com/minecraft/bukkit-plugins/simple-voice-chat/files/all) (Pozor na stáhnutí správného pluginu, podle vaší verze. 😄), až se nám plugin stáhne, nahrajeme ho přes správce souborů nebo (S)FTP na náš server do složky **plugins** a server restartujeme. Po restartu se nám ve složce **plugins** vytvoří složka se jménem "voicechat", složku otevřeme a následně i konfigurační soubor **voicechat-server.properties**. V souboru je důležité upravit port, použijeme jeden z volných portů (Pokud nám žádné porty nebyly přiděleny, kontaktujeme správce hostingu), ostatní položky upravovat nemusíme.
```
#
#Sat Jul 1 00:00:00 UTC 2000
min_voice_distance=4.0
broadcast_range=-1.0
spectator_interaction=false
force_voice_chat=false
bind_address=
open_groups=false
whisper_distance_multiplier=0.5
codec=VOIP
allow_recording=true
max_voice_distance=48.0
port=24454                        <- zde upravíme port
crouch_distance_multiplier=1.0
mtu_size=1024
voice_host=
keep_alive=1000
login_timeout=10000
spectator_player_possession=false
enable_groups=true
```
Soubor po změnění portu uložíme a následně server opět restartujeme.


## Klient
Abychom mohli nainstalovat danný mód, musíme mít nainstalovaný v klientu Forge nebo Fabric, my doporučujeme Fabric, který stáhneme [zde](https://fabricmc.net/use/installer/) a poté nainstalujeme pro naší verzi. Po nainstalování stáhneme mód do klienta [zde](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat/files/all). Stažený mód nahrajeme do složky **mods**, kterou nalezneme v **.minecraft**.
