# RotorCrypt X

Free offline hybrid encryption software for Windows 10/11.
Three cryptographic layers: Enigma rotor logic + AES-256-GCM + HKDF-SHA3-256.
Quantum-resistant. No cloud. No server. No account required.

## 🌐 Website & Download
https://www.bagdadi.de

---

---
---

## 🇩🇪 Deutsch

### Drei kryptografische Schutzebenen

**Ebene 1 – Enigma-Rotormaschine**
RotorCrypt X basiert auf einem fortgeschrittenen Enigma-Rotorprinzip, weit über die historische Maschine hinaus:
- Bis zu **50 konfigurierbare Walzen** (die historische Enigma hatte 3–5)
- Vollständige **Unicode-Unterstützung** – 65.536 mögliche Zeichen statt 26 Buchstaben
- Jede Nachricht erhält eine **vollständig neue, kryptografisch erzeugte Konfiguration**
- Steckbrett und Reflektor werden pro Nachricht neu generiert
- Keine zwei Nachrichten teilen jemals denselben Walzenzustand

**Ebene 2 – AES-256-GCM**
Die Enigma-Ausgabe wird ein zweites Mal mit AES-256 im Galois/Counter-Modus verschlüsselt:
- Militärstandard-Verschlüsselung
- Eingebautes Authentifizierungs-Tag – jede Manipulation wird erkannt und abgelehnt

**Ebene 3 – HKDF-SHA3-256 Schlüsselableitung**
Jede Nachricht erzeugt frische kryptografische Schlüssel:
- **Perfect Forward Secrecy** – ein kompromittierter Schlüssel verrät nichts über vergangene oder zukünftige Nachrichten
- Schlüssel werden abgeleitet, niemals übertragen
- Automatische Schlüsselrotation nach jeder einzelnen Nachricht

### Sicherheitsarchitektur

**Keyfile-System**
Jeder Kontakt besitzt eine eigene Schlüsseldatei, die das Gerät niemals verlässt:
- Echtes Schlüsselmaterial ist von zufälligem Füllmaterial nicht unterscheidbar
- Kein Passwort nötig – Authentifizierung erfolgt über die Schlüsseldatei selbst
- Manipulationen werden sofort erkannt

**Einmaliger Handshake**
Ein einmaliger Handshake etabliert die gemeinsame kryptografische Grundlage:
- Der Handshake wird **genau einmal** pro Kontakt durchgeführt
- Ein farbkodiertes Banner zeigt jederzeit den Sicherheitsstatus
- Nach Abschluss ist der Handshake **kryptografisch gesperrt** und kann nie zurückgesetzt werden
- Danach wird niemals wieder Schlüsselmaterial zwischen den Partnern ausgetauscht

**Replay-Schutz**
Jede Nachricht kann **genau einmal** entschlüsselt werden:
- Eindeutige Nachrichtenzähler verhindern jede Wiederholung
- Doppelte Entschlüsselungsversuche werden sofort blockiert
- Eine klare Warnung erscheint bei erkanntem Replay-Angriff

**Manipulationsschutz**
RotorCrypt X schützt aktiv gegen Reverse Engineering:
- **Anti-Debug-Erkennung** – Analysewerkzeuge werden zur Laufzeit erkannt, das Programm beendet sich sofort
- **EXE-Integritätsprüfung** – jede Veränderung der Programmdatei wird beim Start erkannt
- **Schlüsselvernichtung** – bei erkannter Manipulation werden alle Schlüsseldateien kryptografisch zerstört
- **Kern-Verschleierung** – die Krypto-Engine läuft durch einen proprietären Interpreter; Dekompilierung liefert keinen lesbaren Algorithmus

**Kontaktverifikation**
Jeder Kontakt hat eine verifizierbare kryptografische Identität:
- Kontaktnamen sind verschlüsselt und nur lokal gespeichert
- Grünes Banner = beide Seiten verifiziert, volle Sicherheit aktiv

### Quantensicherheit
- Effektiver Schlüsselraum **2^768** – widersteht dem Grover-Algorithmus
- Selbst mit einem Quantencomputer mit 10^18 Operationen pro Sekunde würde das Knacken länger dauern als das Universum alt ist
- Drei unabhängige Schichten müssen gleichzeitig gebrochen werden

### Änderungen Version 1.8
- Schlüsselraum erhöht auf **2^768** (vorher 2^352)
- Maximale Nachrichtenlänge: **5.951 Zeichen**
- Neu: **Bootstrap-Schutz** – zirkuläre kryptografische Abhängigkeit
- Neu: **Replay-Schutz** – jede Nachricht nur einmal entschlüsselbar
- Neue Sprachen: **Russisch** und **Portugiesisch**

