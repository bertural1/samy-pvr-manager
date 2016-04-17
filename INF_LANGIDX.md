# LANGIDX #

The bytes at 0x1D24 and 0x1D25 is the index (little endian) of the Language string in the list of translated strings. For example, if your TV is configured in English and the values at 0x1D24 and 0x1D25 are 0x14 and 0x02 (0x0214), then the language string displayed by the TV is "English". With the values 0x16 and 0x02 (0x0216), the text is "French". When you change the language of the menus with the settings of the TV to French, the same values point to "Anglais" and "Français". (_T4P rol_)

# Details #

Language indexes:

  * 0213 Korean
  * 0214 English
  * 0215 Spanish
  * 0216 French
  * 0217 Japanese
  * 0218 T-Chinese
  * 0219 Chinese
  * 021A S-Chinese
  * 021B German
  * 021C Italian
  * 021D Russian
  * 021E Dutch
  * 021F Portugese
  * 0220 Swedish
  * 0221 Bulgarian
  * 0222 Croatian
  * 0223 Czech
  * 0224 Greek
  * 0225 Hungarian
  * 0226 Polish
  * 0227 Romanian
  * 0228 Turkish
  * 0229 Danish
  * 022A Finnish
  * 022B Norwegian
  * 022C Serbian
  * 022D Welsh
  * 022E Gaelic
  * 022F Irish
  * 0230 Slovakian
  * 0231 Catalan
  * 0232 Valencian
  * 0233 Maori
  * 0234 Mandarin
  * 0235 Cantonese
  * 0236 Hindi
  * 0269 Latvian
  * 026A Lithuanian
  * 026B Basque
  * 026C Galicean
  * 026D Estonian
  * 026E Arabic
  * 026F Hebrew
  * 0270 Afrikaans
  * 0271 Amharic
  * 0272 Hansa
  * 0273 Igbo
  * 0274 Swahili
  * 0275 Xhosa
  * 0276 Yoruba
  * 0277 Zulu
  * 0278 Indonesian
  * 0279 Thai
  * 027A Vietnamese
  * 02FA Canadian French

Special Language indexes:

  * 020A Multi
  * 023D bilingual
  * 0237 V.O.