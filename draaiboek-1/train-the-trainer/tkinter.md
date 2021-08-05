---
description: Create Graphic User Interfaces
---

# Tkinter

## Tkinter General Info

[https://docs.python.org/3/library/tkinter.html](https://docs.python.org/3/library/tkinter.html)

## 1. Basis App

![example code](../../.gitbook/assets/image%20%2810%29.png)

**from tkinter import \*:** Importeren van ‘alle’ functionaliteiten uit de tkinter module

**\#naamApp\#** = Tk\(\): Creëren van het basisscherm

**\#naamApp\#.mainLoop\(\)**: ‘Laten lopen’ van de app  


## 2. Widgets

{% tabs %}
{% tab title="Labels" %}
![example code](../../.gitbook/assets/image%20%281%29.png)

#### 1.       Label maken

**\#naamLabel\# = Label\(\#naamApp\#, text = “\#\#\#”\)**

Extra functionaliteiten:

* **fg=”\#”**: tekstkleur van de label \(kleuren of hexcodes\)
* **bg=”\#”**: achtergrondkleur van de label \(kleuren of hexcodes\)
* **borderwidth=\#:** Breedte van de rand van de label

#### 2.       Label laten verschijnen op het scherm

**\#naamLabel\#.grid\(row=\#, column=\#\)**
{% endtab %}

{% tab title="Buttons" %}
![example code](../../.gitbook/assets/image%20%2814%29.png)

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

![example code](../../.gitbook/assets/image%20%288%29.png)
{% endtab %}

{% tab title="Inputboxes" %}
![example code](../../.gitbook/assets/image%20%283%29.png)

#### 1.       Inputbox maken

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

{% endtab %}

{% tab title="Icon" %}

{% endtab %}
{% endtabs %}

## 4. Message Boxes

## 5. File Dialog

