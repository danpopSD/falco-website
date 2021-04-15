---
title: ആമുഖം
description: ഫാൽക്കോയ്‌ക്ക് ആമുഖം
weight: 2
---
ഒരു പ്രാദേശിക മെഷീൻ, ക്ലൗഡ്, നിയന്ത്രിത കുബേർനെറ്റ്സ് ക്ലസ്റ്റർ അല്ലെങ്കിൽ IoT & എഡ്ജ് കമ്പ്യൂട്ടിംഗിൽ പ്രവർത്തിക്കുന്ന K3s പോലുള്ള കുബേർനെറ്റ്സ് ക്ലസ്റ്റർ എന്നിവയിൽ നിങ്ങൾക്ക് ഫാൽക്കോയെ വിന്യസിക്കാൻ കഴിയും.

## ഫാൽക്കോ ആർക്കിട്ടെക്ചർ

ലിനക്സ് സിസ്റ്റം കോളുകൾ ഉൾപ്പെടുന്ന ഏത് സ്വഭാവവും ഫാൽകോയ്ക്ക് കണ്ടെത്താനും മുന്നറിയിപ്പ് നൽകാനും കഴിയും. നിർദ്ദിഷ്‌ട സിസ്റ്റം കോളുകൾ, ആർഗ്യുമെന്റുകൾ, കോളിംഗ് പ്രോസസിന്റെ സവിശേഷതകൾ എന്നിവയെ അടിസ്ഥാനമാക്കി ഫാൽകോ അലേർട്ടുകൾ പ്രവർത്തിക്കുന്നു.  ഉപയോക്തൃ സ്ഥലത്തും കേർണൽ സ്ഥലത്തും ഫാൽകോ പ്രവർത്തിക്കുന്നു. സിസ്റ്റം കോളുകളെ ഫാൽക്കോ കേർണൽ മൊഡ്യൂൾ വ്യാഖ്യാനിക്കുന്നു. ഉപയോക്തൃസ്ഥലത്തെ ലൈബ്രറികൾ ഉപയോഗിച്ച് സിസ്‌കോളുകൾ വിശകലനം ചെയ്യുന്നു. ഫാൽകോ നിയമങ്ങൾ കോൺഫിഗർ ചെയ്‌തിരിക്കുന്ന റൂൾസ് എഞ്ചിൻ ഉപയോഗിച്ച് ഇവന്റുകൾ ഫിൽട്ടർ ചെയ്യുന്നു. സിസ്‌ലോഗ്, ഫയലുകൾ, സ്റ്റാൻഡേർഡ് ഔട്ട്പുട്ട്  എന്നിങ്ങനെ കോൺഫിഗർ ചെയ്‌തിരിക്കുന്ന ഔട്ട് പുട്ടുകളിലേക്ക് സംശയാസ്‌പദമായ ഇവന്റുകളെക്കുറിച്ചു  മുന്നറിയിപ്പ് നൽകുന്നു.


![Falco Architecture](/docs/images/falco_architecture.png)
## വിന്യാസം
നിലവിൽ, നിങ്ങൾക്ക് ഇനിപ്പറയുന്നതിലൂടെ ഫാൽക്കോയെ വിന്യസിക്കാൻ കഴിയും:
-  ഒരു ലിനക്സ് ഹോസ്റ്റിൽ ഫാൽക്കോ [ഡൌൺലോഡ്](/docs/getting-started/download) ചെയ്ത് പ്രവർത്തിപ്പിക്കുക. അല്ലെങ്കിൽ ഡ്രൈവർ ഇൻസ്റ്റാൾ ചെയ്തിട്ടുള്ള അടിസ്ഥാന ഹോസ്റ്റിൽ പ്രവർത്തിക്കുന്ന ഒരു കണ്ടെയ്നറിൽ ഫാൽകോ യൂസർസ്പേസ് പ്രോഗ്രാം പ്രവർത്തിപ്പിക്കുക.

-  ഉറവിടത്തിൽ നിന്ന് നിർമ്മിച്ച് [Building](/docs/getting-started/source) ഫാൽകോ ഒരു ലിനക്സ് ഹോസ്റ്റിലോ കണ്ടെയ്നറിലോ പ്രവർത്തിപ്പിക്കുക.