RotorCrypt X, Enigma, Enigma Maschine, Enigma WWII, Enigma Zweiter Weltkrieg, Enigma Verschlüsselung, Enigma knacken, Bletchley Park, Alan Turing, Gordon Welchman, Marian Rejewski, Bomba kryptologiczna, Bombe Maschine, Ultra Geheimnis, Operation Ultra, Wehrmacht Chiffre, Kriegsmarine Enigma, Luftwaffe Verschlüsselung, U-Boot Kommunikation, Funkschlüssel, Schlüsselmaschine, Lorenz SZ42, Colossus Computer, Codebreaking, Kryptanalyse Geschichte, Zygalski Lochblätter, Rotorchiffre, polyalphabetische Substitution, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, Galois Counter Mode, AEAD, authentifizierte Verschlüsselung, Perfect Forward Secrecy, Hybridverschlüsselung, symmetrische Verschlüsselung, asymmetrische Verschlüsselung, Schlüsselableitungsfunktion, KDF, Nonce, Initialisierungsvektor, Stromchiffre, Blockchiffre, Einmalblock, Vernam-Chiffre, Informationstheoretische Sicherheit, Brute-Force-Angriff, Wörterbuchangriff, Rainbow Table, Zero-Knowledge-Beweis, homomorphe Verschlüsselung, Gitterkryptographie, Quantencomputer, Quantenkryptographie, Quantenschlüsselverteilung, QKD, BB84-Protokoll, Quantenverschränkung, Quantenüberlagerung, Qubit, Grover-Algorithmus, Shor-Algorithmus, Post-Quanten-Kryptographie, PQC, NIST Post-Quantum, quantenresistent, quantensicher, 2^768 Schlüsselraum, 768-Bit-Schlüsselraum, Hacken, Hacker, White Hat, Black Hat, Penetrationstest, Red Team, Cybersicherheit, Informationssicherheit, IT-Sicherheit, Zero Trust, Defense in Depth, Man-in-the-Middle, Replay-Angriff, Seitenkanalangriff, Timing-Angriff, Social Engineering, Phishing, Malware, Ransomware, APT, NSA, GCHQ, BND, Überwachung, PRISM, End-to-End-Verschlüsselung, Metadaten, Anonymität, Privatsphäre, Datenschutz, DSGVO, Air-Gap, Hardware Security Module, HSM, Trusted Platform Module, TPM, Chain of Trust, Code Signing, formale Verifikation, beweisbare Sicherheit, IND-CPA, IND-CCA2, Whistleblower, Quellenschutz, Pressefreiheit, Militärverschlüsselung, COMSEC, TEMPEST, Schlüsselmanagement, Sitzungsschlüssel, ephemerer Schlüssel, kostenlose Verschlüsselung, Offline-Verschlüsselung, keine Cloud, kein Server, portabel, USB-Stick, Windows 10, Windows 11, sicherer Messenger, Dateisverschlüsselung, Textverschlüsselung, Keyfile, Handshake-Protokoll, Unicode-Verschlüsselung, 50 Walzen, 65536 Zeichen, 3 Sicherheitsebenen, Shareware, Freeware
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_de.html

---

## 🇬🇧 English

### Three Cryptographic Layers

**Layer 1 – Enigma Rotor Engine**
RotorCrypt X is built on an advanced Enigma rotor principle, far beyond the historical machine:
- Up to **50 configurable rotors** (historical Enigma had 3–5)
- Full **Unicode support** – 65,536 possible characters instead of 26 letters
- Every message gets a **completely new, cryptographically generated configuration**
- Plugboard and reflector are regenerated per message
- No two messages ever share the same rotor state

**Layer 2 – AES-256-GCM**
The Enigma output is encrypted a second time using AES-256 in Galois/Counter Mode:
- Military-grade encryption
- Built-in authentication tag – any manipulation is detected and rejected

**Layer 3 – HKDF-SHA3-256 Key Derivation**
Every message generates fresh cryptographic keys:
- **Perfect Forward Secrecy** – a compromised key reveals nothing about past or future messages
- Keys are derived, never transmitted
- Automatic key rotation after every single message

### Security Architecture

**Keyfile System**
Every contact has a dedicated keyfile that never leaves the device:
- Real key material is indistinguishable from random padding
- No password needed – authentication happens through the keyfile itself
- Tampering is detected immediately

**One-Time Handshake**
A one-time handshake establishes the shared cryptographic foundation:
- Performed **exactly once** per contact
- A color-coded banner shows the security state at all times
- Once complete, the handshake is **cryptographically locked** and can never be reset
- No key material is ever exchanged again after completion

**Replay Protection**
Each message can be decrypted **exactly once**:
- Unique message counters prevent any replay
- Duplicate decryption attempts are blocked immediately
- A clear warning appears when a replay attack is detected

**Tamper Protection**
RotorCrypt X actively defends against reverse engineering:
- **Anti-debug detection** – analysis tools are detected at runtime, program exits immediately
- **Executable integrity check** – any modification to the binary is detected on startup
- **Key destruction** – if tampering is detected, all keyfiles are cryptographically destroyed
- **Core obfuscation** – the crypto engine runs through a proprietary interpreter; decompilation yields no readable algorithm

**Contact Verification**
Every contact has a verifiable cryptographic identity:
- Contact names are encrypted and stored locally only
- Green banner = both sides verified, full security active

### Quantum Resistance
- Effective key space **2^768** – withstands Grover's algorithm
- Even with a quantum computer at 10^18 operations per second, breaking the encryption takes longer than the age of the universe
- Three independent layers must be broken simultaneously

### Changes in Version 1.8
- Key space increased to **2^768** (previously 2^352)
- Maximum message length: **5,951 characters**
- New: **Bootstrap protection** – circular cryptographic dependency
- New: **Replay protection** – each message decryptable exactly once
- New languages: **Russian** and **Portuguese**

RotorCrypt X, Enigma, Enigma machine, Enigma cipher, Enigma WWII, Enigma decoder, Enigma breaker, Bletchley Park, Alan Turing, Gordon Welchman, Marian Rejewski, Bomba kryptologiczna, Bombe machine, Ultra intelligence, Operation Ultra, Wehrmacht cipher, Kriegsmarine Enigma, U-boat communication, rotor machine, Lorenz cipher, Lorenz SZ42, Colossus computer, codebreaking WWII, cryptanalysis history, Zygalski sheets, rotor cipher, polyalphabetic substitution, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, Galois Counter Mode, AEAD, authenticated encryption, Perfect Forward Secrecy, hybrid encryption, symmetric encryption, asymmetric encryption, key derivation function, KDF, nonce, initialization vector, stream cipher, block cipher, one-time pad, Vernam cipher, information theoretic security, brute force attack, dictionary attack, rainbow table, zero-knowledge proof, homomorphic encryption, lattice cryptography, quantum computer, quantum cryptography, quantum key distribution, QKD, BB84 protocol, quantum entanglement, quantum superposition, qubit, Grover algorithm, Shor algorithm, post-quantum cryptography, PQC, NIST post-quantum, quantum-resistant, quantum-safe, 2^768 key space, 768-bit key space, hacking, hacker, white hat, black hat, penetration testing, red team, cybersecurity, information security, IT security, Zero Trust, Defense in Depth, man-in-the-middle, replay attack, side channel attack, timing attack, social engineering, phishing, malware, ransomware, APT, NSA, GCHQ, surveillance, PRISM, end-to-end encryption, metadata, anonymity, privacy, data protection, GDPR, air-gap, HSM, TPM, chain of trust, code signing, formal verification, provable security, IND-CPA, IND-CCA2, whistleblower, source protection, press freedom, military encryption, COMSEC, TEMPEST, key management, session key, ephemeral key, free encryption, offline encryption, no cloud, no server, portable, USB stick, Windows 10, Windows 11, secure messenger, file encryption, text encryption, keyfile, handshake protocol, Unicode encryption, 50 rotors, 65536 characters, 3 security layers, shareware, freeware
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_en.html

