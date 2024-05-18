# Instalando e configurando o Voicemeeter Banana

O **Voicemeeter Banana** é um software gratuito de mixagem de áudio virtual para Windows. Ele funciona como uma mesa de som digital, permitindo que você conecte e misture diversas fontes de áudio de maneira fácil e com controle preciso da qualidade do som.

![Logo](images/vmb_thumbnail.png)

## Recursos do Voicemeeter Banana:

- **Mixar várias fontes de áudio:** Microfone, som do computador, música, instrumentos musicais e muito mais.

- **Rotear áudio para diferentes destinos:** Alto-falantes, fones de ouvido, programas de streaming e software de gravação.

- **Aplicar efeitos de áudio:** Equalização, compressão, reverb e outros.

- **Criar mixagens personalizadas:** Salvar e carregar presets para diferentes situações.

- **Monitorar seus níveis de áudio:** Visualizadores de nível de som para cada canal.

## O Voicemeeter Banana é ideal para:

- **Streamers e criadores de conteúdo:** Misturar áudio de microfone, música, jogos e outros programas para transmissões ao vivo e gravações.

- **Músicos:** Gravar e produzir música com vários instrumentos e vozes.

- **Podcasters:** Gravar podcasts com alta qualidade de som.

- **DJs:** Mixar músicas para apresentações ao vivo.

- **Usuários comuns:** Melhorar a qualidade do som do computador para ouvir música, assistir a filmes e jogar.

## Índice

Neste repostório será desmonstrado como instalar e configurar o **Voicemeeter Banana** para separar faixas de áudios advindas de:

**Aplicativos de músicas** (Spotify, Deezer, Soundcloud...)

**Aplicativos de comunicação** (Discord, TeamSpeak, VOIPs... )

**Aplicativos restantes** (navegadores, jogos, notificações...)

Portanto, você conseguirá manipular separadamente cada uma dessas faixas de áudio.

