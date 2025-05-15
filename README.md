# 🗳️ Urna Eletrônica com Interface Gráfica

Este projeto é uma simulação de uma urna eletrônica desenvolvida com **Python**, utilizando as bibliotecas **Tkinter** para a interface gráfica e **OpenCV** para captura de imagens dos candidatos pela webcam. A aplicação permite o cadastro de candidatos, a realização da votação com confirmação, votos em branco, e a exibição do vencedor ao final da eleição.

## 📌 Funcionalidades

- Cadastro de candidatos com foto (tirada pela webcam)
- Interface amigável para votação
- Digitação do número do candidato com feedback visual
- Resultado exibido ao final da votação
- Exportação dos resultados em `.txt`
- Interface do administrador com acesso a cadastro e encerramento

## 🛠️ Tecnologias utilizadas

- Python 3
- Tkinter (GUI)
- OpenCV (cv2)
- PIL (Pillow)
- OS / Shutil / Time / Random / JSON

## 📷 Cadastro de Candidatos

Durante o cadastro, o administrador digita o nome, número e cargo do candidato e a webcam será ativada para capturar uma imagem, que será associada ao candidato. Os dados são armazenados em um arquivo `.json`.

## 🔐 Acesso do Administrador

O administrador pode:
- Cadastrar candidatos
- Encerrar a votação
- Visualizar e exportar os resultados em um arquivo `.txt`

## 📁 Estrutura do Projeto

- **main.py**  
  Arquivo principal da aplicação. Contém toda a lógica do sistema, desde a interface gráfica até o controle de votos e exportação de resultados.

- **candidatos.json**  
  Arquivo em formato JSON onde são salvos os dados dos candidatos cadastrados, como nome, número e caminho da imagem.

- **resultado.txt**  
  Arquivo gerado automaticamente ao final da votação, contendo a contagem de votos e o vencedor.

- **fotos/**  
  Diretório que armazena as imagens capturadas pela webcam no momento do cadastro do candidato.