---

## 🇫🇷 Français

### Trois couches cryptographiques

**Couche 1 – Moteur à rotors Enigma**
RotorCrypt X repose sur un principe de rotor Enigma avancé, bien au-delà de la machine historique :
- Jusqu'à **50 rotors configurables** (l'Enigma historique en avait 3–5)
- Support **Unicode** complet – 65 536 caractères possibles au lieu de 26 lettres
- Chaque message reçoit une **configuration entièrement nouvelle, générée cryptographiquement**
- Le tableau de connexions et le réflecteur sont régénérés à chaque message
- Aucun message ne partage jamais le même état de rotor

**Couche 2 – AES-256-GCM**
La sortie Enigma est chiffrée une seconde fois avec AES-256 en mode Galois/Compteur :
- Chiffrement de niveau militaire
- Tag d'authentification intégré – toute manipulation est détectée et rejetée

**Couche 3 – Dérivation de clé HKDF-SHA3-256**
Chaque message génère de nouvelles clés cryptographiques :
- **Confidentialité persistante parfaite** – une clé compromise ne révèle rien sur les messages passés ou futurs
- Les clés sont dérivées, jamais transmises
- Rotation automatique des clés après chaque message

### Architecture de sécurité

**Système de fichiers de clés**
Chaque contact possède un fichier de clés dédié qui ne quitte jamais l'appareil :
- Le matériel de clé réel est indiscernable du rembourrage aléatoire
- Aucun mot de passe requis – l'authentification se fait via le fichier de clés
- Toute falsification est détectée immédiatement

**Handshake unique**
Un handshake unique établit la base cryptographique commune :
- Effectué **exactement une fois** par contact
- Une bannière à code couleur indique l'état de sécurité en permanence
- Une fois terminé, le handshake est **verrouillé cryptographiquement** et ne peut jamais être réinitialisé
- Aucun matériel de clé n'est plus jamais échangé après cela

**Protection contre la relecture**
Chaque message ne peut être déchiffré **qu'une seule fois** :
- Des compteurs de messages uniques empêchent toute relecture
- Les tentatives de déchiffrement en double sont immédiatement bloquées

**Protection contre la falsification**
RotorCrypt X défend activement contre l'ingénierie inverse :
- **Détection anti-debug** – les outils d'analyse sont détectés à l'exécution
- **Vérification de l'intégrité de l'exécutable** – toute modification est détectée au démarrage
- **Destruction des clés** – si une falsification est détectée, tous les fichiers de clés sont détruits
- **Obscurcissement du noyau** – le moteur crypto fonctionne via un interpréteur propriétaire

**Résistance quantique**
- Espace de clés effectif **2^768** – résiste à l'algorithme de Grover
- Même avec un ordinateur quantique, le cassage prendrait plus longtemps que l'âge de l'univers
- Trois couches indépendantes doivent être cassées simultanément

Logiciel de chiffrement hors ligne gratuit pour Windows. Chiffre à rotors Enigma + AES-256-GCM + HKDF-SHA3-256. Résistant aux quantiques. Sans cloud. Sans serveur. Portable. Clé USB. machine Enigma, chiffre Enigma, Enigma WWII, Bletchley Park, Alan Turing, Gordon Welchman, Marian Rejewski, Bomba kryptologiczna, machine Bombe, renseignement Ultra, opération Ultra, chiffre Wehrmacht, Enigma Kriegsmarine, machine à rotors, chiffre Lorenz, Colossus, cryptanalyse, feuilles Zygalski, chiffre à rotors, substitution polyalphabétique, SHA-3, Keccak, mode Galois Counter, AEAD, chiffrement authentifié, confidentialité persistante parfaite, chiffrement hybride, ordinateur quantique, cryptographie quantique, algorithme de Grover, algorithme de Shor, cryptographie post-quantique, résistant aux quantiques, espace clé 2^768, hacker, test de pénétration, cybersécurité, Zero Trust, homme du milieu, attaque par rejeu, ingénierie sociale, hameçonnage, logiciel malveillant, rançongiciel, NSA, surveillance, chiffrement de bout en bout, anonymat, vie privée, protection des données, RGPD, chiffrement hors ligne, sans cloud, sans serveur, portable, clé USB, Windows 10, Windows 11, messagerie sécurisée, chiffrement de fichiers, logiciel gratuit
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_fr.html

---

## 🇪🇸 Español

### Tres capas criptográficas

**Capa 1 – Motor de rotores Enigma**
RotorCrypt X se basa en un principio avanzado de rotor Enigma, muy superior a la máquina histórica:
- Hasta **50 rotores configurables** (la Enigma histórica tenía 3–5)
- Soporte **Unicode** completo – 65.536 caracteres posibles en lugar de 26 letras
- Cada mensaje recibe una **configuración completamente nueva, generada criptográficamente**
- El tablero de conexiones y el reflector se regeneran por mensaje
- Ningún mensaje comparte jamás el mismo estado de rotor

**Capa 2 – AES-256-GCM**
La salida Enigma se cifra una segunda vez con AES-256 en modo Galois/Contador:
- Cifrado de grado militar
- Etiqueta de autenticación integrada – cualquier manipulación es detectada y rechazada

**Capa 3 – Derivación de clave HKDF-SHA3-256**
Cada mensaje genera claves criptográficas frescas:
- **Confidencialidad directa perfecta** – una clave comprometida no revela nada sobre mensajes pasados o futuros
- Las claves se derivan, nunca se transmiten
- Rotación automática de claves tras cada mensaje

