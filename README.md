# Reconhecimento Facial e transformação de imagens em Dados no Azure ML

Para a realização do trabalho, foram seguidos os passos descritos no site **[Microsoft Learn](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html)**

O Azure AI Vision inclui inúmeras capacidades para compreender o conteúdo e o contexto da imagem e extrair informações das imagens. O Azure AI Vision Studio permite-lhe experimentar muitas das capacidades de análise de imagens.

# Uso

Criar um recurso de *serviços de IA do Azure*, conectar o seu recurso de serviço de IA do Azure ao Vision Studio, extrair textos de imagens no Vision Studio

# Processo

<details>
<summary>Crie um recurso de *serviços de IA do Azure*</summary>

Você pode usar os recursos de OCR do Azure AI Vision com um recurso multisserviço de serviços de IA do Azure. Se ainda não o fez, crie um recurso de serviços de IA do Azure na sua assinatura do Azure.

1. Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com, entrando com a conta da Microsoft associada à sua assinatura do Azure.
2. Clique no botão **＋Criar um recurso** e pesquise os serviços de IA do Azure . Selecione **criar** um plano de **serviços de IA do Azure**. Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações:
    - **Assinatura**: sua assinatura do Azure;
    - **Grupo de recursos**: selecione ou crie um grupo de recursos com um nome exclusivo;
    - **Região**: Leste dos EUA;
    - **Nome**: Insira um nome exclusivo;
    - **Nível de preços**: Padrão S0;
    - **Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo**: Selecionado;
3. Selecione **Revisar + criar** e depois **Criar** e aguarde a conclusão da implantação.


</details>
<details>
<summary>Conecte seu recurso de serviço de IA do Azure ao Vision Studio</summary>

Em seguida, conecte o recurso de serviços de IA do Azure provisionado acima ao Vision Studio.

1. Em outra guia do navegador, navegue até **Vision Studio** em https://portal.vision.cognitive.azure.com.

2. Entre com sua conta e certifique-se de usar o mesmo diretório onde você criou seu recurso de serviços de IA do Azure.

3. Na página inicial do Vision Studio, selecione **Visualizar todos os recursos** no título **Introdução ao Vision**.

![image](https://github.com/juliocandrade/azure-ai-vision-studio/assets/66694754/d890f57c-9000-4dd0-b076-caa47e524f1c)

4. Na página **Selecione um recurso para trabalhar**, passe o cursor do mouse sobre o recurso que você criou acima na lista e marque a caixa à esquerda do nome do recurso e selecione **Selecionar como recurso padrão**.

 >[!IMPORTANT]
 > Se o seu recurso não estiver listado, pode ser necessário **atualizar** a página.

![image](https://github.com/juliocandrade/azure-ai-vision-studio/assets/66694754/3d0b83ef-b454-4b51-996d-f6918d936a6d)

5. Feche a página de configurações selecionando o “x” no canto superior direito da tela.

</details>
<details>
<summary>Extraia texto de imagens no Vision Studio</summary>
  
1. Num navegador web, navegue até **Vision Studio** em https://portal.vision.cognitive.azure.com.

2. Na página inicial de **Introdução ao Vision**, selecione **Optical character recognition** e, em seguida, na caixa **Extract text from images**.

3. No subtítulo **Try it out**, reconheça a política de uso de recursos lendo e marcando a caixa.

4. Selecione https://aka.ms/mslearn-ocr-images para baixar **ocr-images.zip**. Em seguida, abra a pasta.

5. No portal, selecione **Browse for a file** e navegue até a pasta em seu computador onde você baixou **ocr-images.zip**. Selecione **advert.jpg** e selecione Open.

6. Agora revise o que é retornado:
      - Nos **Detected attributes**, qualquer texto encontrado na imagem é organizado em uma estrutura hierárquica de regiões, linhas e palavras.
      - Na imagem, a localização do texto é indicada por uma caixa delimitadora, conforme mostrado aqui:

![image](https://github.com/juliocandrade/azure-ai-vision-studio/assets/66694754/b7b9dfbe-8683-4cc4-b9b1-90e07bb59268)

7. Agora você pode tentar outra imagem. **Browse for a file** e navegue até a pasta onde você salvou os arquivos do GitHub. Selecione **letter.jpg**.

![image](https://github.com/juliocandrade/azure-ai-vision-studio/assets/66694754/c078f6db-7e25-4516-b43d-aa669f611e43)

8. Revise os resultados da segunda imagem. Deve retornar o texto e as caixas delimitadoras do texto. Se você tiver tempo, tente **note.jpg** e **receipt.jpg**.
</details>
<details>
<summary>Excluir</summary>

Se não pretende fazer mais exercícios, exclua todos os recursos que não precisa mais. Isso evita acumular custos desnecessários.

1. Abra o **portal do Azure** em https://portal.azure.com e selecione o grupo de recursos que contém o recurso que você criou.
2. Selecione o recurso e selecione **Delete** e depois **Yes** para confirmar. O recurso é então excluído.
</details>
