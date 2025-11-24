# OpenCore Hackintosh EFI for Lenovo IdeaPad 3 17IIL05
*Basé sur le chargeur de démarrage OpenCore, issu directement du projet officiel [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg) développé par [acidanthera](https://github.com/acidanthera) hébergé sur GitHub. Tout a été configuré de A à Z en suivant scrupuleusement le [Guide d’installation OpenCore de Dortania](https://dortania.github.io/OpenCore-Install-Guide/) afin d’obtenir la meilleure stabilité et compatibilité possible ! Si mon travail vous est utile, n’hésitez pas à me soutenir sur [Ko-Fi](https://ko-fi.com/duncanlangrume74395)❤️*

**AVERTISSEMENT/DISCLAIMER (TRÈS IMPORTANT)**: Cette EFI prend uniquement en charge macOS Big Sur (11) jusqu’à macOS Sequoia (15) inclus!


# Prérequis
Pour que le Wi-Fi fonctionne correctement sous **macOS Sequoia (15)** : Tu **DOIS** absolument télécharger et installer **HeliPort** (.dmg) depuis le dépôt officiel : https://github.com/OpenIntelWireless/HeliPort. Il est également **fortement recommandé** d’installer la dernière version de [YogaSMC](https://github.com/zhen-zen/YogaSMC/releases/latest) afin d’avoir les informations de batterie, le contrôle des ventilateurs et d’autres fonctions utiles. Après avoir ouvert le fichier **YogaSMC-App-Release.dmg**, double-clique sur **YogaSMCPane.prefPane** pour l’installer dans les Préférences Système, puis glisse-dépose **YogaSMCNC.app** dans le dossier **Applications**.

## Spécifications/Specs

![A Propos](images/system-inf.png) 

| | |
|-|-|
|**CPU**|Intel® Core™ i3-1005G1 Processor @ 1.2GHz (Ice Lake)|
|**RAM**|8GB DDR4 3200MHz|
|**iGPU**|Intel® UHD Graphics G1|
|**SSD**|NVMe M.2 SKHynix-HFM512GDHTNI-87A0B 512GB SSD|
|**WLAN+BT**|Intel® Wireless-AC 9560 (Une carte BCM nativement supportée par macOS sera beaucoup plus stable)|
|**Audio**|Realtek ALC230|
|**Ports**|2xUSB3.0, 1xUSB2.0, HDMI (ne fonctionne absolument pas sur les appareils Ice Lake), lecteur de carte SD, prise casque/micro, et port de charge DC|
|**OpenCore Bootloader**|V1.0.1 MOD (Cette EFI sera mise à jour en continu, kexts et pilotes inclus. Il te suffira de revenir dans un mois environ et de vérifier soit un commit du type « Updated OpenCore to X.X.X MOD ! », soit tout simplement la dernière release !)

## Non fonctionnel

- HDMI (probablement jamais réparable. NB : ce problème est exclusif aux processeurs Ice Lake)
- Hibernation (aucun souci, je l’ai désactivée dans OpenCore)
- Tu me diras si tu trouves autre chose ?!

## Fonctionnel
- **Tout le reste qui n’est pas dans la section « Non fonctionnel » :D**
- Bluetooth (fonctionne nativement sur toutes les versions de macOS)
- Wi-Fi (fonctionne nativement sur tous les macOS sauf Sequoia → voir [cette section](#prequisites) pour la correction ultra-simple sous macOS Sequoia 15)
- Ports USB mappés précisément (fonctionnent même après veille)
- Touchpad ELAN Precision HID avec gestes entièrement opérationnels
- Audio (et ses touches de raccourcis) : haut-parleurs, micro interne et prise casque/micro
- Accélération graphique complète (QE/CI)
- Veille / réveil
- Lecteur de cartes SDHC/SDXC
- Luminosité (et ses touches de raccourcis)

## Conclusion

J’espère que cette EFI te permettra d’avoir un Hackintosh sans prise de tête.
S’il reste des soucis, les pull requests et les suggestions sont les bienvenus ! :)
Voici le forum officiel où mon EFI a toujours été hébergée si tu veux un autre moyen de contact !