### Arquitectura de seguridad

**Sistema de archivos de claves**
Cada contacto tiene un archivo de claves dedicado que nunca abandona el dispositivo:
- El material de clave real es indistinguible del relleno aleatorio
- Sin contraseña – la autenticación ocurre mediante el archivo de claves
- Cualquier manipulación es detectada inmediatamente

**Handshake único**
Un handshake único establece la base criptográfica compartida:
- Realizado **exactamente una vez** por contacto
- Un banner con código de colores muestra el estado de seguridad en todo momento
- Una vez completado, el handshake está **bloqueado criptográficamente** y nunca puede restablecerse

**Protección contra repetición**
Cada mensaje puede descifrarse **exactamente una vez**:
- Contadores únicos de mensajes impiden cualquier repetición
- Los intentos de descifrado duplicados se bloquean inmediatamente

**Protección contra manipulaciones**
RotorCrypt X defiende activamente contra la ingeniería inversa:
- **Detección anti-debug** – las herramientas de análisis se detectan en tiempo de ejecución
- **Verificación de integridad del ejecutable** – cualquier modificación se detecta al inicio
- **Destrucción de claves** – si se detecta manipulación, todos los archivos de claves son destruidos
- **Ofuscación del núcleo** – el motor criptográfico funciona a través de un intérprete propietario

**Resistencia cuántica**
- Espacio de claves efectivo **2^768** – resiste el algoritmo de Grover
- Incluso con una computadora cuántica, romper el cifrado tomaría más tiempo que la edad del universo

RotorCrypt X, Enigma, máquina Enigma, cifrado Enigma, Enigma WWII, Bletchley Park, Alan Turing, Gordon Welchman, Marian Rejewski, Bomba kryptologiczna, máquina Bombe, inteligencia Ultra, operación Ultra, cifrado Wehrmacht, Enigma Kriegsmarine, máquina de rotores, cifrado Lorenz, Colossus, criptoanálisis, hojas Zygalski, cifrado de rotores, sustitución polialfabética, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, modo Galois Counter, AEAD, cifrado autenticado, confidencialidad directa perfecta, cifrado híbrido, cifrado simétrico, cifrado asimétrico, función de derivación de clave, KDF, nonce, vector de inicialización, cifrado de flujo, cifrado de bloque, bloc de notas de un solo uso, seguridad teórica de la información, ataque de fuerza bruta, ataque de diccionario, tabla arcoíris, prueba de conocimiento cero, cifrado homomórfico, criptografía de celosía, computadora cuántica, criptografía cuántica, distribución de claves cuánticas, algoritmo de Grover, algoritmo de Shor, criptografía post-cuántica, resistente a cuánticos, espacio de claves 2^768, piratería, hacker, prueba de penetración, ciberseguridad, seguridad de la información, Zero Trust, hombre en el medio, ataque de repetición, ingeniería social, phishing, malware, ransomware, NSA, vigilancia, cifrado de extremo a extremo, anonimato, privacidad, protección de datos, GDPR, módulo de seguridad de hardware, TPM, gestión de claves, cifrado sin conexión, sin nube, sin servidor, portátil, USB, Windows 10, Windows 11, mensajería segura, cifrado de archivos, software gratuito
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_es.html

---

## 🇹🇷 Türkçe

### Üç Kriptografik Katman

**Katman 1 – Enigma Rotor Motoru**
RotorCrypt X, tarihi makinenin çok ötesinde gelişmiş bir Enigma rotor prensibine dayanır:
- **50'ye kadar yapılandırılabilir rotor** (tarihi Enigma 3–5 rotora sahipti)
- Tam **Unicode desteği** – 26 harf yerine 65.536 olası karakter
- Her mesaj **tamamen yeni, kriptografik olarak oluşturulmuş bir yapılandırma** alır
- Her mesaj için fiş tahtası ve reflektör yeniden oluşturulur
- Hiçbir iki mesaj aynı rotor durumunu paylaşmaz

**Katman 2 – AES-256-GCM**
Enigma çıktısı AES-256 ile Galois/Sayaç modunda ikinci kez şifrelenir:
- Askeri düzeyde şifreleme
- Yerleşik kimlik doğrulama etiketi – her türlü manipülasyon tespit edilir ve reddedilir

**Katman 3 – HKDF-SHA3-256 Anahtar Türetme**
Her mesaj yeni kriptografik anahtarlar oluşturur:
- **Mükemmel İleri Gizlilik** – ele geçirilen bir anahtar geçmiş veya gelecek mesajlar hakkında hiçbir şey ortaya koymaz
- Anahtarlar türetilir, asla iletilmez
- Her mesajdan sonra otomatik anahtar rotasyonu

### Güvenlik Mimarisi

**Anahtar Dosya Sistemi**
Her kişinin cihazı hiç terk etmeyen özel bir anahtar dosyası vardır:
- Gerçek anahtar materyali rastgele dolgudan ayırt edilemez
- Şifre gerekmez – kimlik doğrulama anahtar dosyası aracılığıyla gerçekleşir
- Her türlü kurcalama anında tespit edilir

**Tek Seferlik El Sıkışma**
Tek seferlik bir el sıkışma ortak kriptografik temeli oluşturur:
- Her kişi başına **tam olarak bir kez** gerçekleştirilir
- Renk kodlu bir banner güvenlik durumunu her zaman gösterir
- Tamamlandığında el sıkışma **kriptografik olarak kilitlenir** ve asla sıfırlanamaz

**Yeniden Oynatma Koruması**
Her mesaj **tam olarak bir kez** şifresi çözülebilir:
- Benzersiz mesaj sayaçları her türlü tekrarı önler
- Yinelenen şifre çözme girişimleri anında engellenir

