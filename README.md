# README — Visualizador de Imagens

## 📱 Projeto: Visualizador de Imagens

Aplicativo desenvolvido no Android Studio com Java utilizando o componente `ImageView` para exibir imagens dinamicamente através de botões.

O projeto tem como objetivo praticar conceitos básicos de desenvolvimento Android, como:

* Criação de interfaces com `ConstraintLayout`
* Manipulação de imagens
* Utilização de `ImageView`
* Utilização de `Button`
* Programação de eventos de clique
* Alteração dinâmica de componentes
* Atualização de textos com Java

---

# 🖼️ Funcionalidades do Aplicativo

✅ Exibição de imagens na tela
✅ Texto informativo abaixo da imagem
✅ Botão para abrir a Foto 1
✅ Botão para abrir a Foto 2
✅ Alteração dinâmica das imagens
✅ Atualização automática do texto

---

# 🛠️ Tecnologias Utilizadas

* Java
* Android Studio
* XML
* ConstraintLayout

---

# 📂 Estrutura do Projeto

```plaintext
java/
 └── Arquivos Java

res/
 ├── layout/
 │    └── activity_visualizador_imagens.xml
 │
 ├── drawable/
 │    ├── foto1.jpg
 │    └── foto2.jpg
```

---

# 📸 Imagens Utilizadas

O aplicativo utiliza duas imagens:

* `foto1.jpg`
* `foto2.jpg`

As imagens devem ser adicionadas dentro da pasta:

```plaintext
res/drawable
```

---

# 📱 Interface do Aplicativo

A tela do aplicativo possui:

* Um título informativo
* Um `ImageView`
* Um `TextView`
* Dois botões

---

# 🧩 Componentes Utilizados

## ImageView

Responsável por exibir as imagens na tela.

```xml
<ImageView
    android:id="@+id/imgfoto"
    android:layout_width="250dp"
    android:layout_height="250dp"
    android:src="@drawable/foto1"/>
```

---

## TextView

Exibe o nome da imagem atual.

```xml
<TextView
    android:id="@+id/txtinformacao"
    android:text="Foto 1"/>
```

---

## Buttons

Permitem alternar entre as imagens.

```xml
<Button
    android:id="@+id/btfoto1"
    android:text="Abrir Foto 1"/>
```

```xml
<Button
    android:id="@+id/btfoto2"
    android:text="Abrir Foto 2"/>
```

---

# ⚙️ Funcionamento do Aplicativo

Ao clicar no botão:

### 📌 Abrir Foto 1

O aplicativo:

* exibe a imagem `foto1`
* altera o texto para `"Foto 1"`

```java
imgfoto.setImageResource(R.drawable.foto1);
txtinformacao.setText("Foto 1");
```

---

### 📌 Abrir Foto 2

O aplicativo:

* exibe a imagem `foto2`
* altera o texto para `"Foto 2"`

```java
imgfoto.setImageResource(R.drawable.foto2);
txtinformacao.setText("Foto 2");
```

---

# 💻 Código Java Principal

```java
btfoto1.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View view) {

        imgfoto.setImageResource(R.drawable.foto1);

        txtinformacao.setText("Foto 1");
    }
});

btfoto2.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View view) {

        imgfoto.setImageResource(R.drawable.foto2);

        txtinformacao.setText("Foto 2");
    }
});
```

---

# ▶️ Como Executar o Projeto

1. Abra o Android Studio
2. Clique em:

   ```plaintext
   Open
   ```
3. Selecione a pasta do projeto
4. Aguarde o Gradle sincronizar
5. Execute o aplicativo em:

   * Emulador Android
   * Celular físico

---

# 🎯 Objetivo Educacional

Este projeto foi desenvolvido com fins educacionais para praticar:

* Desenvolvimento Android
* Programação em Java
* Manipulação de componentes gráficos
* Eventos de clique
* Alteração dinâmica da interface

---

# 👨‍💻 Autor

Projeto desenvolvido por Camille Ferreira para estudos de Desenvolvimento Mobile com Android Studio.
