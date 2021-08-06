---
description: Create Graphic User Interfaces
---

# Tkinter

## Tkinter General Info

[https://docs.python.org/3/library/tkinter.html](https://docs.python.org/3/library/tkinter.html)

## 1. Basis App

![example code](../../.gitbook/assets/image%20%2816%29.png)

**from tkinter import \*:** Importeren van ‘alle’ functionaliteiten uit de tkinter module



**\#naamApp\#.mainLoop\(\)**: ‘Laten lopen’ van de app

## 2. Widgets

{% tabs %}
{% tab title="Labels" %}
![example code](../../.gitbook/assets/image%20%281%29.png)

#### 

**\#naamLabel\# = Label\(\#naamApp\#, text = “\#\#\#”\)**

Extra functionaliteiten:

* **fg=”\#”**: tekstkleur van de label \(kleuren of hexcodes\)
* **bg=”\#”**: achtergrondkleur van de label \(kleuren of hexcodes\)
* **borderwidth=\#:** Breedte van de rand van de label

#### 2.       Label laten verschijnen op het scherm

**\#naamLabel\#.grid\(row=\#, column=\#\)**
{% endtab %}

{% tab title="Buttons" %}
![example code](../../.gitbook/assets/image%20%2823%29.png)

#### 1.       Button maken

**\#naamButton\# = Button\(\#naamApp\#, text=”\#\#\#”\)**

Extra functionaliteiten:

* **padx=\#**: hoogte van de button
* **pady=\#**: breedte van de button
* **fg=”\#”**: tekstkleur van de button \(kleuren of hexcodes\)
* **bg=”\#”**: achtergrondkleur van de button \(kleuren of hexcodes\)
* **borderwidth=\#:** Breedte van de rand van de button

#### 2.       Button laten verschijnen op het scherm

**\#naamButton\#.grid\(row=\#, column=\#\)**

#### 3.       Button een command laten uitvoeren

![example code](../../.gitbook/assets/image%20%2811%29.png)
{% endtab %}

{% tab title="Inputboxes" %}
![example code](../../.gitbook/assets/image%20%283%29.png)

#### 

**\#naamInputbox\# = Entry\(\#naamApp\#\)**

Extra functionaliteiten:

* **width=\#:** breedte van de inputbox
* **fg=”\#”**: tekstkleur van de inputbox \(kleuren of hexcodes\)
* **bg=”\#”**: achtergrondkleur van de inputbox \(kleuren of hexcodes\)
* **borderwidth=\#:** Breedte van de rand van de inputbox

#### 2.       Inputbox laten verschijnen op het scherm

**\#naamInputbox\#.grid\(row=\#, column=\#\)**

#### 3.       Input uit de box gebruiken

**\#naamInputbox\#.get\(\)**

![example code](../../.gitbook/assets/image%20%287%29.png)
{% endtab %}

{% tab title="Checkboxes" %}

{% endtab %}
{% endtabs %}

## 3. Layout

{% tabs %}
{% tab title="General Layout" %}
**Algemene opties:**

* **\#naamApp\#.title\("\#"\):** Titel van de App
* **\#naamApp\#.configure\(bg="\#"\):** Achtergrondkleur van de App
* **\#naamApp\#.geometry\("\#x\#"\):** Afmeting van de App
{% endtab %}

{% tab title="Images" %}
**from PIL import ImageTk, Image**\*: Module individueel te importeren

#### **1.        Afbeelding maken**

**\#afbeelding\# = ImageTk.PhotoImage\(Image.open\("'\#pad\#"\)**

#### **2.       Afbeelding laten verschijnen op het scherm**

**\#Label\# = Label\(image=\#afbeelding\#\)**

**\#Label\#.grid\(row=0, column=0\)**

\*pip install Pillow
{% endtab %}

{% tab title="Icon" %}
**\#naamApp\#.iconbitmap\("\#padnaam\#"\)**: Selecteer een Icon voor je venster _\(.ico afbeelding\)_
{% endtab %}
{% endtabs %}

## 4. Message Boxes

{% tabs %}
{% tab title="Info" %}
**messagebox.showinfo\("\#", "\#"\)**: Geeft een info pop-up _\(eerste tekst komt in header, tweede in de messagebox\)_

![example of info messagebox](../../.gitbook/assets/image%20%289%29.png)

![example code](../../.gitbook/assets/image%20%2813%29.png)

**from tkinter import messagebox**: Module apart te importeren
{% endtab %}

{% tab title="Warning" %}
**messagebox.showwarning\("\#", "\#"\)**: Geeft een info pop-up _\(eerste tekst komt in header, tweede in de messagebox\)_

![example of warning messagebox](../../.gitbook/assets/image%20%2810%29.png)
{% endtab %}

{% tab title="Error" %}
**messagebox.showerror\("\#", "\#"\)**: Geeft een info pop-up _\(eerste tekst komt in header, tweede in de messagebox\)_

![example of warning messagebox](../../.gitbook/assets/image%20%2818%29.png)
{% endtab %}

{% tab title="Yes/No" %}
**messagebox.askyesno\("\#", "\#"\)**: Geeft een info pop-up _\(eerste tekst komt in header, tweede in de messagebox\)_

![example of question messagebox](../../.gitbook/assets/image%20%288%29.png)

Klikken op 'Ja', returns een 1, klikken op 'Nee' een 0.

![example code](../../.gitbook/assets/image%20%2825%29.png)
{% endtab %}

{% tab title="Cancel" %}
**messagebox.askokcancel\("\#", "\#"\)**: Geeft een info pop-up _\(eerste tekst komt in header, tweede in de messagebox\)_

![example of cancel messagebox](../../.gitbook/assets/image%20%2815%29.png)

Klikken op 'Ok', returns een 1, klikken op 'Annuleren' een 0.
{% endtab %}

{% tab title="Yes/No/Cancel" %}
**messagebox.askyesnocancel\("\#", "\#"\)**: Geeft een info pop-up _\(eerste tekst komt in header, tweede in de messagebox\)_

![example of yes/no/cancel messagebox](../../.gitbook/assets/image%20%2817%29.png)
{% endtab %}
{% endtabs %}

## 5. File Dialog

**from tkinter import filedialog**: Module apart te importeren

**filedialog.askopenfilename\(title = "\#", filetypes=\(\("\#", "\*.\#\#\#"\),\("\#", "\*.\#\#\#"\)\)\)**: Opent een filedialog om bestanden te selecteren

**filedialog.askopendirecotry\(title = "\#"\)**: Opent een filedialog om een directory te selecteren

filedialog returns het pad naar het gekozen bestand of directory

## 6. Create new Window

**\#naamwindow\# = Toplevel\(\):** Creatie van een tweede scherm

**\#naamButton\# = Button\(\#naamwindow\#, text="\#", command=\#naamwindow\#.destroy\):** Automatisch sluiten van het tweede scherm

\*Second windows **within a function** need **global** variables 