**Kurcalamaya Karşı Koruma**
RotorCrypt X tersine mühendisliğe karşı aktif savunma yapar:
- **Anti-debug tespiti** – analiz araçları çalışma zamanında tespit edilir
- **Yürütülebilir bütünlük kontrolü** – ikili dosyada herhangi bir değişiklik başlangıçta tespit edilir
- **Anahtar imhası** – kurcalama tespit edilirse tüm anahtar dosyaları kriptografik olarak imha edilir
- **Çekirdek gizleme** – kripto motoru tescilli bir yorumlayıcı aracılığıyla çalışır

**Kuantum Direnci**
- Etkin anahtar uzayı **2^768** – Grover algoritmasına dayanır
- Kuantum bilgisayarla bile şifrenin kırılması evrenin yaşından daha uzun sürer

RotorCrypt X, Enigma, Enigma makinesi, Enigma şifresi, Enigma İkinci Dünya Savaşı, Bletchley Park, Alan Turing, Gordon Welchman, Marian Rejewski, Bomba kryptologiczna, Bombe makinesi, Ultra istihbaratı, Wehrmacht şifresi, Enigma Kriegsmarine, rotor makinesi, Lorenz şifresi, Colossus, kriptanaliz, rotor şifresi, polialfabetik ikame, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, Galois Counter modu, AEAD, kimlik doğrulamalı şifreleme, mükemmel ileri gizlilik, hibrit şifreleme, simetrik şifreleme, asimetrik şifreleme, anahtar türetme fonksiyonu, KDF, nonce, başlatma vektörü, akış şifresi, blok şifresi, tek kullanımlık ped, kaba kuvvet saldırısı, sözlük saldırısı, gökkuşağı tablosu, kuantum bilgisayar, kuantum kriptografisi, kuantum anahtar dağıtımı, Grover algoritması, Shor algoritması, kuantum sonrası kriptografi, kuantuma dayanıklı, 2^768 anahtar uzayı, hackleme, hacker, sızma testi, siber güvenlik, bilgi güvenliği, Sıfır Güven, ortadaki adam, sosyal mühendislik, kimlik avı, kötü amaçlı yazılım, fidye yazılımı, NSA, gözetleme, uçtan uca şifreleme, anonimlik, gizlilik, veri koruma, GDPR, donanım güvenlik modülü, TPM, anahtar yönetimi, çevrimdışı şifreleme, bulut yok, sunucu yok, taşınabilir, USB, Windows 10, Windows 11, güvenli mesajlaşma, dosya şifreleme, ücretsiz yazılım
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_tr.html

---

## 🇯🇵 日本語

### 3つの暗号化レイヤー

**レイヤー1 – エニグマローターエンジン**
RotorCrypt Xは、歴史的なマシンをはるかに超えた高度なエニグマローター原理に基づいています：
- 最大**50個の設定可能なローター**（歴史的なエニグマは3〜5個）
- 完全な**Unicode対応** – 26文字ではなく65,536文字
- すべてのメッセージが**完全に新しい、暗号学的に生成された構成**を受け取る
- プラグボードとリフレクターはメッセージごとに再生成
- 2つのメッセージが同じローター状態を共有することはない

**レイヤー2 – AES-256-GCM**
エニグマ出力はGalois/カウンターモードのAES-256で2回目の暗号化：
- 軍事グレードの暗号化
- 組み込み認証タグ – あらゆる改ざんを検出して拒否

**レイヤー3 – HKDF-SHA3-256鍵導出**
すべてのメッセージが新鮮な暗号鍵を生成：
- **完全前方秘匿性** – 侵害された鍵は過去・未来のメッセージを明かさない
- 鍵は導出され、送信されない
- すべてのメッセージの後に自動鍵ローテーション

### セキュリティアーキテクチャ

**鍵ファイルシステム**
各連絡先はデバイスを絶対に離れない専用の鍵ファイルを持つ：
- 本物の鍵素材はランダムなパディングと区別不可能
- パスワード不要 – 鍵ファイルで認証
- 改ざんは即座に検出

**一回限りのハンドシェイク**
一回限りのハンドシェイクが共有暗号基盤を確立：
- 連絡先ごとに**正確に1回**実行
- 色分けされたバナーが常にセキュリティ状態を表示
- 完了後、ハンドシェイクは**暗号学的にロック**されリセット不可能

**リプレイ保護**
各メッセージは**正確に1回**のみ復号可能：
- ユニークなメッセージカウンターがリプレイを防止
- 重複復号試行は即座にブロック

**改ざん保護**
RotorCrypt Xはリバースエンジニアリングを積極的に防御：
- **アンチデバッグ検出** – 解析ツールを実行時に検出
- **実行ファイル整合性チェック** – バイナリの変更を起動時に検出
- **鍵の破棄** – 改ざん検出時にすべての鍵ファイルを暗号学的に破棄
- **コア難読化** – 暗号エンジンは独自インタープリターで実行

**耐量子性**
- 有効な鍵空間**2^768** – グローバーのアルゴリズムに耐える
- 量子コンピューターでも解読は宇宙の年齢より長くかかる

RotorCrypt X, エニグマ, エニグマ暗号機, エニグマ第二次世界大戦, ブレッチリー・パーク, アラン・チューリング, マリアン・レイェフスキ, ボンバ, ボンブ, ウルトラ作戦, ローター暗号機, ローレンツ暗号, コロッサス, 暗号解読, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, 認証付き暗号, 完全前方秘匿性, ハイブリッド暗号, 対称暗号, 非対称暗号, 鍵導出関数, ブロック暗号, ストリーム暗号, 量子コンピュータ, 量子暗号, 量子鍵配送, QKD, グローバーのアルゴリズム, ショアのアルゴリズム, ポスト量子暗号, 量子耐性, 2^768鍵空間, ハッキング, ハッカー, ペネトレーションテスト, サイバーセキュリティ, 情報セキュリティ, ゼロトラスト, 中間者攻撃, ソーシャルエンジニアリング, フィッシング, マルウェア, ランサムウェア, NSA, 監視, エンドツーエンド暗号化, 匿名性, プライバシー, データ保護, GDPR, ハードウェアセキュリティモジュール, TPM, 鍵管理, オフライン暗号化, クラウドなし, サーバーなし, ポータブル, USB, Windows 10, Windows 11, セキュアメッセージング, ファイル暗号化, 無料ソフトウェア
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_ja.html

