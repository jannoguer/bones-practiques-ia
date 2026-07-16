# BONES PRÀCTIQUES AMB LA IA

<p align="center"><i>"La IA no és intel·ligent, és culta."</i></p>

Guia breu per treure més profit de la IA en el dia a dia. Les respostes de la IA no són sempre correctes: pot cometre errors fins i tot tenint la informació correcta.

## Estructura dels prompts

Persona *(opcional)* → **Context** → **Tasca** → **Format**

> [!TIP]
> La mateixa IA et pot fer els prompts!

**Exemple:** Ets un expert en atenció al client *(←Persona)*. La nostra empresa acumula retards greus en les comandes per un problema amb la missatgeria i diversos clients s'han queixat *(←Context)*. Redacta un missatge de disculpa per calmar-los *(←Tasca)* presentat com una plantilla amb espais per emplenar *(←Format)*.

> [!NOTE]
> El primer prompt rarament dona el resultat desitjat a la primera, cal seguir la conversa demanant ajustos fins arribar-hi.

> [!NOTE]
> Adjuntar exemples millora els prompts significativament.

## Feines pesades

<p align="center"><i>"No deixis que la IA faci la feina, utilitza-la per crear les eines que la faran."</i></p>

### Malament

**Exemple:** "Elimina els duplicats i ordena alfabèticament els correus d'aquesta llista: ..."

**Resultat:** Omissió d'informació, al·lucinacions, imprecisió, degradació de l'atenció, truncament de la resposta, etc.

### Correcte

**Exemple:** "Crea un programa en Python per eliminar els duplicats i ordenar alfabèticament els correus d'aquesta llista: ..."

**Resultat:** Llista correctament estructurada i amb totes les dades. A més, pots repetir el mateix procediment amb una nova llista (si manté el format, és clar).

<p align="center">EL PROGRAMA NO LLEGEIX LA INFORMACIÓ, LA PROCESSA.</p>

## Canvis en fitxers grans

No pots esperar que la IA et generi un fitxer de 2.000 línies sencer, sense errors i de cop a través del xat.

Si els canvis són petits, **demana només les línies modificades**.

Si són molts canvis, hi ha **dues opcions**:
* **Demanar el fitxer actualitzat per descarregar:** Sol·licita que t'ofereixi un botó de descàrrega amb el document llest (no totes les IA ho permeten).
* **Treballar en local:** Planteja't utilitzar la IA directament des de l'escriptori (en lloc de la versió web) per poder editar els fitxers directament des del disc dur.

## Regles de la sessió

A mesura que la conversa creix, la finestra de context s'omple i la qualitat de les respostes es degrada. Per això convé començar de zero sovint:

* **Tasca finalitzada**: Iniciar una **nova sessió**.
* **La IA al·lucina**: Desplegar **prompt "handoff"** → Iniciar una **nova sessió** *(amb resum + fitxers requerits)*.

> [!NOTE]
> Un **prompt "handoff"** és una instrucció que demanes a la IA abans de tancar la sessió perquè resumeixi l'estat de la feina (què s'ha fet, què queda i quins fitxers calen), de manera que puguis enganxar aquest resum a la sessió nova i continuar sense perdre context.

## Glossari

* **Prompt**: la instrucció o text que li escrius a la IA.
* **Finestra de context**: tot el que la IA "recorda" dins una mateixa conversa. Té un límit i, quan s'omple, la qualitat de les respostes baixa.
* **Token**: la unitat en què la IA mesura el text. El càlcul real és complicat, però com a regla simple: unes 3 paraules equivalen aproximadament a 4 tokens (segons l'idioma).
