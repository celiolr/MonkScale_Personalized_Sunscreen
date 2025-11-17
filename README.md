# MonkScale Personalized Sunscreen
Personalized Sunscreen Recommendation System Based on Computer Vision and the Monk Skin Tone Scale

# Sistema de Recomendação Personalizada de Protetor Solar  
### Baseado em Visão Computacional e na Escala Monk

Este repositório contém o código-fonte do projeto **“Sistema de Recomendação Personalizada de Protetor Solar com Base em Visão Computacional e na Escala Monk”**, que integra **Visão Computacional**, **Redes Neurais Convolucionais (CNNs)** e **Ciência Farmacêutica** para estimar tons de pele de forma contínua e sugerir formulações de protetor solar tonalizado personalizadas.

O sistema analisa imagens faciais, estima o tom de pele pela **Monk Skin Tone Scale (MST)**, calibra a cor no espaço **LAB** e calcula a proporção de pigmentos para compor um protetor solar adequado a diferentes tons de pele, promovendo **inclusão dermatológica** e reduzindo o efeito esbranquiçado comum em fotoprotetores convencionais.

---

## 🔍 Funcionalidades

- Detecção facial com **MTCNN**
- Estimação contínua de tom de pele (1–10, Escala Monk)
- Calibração colorimétrica em LAB
- Formulação automatizada (óxidos de ferro + TiO₂)
- Suporte a múltiplas CNNs (ConvNeXt-Tiny, EfficientNet-B0, MobileNetV3-Large, VGG16)
- Pipeline completo em notebook Google Colab
- Geração de gráficos, histogramas e relatórios da formulação

---

## 📁 Estrutura do Repositório

## 📁 Estrutura do Datase
	dataset/
	│
	├── 1/
	│	├── down-facing						cada subpasta
	│	├── front-facing				   	front-facing		
	│   │   ├──	F_cool_1200.jpeg           	├──	F_cool_1200.jpeg 
	│   │   ├──	...           	           	├──	F_cool_200.jpeg  	           	           	           	           	           	           	           	           	           	
	│	├── left-facing                     ├──	F_cool_600.jpeg  
	│	├── right-facing                    ├──	F_warm_1200.jpeg 
	│	├── up-facing                       ├──	F_warm_200.jpeg  
	│	└── monk_scale_value.json           ├──	F_warm_600.jpeg  
	│                                       ├──	H_warm_1200.jpeg 
	├── 2/                                  ├──	H_warm_200.jpeg  
	│   ├── ...                             ├──	H_warm_600.jpeg  
	│   └── monk_scale_value.json           ├──	L_cool_1200.jpeg 
	│                                       ├──	L_cool_200.jpeg  
	│...                                    ├──	L_cool_600.jpeg  
	└── 285/                                ├──	L_warm_1200.jpeg 
		├── ...                             ├──	L_warm_200.jpeg  
		└── monk_scale_value.json           └── L_warm_600.jpeg	

	Exemplo .json
	{"value": 5.5}

A licença aplica-se somente ao código-fonte.

Nenhum dataset, imagem ou material sensível está incluído 
ou licenciado neste repositório.


