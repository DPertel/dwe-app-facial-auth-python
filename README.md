# FaceID-Local

Aplicação local para detecção/identificação facial usando OpenCV (Haar Cascade) e/ou face_recognition (dlib).

# DWE - OWNERs
- Deivison Pertel – RM 550803
- Eduardo Akira Murata – RM 98713
- Wesley Souza de Oliveira – RM 97874


## Instalação

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate   # Windows
pip install -r requirements.txt
```

## Execução

1. Enrole um usuário:
```bash
python -m src.enroll --name SeuNome --num 5
```

2. Rode a aplicação principal:
```bash
python -m src.main
```

Ajuste parâmetros em `config.yaml`.

## 3. Teclas de controle na aplicação:

- C: Cadastrar novo usuário.

- D: Deletar usuário existente.

- Q: Encerrar o programa.

### Funcionalidades visuais:

- Rostos reconhecidos exibem o nome cadastrado em verde.

- Rostos não reconhecidos exibem Rosto Desconhecido em vermelho.

- FPS e instruções exibidas na tela (configurável).

# Nota Ética

- Consentimento: sempre obtenha consentimento explícito de qualquer pessoa cujas imagens ou dados faciais serão capturados e usados.

- Minimização de dados: armazene apenas o mínimo necessário. Evite manter dados por mais tempo do que o necessário.

- Segurança: proteja encodings e imagens (criptografia em trânsito/repouso, controle de acesso).

- Viés e justiça: modelos pré-treinados podem ter enviesamentos por idade, etnia, gênero. Teste com diversidade e documente limitações.

- Uso responsável: não use este código para vigilância em larga escala, decisões automatizadas sem supervisão humana, ou em contextos sensíveis sem revisão legal/ética.