---

## 🇨🇳 中文

### 三重密码保护层

**第1层 – 恩尼格玛转子引擎**
RotorCrypt X基于先进的恩尼格玛转子原理，远超历史机器：
- 最多**50个可配置转子**（历史上的恩尼格玛有3-5个）
- 完整**Unicode支持** – 65,536个可能字符，而非26个字母
- 每条消息获得**全新的、密码学生成的配置**
- 插线板和反射器每条消息重新生成
- 没有两条消息共享相同的转子状态

**第2层 – AES-256-GCM**
恩尼格玛输出再次使用Galois/计数器模式的AES-256加密：
- 军事级加密
- 内置认证标签 – 任何篡改都会被检测并拒绝

**第3层 – HKDF-SHA3-256密钥派生**
每条消息生成新鲜的密码密钥：
- **完美前向保密** – 泄露的密钥不会泄露过去或未来消息的任何信息
- 密钥被派生，从不传输
- 每条消息后自动密钥轮换

### 安全架构

**密钥文件系统**
每个联系人都有一个专用密钥文件，永远不会离开设备：
- 真实密钥材料与随机填充无法区分
- 无需密码 – 通过密钥文件进行认证
- 任何篡改立即被检测

**一次性握手**
一次性握手建立共享密码基础：
- 每个联系人**恰好执行一次**
- 颜色编码横幅始终显示安全状态
- 完成后，握手**密码学锁定**，永远无法重置

**重放保护**
每条消息只能解密**一次**：
- 唯一消息计数器防止任何重放
- 重复解密尝试立即被阻止

**防篡改保护**
RotorCrypt X积极防御逆向工程：
- **反调试检测** – 在运行时检测分析工具
- **可执行文件完整性检查** – 启动时检测二进制文件的任何修改
- **密钥销毁** – 检测到篡改时，所有密钥文件被密码学销毁
- **核心混淆** – 密码引擎通过专有解释器运行

**量子抵抗**
- 有效密钥空间**2^768** – 抵抗Grover算法
- 即使使用量子计算机，破解加密所需时间也超过宇宙年龄

适用于Windows的免费离线加密软件。Enigma转子密码 + AES-256-GCM + HKDF-SHA3-256。抗量子。无云。无服务器。便携式。USB。恩尼格玛, 恩尼格玛密码机, 恩尼格玛二战, RotorCrypt X, 恩尼格玛, 恩尼格玛密码机, 恩尼格玛二战, 布莱切利公园, 阿兰·图灵, 玛丽安·雷耶夫斯基, 炸弹机, 超级情报, 转子密码机, 洛伦茨密码, 巨像计算机, 密码分析, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, 认证加密, 完美前向保密, 混合加密, 对称加密, 非对称加密, 密钥派生函数, 块密码, 流密码, 量子计算机, 量子密码学, 量子密钥分发, QKD, 格罗弗算法, 肖尔算法, 后量子密码学, 抗量子, 2^768密钥空间, 黑客, 渗透测试, 网络安全, 信息安全, 零信任, 中间人攻击, 社会工程学, 网络钓鱼, 恶意软件, 勒索软件, NSA, 监控, 端到端加密, 匿名性, 隐私, 数据保护, GDPR, 硬件安全模块, TPM, 密钥管理, 离线加密, 无云, 无服务器, 便携式, USB, Windows 10, Windows 11, 安全消息, 文件加密, 免费软件
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_zh.html

---

## 🇸🇦 العربية

### ثلاث طبقات تشفير

**الطبقة 1 – محرك روتور إنجما**
يعتمد RotorCrypt X على مبدأ روتور إنجما متقدم، يتجاوز الآلة التاريخية بكثير:
- ما يصل إلى **50 روتوراً قابلاً للتهيئة** (كانت إنجما التاريخية تحتوي على 3-5)
- دعم **Unicode** الكامل – 65,536 حرفاً محتملاً بدلاً من 26 حرفاً
- كل رسالة تحصل على **تهيئة جديدة كلياً، مولّدة تشفيرياً**
- يتم إعادة توليد لوحة التوصيل والعاكس لكل رسالة
- لا تشترك رسالتان أبداً في نفس حالة الروتور

**الطبقة 2 – AES-256-GCM**
يتم تشفير مخرجات إنجما مرة ثانية باستخدام AES-256 في وضع Galois/Counter:
- تشفير بمستوى عسكري
- علامة مصادقة مدمجة – يتم اكتشاف أي تلاعب ورفضه

**الطبقة 3 – اشتقاق مفتاح HKDF-SHA3-256**
كل رسالة تولد مفاتيح تشفير جديدة:
- **السرية الأمامية المثالية** – مفتاح مخترق لا يكشف شيئاً عن الرسائل الماضية أو المستقبلية
- المفاتيح مشتقة، ليست منقولة أبداً
- تدوير تلقائي للمفاتيح بعد كل رسالة

### بنية الأمان

**نظام ملف المفتاح**
كل جهة اتصال لها ملف مفتاح مخصص لا يغادر الجهاز أبداً:
- مادة المفتاح الحقيقية غير قابلة للتمييز عن الحشو العشوائي
- لا يلزم كلمة مرور – تتم المصادقة عبر ملف المفتاح
- يتم اكتشاف أي تلاعب فوراً

**المصافحة لمرة واحدة**
تُنشئ مصافحة لمرة واحدة الأساس التشفيري المشترك:
- تُجرى **مرة واحدة بالضبط** لكل جهة اتصال
- لافتة مرمزة بالألوان تُظهر حالة الأمان دائماً
- عند الاكتمال، تُقفل المصافحة **تشفيرياً** ولا يمكن إعادة تعيينها أبداً

**حماية إعادة التشغيل**
يمكن فك تشفير كل رسالة **مرة واحدة فقط**:
- عدادات رسائل فريدة تمنع أي إعادة تشغيل
- محاولات فك التشفير المكررة تُحجب فوراً

