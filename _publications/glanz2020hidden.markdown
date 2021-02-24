---
layout: publication
title: Hidden in Plain Sight: Obfuscated Strings Threatening Your Privacy
authors: Leonid Glanz, Patrick Müller, Lars Baumgärtner, Michael Reif, Sven Amann, Pauline Anthonysamy, Mira Mezini
conference: ASIACCS
year: 2020
bibkey: glanz2020hidden
additional_links:
   - {name: "Paper", url: "https://dl.acm.org/doi/pdf/10.1145/3320269.3384745"}
   - {name: "code", url: "https://github.com/stg-tud/StringHound"}
tags: ["string (de-)obfuscation", "Android apps", "slicing"]
---
String obfuscation is an established technique used by proprietary, closed-source applications to protect intellectual property. Further-more, it is also frequently used to hide spyware or malware in applications. In both cases, the techniques range from bit-manipulation over XOR operations to AES encryption. However, string obfuscation techniques/tools suffer from one shared weakness: They generally have to embed the necessary logic to deobfuscate strings into the app code. In this paper, we show that most of the string obfuscation techniques found in malicious and benign applications for Android can easily be broken in an automated fashion. We developed StringHound, an open-source tool that uses novel techniques that identify obfuscated strings and reconstruct the originals using slicing. We evaluated StringHound on both benign and malicious Android apps. In summary, we deobfuscate almost 30 times more obfuscated strings than other string deobfuscation tools. Additionally, we analyzed 100,000 Google Play Store apps and found multiple obfuscated strings that hide vulnerable cryptographic usages, insecure internet accesses, API keys, hard-coded passwords, and exploitation of privileges without the awareness of the developer. Furthermore, our analysis reveals that not only malware uses string obfuscation but also benign apps make extensive use of string obfuscation.