1. [Instalação do Voicemeeter Banana](#instalação-do-voicemeeter-Banana)

2. [Instalação do Virtual Audio Cable](#instalação-do-virtual-audio-cable)

3. [Configurando o Voicemeeter Banana](#configurando-o-voicemeeter-banana)

4. [Configurando o Windows](#configurando-o-windows)

5. [Configurando a Saída de Música](#configurando-a-saída-de-música)

6. [Configurando a Saída de Comunicação](#configurando-a-saída-de-comunicação)

7. [Observações](#observações)

8. [Referências](#referências)

## Instalação do Voicemeeter Banana

**Faça o download do arquivo do Voicemeeter Banana.**

Faça o download [aqui](https://github.com/matheusaudibert/voice_meeter_banana/blob/main/voicemeeterbanana/VoicemeeterProSetup.exe) ou baixe no site oficial: https://vb-audio.com/Voicemeeter/banana.htm

Após concluir o download do arquivo, inicie-o e clique em "Install".

![Logo](images/vmb_install.png)

## Instalação do Virtual Audio Cable

**Faça o download do arquivo do Virtual Audio Cable.**

**Virtual Audio Cable (VAC)**, também conhecido como **Cabo de Áudio Virtual**, é um dispositivo de entrada e saída de áudio virtual que funciona como uma ponte entre diferentes programas e aplicativos. Ele permite que você roteie o áudio de um programa para outro, sem a necessidade de cabos físicos.

Faça o download [aqui](https://github.com/matheusaudibert/voice_meeter_banana/blob/main/virtualaudiocable/VBCABLE_Driver_Pack43.zip) ou baixe no site oficial: https://vb-audio.com/Cable/index.htm

Extraia os arquivos para um pasta e execute o aplicativo **VBCABLE_Setup_x64** como administrador e cliquei em "Install Driver".

![Logo](images/vac_install.png)

Após ter feito a instalação do **Voicemeeter Banana** e do **Virtual Audio Cable**, reinicie o seu computador.

## Configurando o Voicemeeter Banana

Depois de renicializar o seu computador, digite **Banana** na barra de pesquisa do Windows e abra o aplicativo.

Ao abrir o aplicativo pela primeira vez, você vai se deparar com isto:

![Logo](images/vmb_interface.png)

Não se assuste, esta é a interface padrão do **Voicemeeter Banana**, e logo você vai aprender a como utiliza-lá.

**Para começar o a configurar o aplicativo, siga estes passos:**

1. Clique em **MENU** e habilite as opções **System Tray** e **Run on Windows Startup**.

2. Clique com o botão direito em **HARDWARE INPUT 1** e nomeie a seção como **Mic**.

3. Clique em **Mic** e selecione o seu **microfone**, o dispositvo que você está usando para de comunicar. A opção selecionada deve ser do tipo **WDM**.

   Seu programa deve estar desta maneira:

   ![Logo](images/vmb_mic.png)

   Isso quer dizer que a faixa, que vai reproduzir a sua voz, foi configurada.

4. Clique com o botão direito em **HARDWARE INPUT 2** e nomeie a seção como **Music**.

5. Clique em **Music** e selecione a opção **WDM: CABLE Output (VB-Audio Virtual Cable)**

   Seu programa deve estar desta maneira:

   ![Logo](images/vmb_music.png)

   Isso quer dizer que a faixa, em que suas músicas serão reproduzidas, foi configurada.

6. Clique com o botão direito em **VIRTUAL INPUTS** e nomeie cada seção com um nome: **Sound** e **Voice**:

   Seu programa deve estar desta maneira:

   ![Logo](images/vmb_virtual_inputs.png)

   Isso quer dizer que a faixa da direita será destinada aos **Aplicativos de comunicação** e a faixa da esquerda aos **Aplicativos restantes**.

7. Clique em **HARDWARE INPUT (A1)** e selecione o seu **Alto-Falante**, o dispositivo que você esta usando para **receber** áudio. A opção selecionada deve ser do tipo **WDM**.

8. Deixe a opção **B1** habilitada apenas na primeira linha de áudio.

9. Clique em **MENU** e em seguida em **Restart Audio Engine**.

10. Clique em **MENU** e em seguida em **System Settings / Options...**.

    Nesta etapa, certifiqui-se de que a frequência do programa esteja em 48.000 Hz.

    Caso seu aplicativo não esteja configurado com a frequência correta você deve altera-lá clicando em **Preferred Main SampleRate** e selecionando **48.000 Hz**.

    ![Logo](images/vmb_hz.png)

Após seguir todos os passos corretamente, o seu **Voicemeeter Banana** estará devidamente configurado, agora falta configurar as opções de áudio do Windows.

## Configurando o Windows

Digite **Sons** na barra de pesquisa do Windows e abra as configurações de som.

![Logo](images/w_sounds.png)

1. Vá até **VoiceMeeter Aux Input** e clique duas vezes sobre ele.

   Feito isso, vá até **Avançado** e defina o formato padrão para **16 bit(s), 48000 Hz (Qualidade de DVD)**

   ![Logo](images/w_16bit.png)

2. Faça a mesma coisa para **VoiceMeeter Input**.

3. Clique com o botão direito sobre o **VoiceMeeter Input** e defina ele como **Dispositivo Padrão**.

4. Clique com o botão direito sobre o **VoiceMeeter Aux Input** e defina ele como **Dispositivo de Cominicação Padrão**.

   Seus dispositivos devem estar desta meneira:

   ![Logo](images/w_default.png)

5. Clique com o botão direito em **ambos VoiceMeeter** e clique em **Desabilitar** e na sequência **habilite** eles novamente.

6. Agora, vá até a aba **Gravação**.

7. Vá até **VoiceMeeter Aux Output** e clique duas vezes sobre ele.

   Feito isso, vá até **Avançado** e defina o formato padrão para **Canal 2, 16 bit(s), 48000 Hz (Qualidade de DVD)**

   ![Logo](images/w_2channel.png)

8. Faça a mesma coisa para **VoiceMeeter Output**.

9. Clique com o botão direito sobre o **VoiceMeeter Output** e defina ele como **Dispositivo Padrão** e **Dispositivo de Cominicação Padrão**.

   Seu dispositivo deve estar desta meneira:

   ![Logo](images/w_default2.png)

Feito isso, seu windows já esta configurado. O últimos passos são configurar a saída de **Música** e configurar a saída de **comunicação**. Para isso vou utilizar como exemplo o **Spotify** e o **Discord**.

## Configurando a Saída de Música

Para configurar a Saída de Música vou utilizar o **Spotify**, mas você pode fazer com qualquer outro aplicativo.

1. Abra o **Spotify** e reproduza uma música.

2. Vá ate as **configurações de sons do Windows**.

3. Selecione a opção **Volume do app e preferências do dispositivo**.

   ![Logo](images/w_sound_options.png)

4. Vá ate o **Spotify** e selecione a opção **CABLE Input (VB-Audio Virtual Cable)**.

   ![Logo](images/w_spotify.png)

Pronto, sua saída de música está configurada.

## Configurando a Saída de Comunicação

Para configurar a Saída de Comunicação vou utilizar o **Discord**, mas você pode fazer com qualquer outro aplicativo.

1. Abra o **Discord**.

2. Vá ate as configurações.

3. Localiza a configuração **Voz e Vídeo**.

   ![Logo](images/discord_settings.png)

4. Defina o dispositivo de entrada como **VoiceMeeter Output** e o de saída como **VoiceMeeter Aux Input**.

   ![Logo](images/discord_input_output.png)

Pronto, sua saída de música está configurada.

## Observações

- A atual versão do Voicemeeter Banana sofre com pequenas instabilidades, portanto se o seu áudio, por algum motivo, ficar estranho ou robotizado reinicie o aplicativo clicando em **MENU** e **Restart Audio Engine**.

- Se a sua voz no Discord, ou em seu aplicativo de comunicação estiver robotizada, siga estes passos:

  - Abra o gerenciador de tarefa e vá até **detalhes**.

  - Procure pelo serviço chamado **audiodg.exe**:

    ![Logo](images/audiodg.png)

  - Clique com o botão direito sobre ele.

  - Defina sua priotidade como **alta**:

    ![Logo](images/audiodg_priority.png)

  - Defina sua afinidade apenas com a **CPU 0**:

    ![Logo](images/audiodg_affinity.png)

## Referências

Para a construção deste repositório foram usadas as seguintes referências.

https://streamlabs.com/content-hub/post/split-audio-using-voicemeeter-banana

https://www.youtube.com/watch?v=0EjDL3BgPk4