**حماية من التلاعب**
يدافع RotorCrypt X بنشاط ضد الهندسة العكسية:
- **كشف مضاد للتصحيح** – أدوات التحليل مكتشفة في وقت التشغيل
- **فحص سلامة الملف التنفيذي** – أي تعديل مكتشف عند بدء التشغيل
- **إتلاف المفاتيح** – عند اكتشاف التلاعب، تُتلف جميع ملفات المفاتيح تشفيرياً
- **تعتيم النواة** – محرك التشفير يعمل عبر مُفسِّر خاص

**مقاومة الكم**
- فضاء مفاتيح فعّال **2^768** – يقاوم خوارزمية غروفر
- حتى مع حاسوب كمومي، سيستغرق كسر التشفير وقتاً أطول من عمر الكون

RotorCrypt X, إنجما, آلة التشفير إنجما, إنجما الحرب العالمية الثانية, بليتشلي بارك, آلان تورينج, ماريان ريجيوسكي, آلة بومبا, استخبارات ألترا, عملية ألترا, آلة التشفير الدوارة, شيفرة لورنز, كولوسوس, تحليل الشفرات, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, تشفير موثق, السرية الأمامية المثالية, تشفير هجين, تشفير متماثل, تشفير غير متماثل, دالة اشتقاق المفتاح, تشفير الكتلة, تشفير التدفق, الحوسبة الكمية, التشفير الكمي, توزيع المفاتيح الكمية, QKD, خوارزمية غروفر, خوارزمية شور, تشفير ما بعد الكم, مقاوم للكم, فضاء مفاتيح 2^768, اختراق, هاكر, اختبار الاختراق, الأمن السيبراني, أمن المعلومات, الثقة الصفرية, هجوم الوسيط, هندسة اجتماعية, تصيد احتيالي, برامج ضارة, برامج الفدية, وكالة الأمن القومي, مراقبة, تشفير من طرف إلى طرف, إخفاء الهوية, الخصوصية, حماية البيانات, GDPR, وحدة أمان الأجهزة, TPM, إدارة المفاتيح, تشفير غير متصل, بدون سحابة, بدون خادم, محمول, USB, Windows 10, Windows 11, رسائل آمنة, تشفير الملفات, برنامج مجاني
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_ar.html

---

## 🇷🇺 Русский

### Три криптографических уровня

**Уровень 1 – Роторный механизм Энигмы**
RotorCrypt X основан на расширенном принципе ротора Энигмы, далеко превосходящем историческую машину:
- До **50 настраиваемых роторов** (историческая Энигма имела 3–5)
- Полная поддержка **Unicode** – 65 536 возможных символов вместо 26 букв
- Каждое сообщение получает **полностью новую, криптографически сгенерированную конфигурацию**
- Коммутационная панель и рефлектор заново генерируются для каждого сообщения
- Никакие два сообщения не используют одинаковое состояние ротора

**Уровень 2 – AES-256-GCM**
Выход Энигмы шифруется второй раз с помощью AES-256 в режиме Галуа/Счётчика:
- Шифрование военного уровня
- Встроенный тег аутентификации – любое вмешательство обнаруживается и отклоняется

**Уровень 3 – Получение ключа HKDF-SHA3-256**
Каждое сообщение генерирует новые криптографические ключи:
- **Совершенная прямая секретность** – скомпрометированный ключ не раскрывает информацию о прошлых или будущих сообщениях
- Ключи получаются, а не передаются
- Автоматическая ротация ключей после каждого сообщения

### Архитектура безопасности

**Система файлов ключей**
У каждого контакта есть отдельный файл ключей, который никогда не покидает устройство:
- Настоящий ключевой материал неотличим от случайного заполнителя
- Пароль не нужен – аутентификация происходит через файл ключей
- Любое вмешательство обнаруживается немедленно

**Одноразовое рукопожатие**
Одноразовое рукопожатие устанавливает общую криптографическую основу:
- Выполняется **ровно один раз** для каждого контакта
- Цветной баннер постоянно показывает состояние безопасности
- После завершения рукопожатие **криптографически заблокировано** и никогда не может быть сброшено

**Защита от повторного воспроизведения**
Каждое сообщение можно расшифровать **ровно один раз**:
- Уникальные счётчики сообщений предотвращают любое повторение
- Попытки повторной расшифровки немедленно блокируются

**Защита от вмешательства**
RotorCrypt X активно защищается от обратной разработки:
- **Обнаружение антиотладки** – инструменты анализа обнаруживаются во время выполнения
- **Проверка целостности исполняемого файла** – любое изменение двоичного файла обнаруживается при запуске
- **Уничтожение ключей** – при обнаружении вмешательства все файлы ключей криптографически уничтожаются
- **Обфускация ядра** – криптодвижок работает через проприетарный интерпретатор

**Квантовая устойчивость**
- Эффективное ключевое пространство **2^768** – противостоит алгоритму Гровера
- Даже с квантовым компьютером взлом шифрования займёт больше времени, чем возраст вселенной

