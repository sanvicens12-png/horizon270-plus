# HORIZON270+

Plataforma de streaming gratuïta per descobrir i veure pel·lícules i sèries.

HORIZON270+ està pensada com una plataforma moderna de contingut audiovisual, amb comptes d'usuari, perfils, catàleg, reproducció i un panell d'administració.

---

## 🎬 Sobre HORIZON270+

HORIZON270+ és una plataforma de streaming centrada en:

* 🎬 Pel·lícules
* 📺 Sèries
* ▶️ Episodis
* 🎞️ Tràilers
* 🎭 Actors i personatges
* ⭐ Llistes personals
* 🔥 Contingut popular
* 🆕 Novetats
* 📅 Estrenes programades
* 🌍 Disponibilitat segons país

La plataforma és **totalment gratuïta**.

---

# 👤 Comptes i perfils

HORIZON270+ utilitza autenticació amb Supabase.

Els usuaris poden:

* Crear un compte
* Iniciar sessió amb correu electrònic
* Iniciar sessió amb Google
* Tancar sessió
* Seleccionar un perfil
* Consultar la configuració del compte
* Gestionar el seu compte
* Eliminar el compte

---

# 🛠️ Administració

HORIZON270+ disposa d'un compte d'administrador.

L'administrador podrà gestionar:

* Pel·lícules
* Sèries
* Temporades
* Episodis
* Actors
* Personatges
* Tràilers
* Contingut relacionat
* Contingut similar
* Portades
* Miniatures
* Estrenes
* Disponibilitat per països

L'accés d'administració està separat dels comptes normals.

---

# 📁 Estructura actual

```text
HORIZON270+
│
├── index.html
├── login.html
├── profiles.html
├── catalog.html
├── account.html
├── admin.html
│
└── README.md
```

---

# 🧭 Navegació

El recorregut principal de l'usuari és:

```text
index.html
      │
      ▼
login.html
      │
      ▼
profiles.html
      │
      ├──────────────► account.html
      │
      ├──────────────► admin.html
      │
      ▼
catalog.html
```

---

# 🔐 Autenticació

La plataforma utilitza:

**Supabase Authentication**

Mètodes actuals:

* Email + contrasenya
* Google

La sessió es comprova abans d'entrar a les zones privades.

---

# 🗄️ Base de dades

La base de dades utilitza Supabase.

Entre les taules del projecte hi ha:

```text
Profiles
```

La taula `Profiles` conté informació com:

```text
id
username
account_type
created_at
```

Els tipus de compte inclouen:

```text
admin
```

i comptes normals.

---

# 🎥 Catàleg

El catàleg serà dinàmic i estarà connectat amb Supabase.

Cada contingut podrà tenir informació com:

```text
Títol
Descripció
Tipus
Gènere
Any
Durada
Imatge
Tràiler
Vídeo
Actors
Països disponibles
Data d'estrena
```

---

# 📺 Sèries

Les sèries tindran una estructura jeràrquica:

```text
Sèrie
│
├── Temporada 1
│   ├── Episodi 1
│   ├── Episodi 2
│   └── Episodi 3
│
├── Temporada 2
│   ├── Episodi 1
│   └── Episodi 2
│
└── Temporada 3
```

---

# ▶️ Reproducció

La plataforma està preparada per incorporar un reproductor de vídeo.

Funcions previstes:

* Reproducció
* Pausa
* Pantalla completa
* Barra de progrés
* Subtítols
* Selecció d'episodi
* Següent episodi
* Continuar veient

---

# ⭐ La meva llista

Els usuaris podran guardar contingut per veure'l més tard.

```text
Pel·lícula
     ↓
+ Afegir a la meva llista
     ↓
La meva llista
```

---

# 📅 Llançaments

HORIZON270+ permetrà programar estrenes.

Exemple:

```text
Títol:
Nova pel·lícula

Data:
15/09/2026

Hora:
20:00
```

Abans de l'estrena es podrà mostrar com a pròxim llançament.

Quan arribi la data i hora programades, el contingut passarà automàticament a estar disponible.

---

# 🌍 Disponibilitat per països

Cada contingut podrà tenir restriccions geogràfiques.

Exemple:

```text
Disponible:
🇪🇸 Espanya
🇫🇷 França
🇮🇹 Itàlia

No disponible:
🇺🇸 Estats Units
```

---

# 📧 Notificacions

Està prevista una funció de notificacions per correu electrònic.

Els usuaris podran rebre informació sobre:

* Noves pel·lícules
* Noves sèries
* Nous episodis
* Estrenes
* Novetats del catàleg

---

# 🔒 Seguretat

Les zones privades requereixen autenticació.

L'administració està destinada exclusivament al compte administrador.

La seguretat definitiva de les dades es gestionarà mitjançant:

* Supabase Authentication
* Row Level Security (RLS)
* Polítiques de base de dades
* Funcions server-side per a operacions sensibles

Les claus secretes de Supabase **mai s'han d'incloure en el codi públic del repositori**.

---

# 🌐 Tecnologia

HORIZON270+ utilitza actualment:

* HTML
* CSS
* JavaScript
* Supabase
* GitHub Pages

---

# 🚧 Estat del projecte

El projecte es troba en desenvolupament.

### ✅ Fet

* [x] Portada
* [x] Login
* [x] Crear compte
* [x] Google Login
* [x] Sessió d'usuari
* [x] Pantalla de perfils
* [x] Compte d'usuari
* [x] Base inicial de Supabase
* [x] Sistema inicial d'administració

### 🔨 En desenvolupament

* [ ] Catàleg connectat a Supabase
* [ ] Gestió real de pel·lícules
* [ ] Gestió real de sèries
* [ ] Temporades
* [ ] Episodis
* [ ] Actors
* [ ] Personatges
* [ ] Tràilers
* [ ] Reproductor
* [ ] La meva llista
* [ ] Continuar veient
* [ ] Llançaments programats
* [ ] Notificacions per correu
* [ ] Restriccions per país
* [ ] RLS definitiva
* [ ] Eliminació segura de comptes
* [ ] Disseny final de la plataforma

---

# 🎯 Objectiu

L'objectiu de HORIZON270+ és crear una plataforma de streaming gratuïta, moderna i accessible on els usuaris puguin descobrir i veure contingut audiovisual en un únic lloc.

---

# 📌 Projecte

**Nom:** HORIZON270+
**Tipus:** Plataforma de streaming
**Model:** Gratuït
**Estat:** En desenvolupament
**Any:** 2026

---

© 2026 HORIZON270+
Tots els drets reservats.