Бесплатное офлайн-шифрование для Windows. Роторный шифр Энигма + AES-256-GCM + HKDF-SHA3-256. Квантовостойкий. Без облака. Без сервера. Портативный. USB. Энигма, машина Энигма, шифр Энигма, Энигма Вторая мировая война, Блетчли-Парк, Алан Тьюринг, Мариан Реевский, Бомба, Ультра, операция Ультра, роторная машина, шифр Лоренца, Колосс, криптоанализ, листы Зыгальского, роторный шифр, SHA-3, Keccak, аутентифицированное шифрование, совершенная прямая секретность, гибридное шифрование, квантовый компьютер, квантовая криптография, алгоритм Гровера, алгоритм Шора, постквантовая криптография, квантовостойкий, пространство ключей 2^768, хакер, тестирование на проникновение, кибербезопасность, нулевое доверие, атака посредника, социальная инженерия, фишинг, вредоносное ПО, программа-вымогатель, АНБ, слежка, сквозное шифрование, конфиденциальность, защита данных, GDPR, офлайн-шифрование, без облака, без сервера, портативный, USB, Windows 10, Windows 11, безопасный мессенджер, шифрование файлов, RotorCrypt X, Энигма, машина Энигма, шифр Энигма, Энигма Вторая мировая война, Блетчли-Парк, Алан Тьюринг, Мариан Реевский, Бомба, Ультра, операция Ультра, роторная машина, шифр Лоренца, Колосс, криптоанализ, листы Зыгальского, роторный шифр, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, режим Галуа счётчика, аутентифицированное шифрование, совершенная прямая секретность, гибридное шифрование, симметричное шифрование, асимметричное шифрование, функция получения ключа, потоковый шифр, блочный шифр, квантовый компьютер, квантовая криптография, квантовое распределение ключей, QKD, алгоритм Гровера, алгоритм Шора, постквантовая криптография, квантовостойкий, пространство ключей 2^768, взлом, хакер, тестирование на проникновение, кибербезопасность, информационная безопасность, нулевое доверие, атака посредника, социальная инженерия, фишинг, вредоносное ПО, программа-вымогатель, АНБ, слежка, сквозное шифрование, анонимность, конфиденциальность, защита данных, GDPR, модуль аппаратной безопасности, TPM, управление ключами, офлайн-шифрование, без облака, без сервера, портативный, USB, Windows 10, Windows 11, безопасный мессенджер, шифрование файлов, бесплатное ПО
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_ru.html

---

## 🇧🇷 Português

### Três Camadas Criptográficas

**Camada 1 – Motor de Rotores Enigma**
RotorCrypt X baseia-se num princípio avançado de rotor Enigma, muito além da máquina histórica:
- Até **50 rotores configuráveis** (a Enigma histórica tinha 3–5)
- Suporte **Unicode** completo – 65.536 caracteres possíveis em vez de 26 letras
- Cada mensagem recebe uma **configuração completamente nova, gerada criptograficamente**
- O painel de ligações e o refletor são regenerados por mensagem
- Nenhuma mensagem partilha o mesmo estado de rotor

**Camada 2 – AES-256-GCM**
A saída Enigma é cifrada uma segunda vez com AES-256 no modo Galois/Contador:
- Cifração de grau militar
- Etiqueta de autenticação integrada – qualquer manipulação é detetada e rejeitada

**Camada 3 – Derivação de Chave HKDF-SHA3-256**
Cada mensagem gera chaves criptográficas novas:
- **Sigilo Direto Perfeito** – uma chave comprometida não revela nada sobre mensagens passadas ou futuras
- As chaves são derivadas, nunca transmitidas
- Rotação automática de chaves após cada mensagem

### Arquitetura de Segurança

**Sistema de Ficheiros de Chaves**
Cada contacto tem um ficheiro de chaves dedicado que nunca abandona o dispositivo:
- O material de chave real é indistinguível do preenchimento aleatório
- Sem palavra-passe – a autenticação acontece através do ficheiro de chaves
- Qualquer adulteração é detetada imediatamente

**Handshake Único**
Um handshake único estabelece a base criptográfica partilhada:
- Realizado **exatamente uma vez** por contacto
- Um banner com código de cores mostra o estado de segurança a qualquer momento
- Uma vez concluído, o handshake está **bloqueado criptograficamente** e nunca pode ser reposto

**Proteção contra Repetição**
Cada mensagem só pode ser decifrada **uma vez**:
- Contadores únicos de mensagens impedem qualquer repetição
- Tentativas de decifragem duplicadas são bloqueadas imediatamente

**Proteção contra Adulteração**
RotorCrypt X defende ativamente contra engenharia reversa:
- **Deteção anti-debug** – ferramentas de análise são detetadas em tempo de execução
- **Verificação de integridade do executável** – qualquer modificação é detetada no arranque
- **Destruição de chaves** – se adulteração for detetada, todos os ficheiros de chaves são destruídos criptograficamente
- **Ofuscação do núcleo** – o motor criptográfico funciona através de um interpretador proprietário

**Resistência Quântica**
- Espaço de chaves efetivo **2^768** – resiste ao algoritmo de Grover
- Mesmo com um computador quântico, quebrar a cifração levaria mais tempo do que a idade do universo

RotorCrypt X, Enigma, máquina Enigma, cifra Enigma, Enigma Segunda Guerra Mundial, Bletchley Park, Alan Turing, Gordon Welchman, Marian Rejewski, Bomba kryptologiczna, máquina Bombe, inteligência Ultra, operação Ultra, máquina de rotores, cifra Lorenz, Colossus, criptoanálise, folhas Zygalski, cifra de rotores, substituição polialfabética, AES-256, AES-256-GCM, HKDF-SHA3-256, SHA-3, Keccak, modo Galois Counter, AEAD, cifração autenticada, sigilo direto perfeito, cifração híbrida, cifração simétrica, cifração assimétrica, função de derivação de chave, KDF, nonce, vetor de inicialização, cifra de fluxo, cifra de bloco, bloco de notas de uso único, segurança teórica da informação, ataque de força bruta, ataque de dicionário, tabela arco-íris, prova de conhecimento zero, cifração homomórfica, criptografia de reticulado, computador quântico, criptografia quântica, distribuição quântica de chaves, QKD, algoritmo de Grover, algoritmo de Shor, criptografia pós-quântica, resistente a quantum, espaço de chaves 2^768, hacking, hacker, teste de penetração, segurança cibernética, segurança da informação, Zero Trust, homem no meio, engenharia social, phishing, malware, ransomware, NSA, vigilância, criptografia de ponta a ponta, anonimato, privacidade, proteção de dados, GDPR, módulo de segurança de hardware, TPM, gerenciamento de chaves, criptografia offline, sem nuvem, sem servidor, portátil, USB, Windows 10, Windows 11, mensagens seguras, criptografia de arquivos, software gratuito
https://www.bagdadi.de/RotorCrypt_X/RotorCryptX_pt.html

---

## Developer
T. Bagdadi · Germany · https://www.bagdadi.de

