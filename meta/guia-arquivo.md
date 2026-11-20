Como fiz recentemente um tutorial (bem decepcionante, diga-se de passagem) sobre [trabalho básico de tradução](https://github.com/cyprianscafe/cyprianscafe/blob/main/meta/guia-traducao.md), decidi que seria útil jogar alguma luz sobre aquilo em que 90% do meu tempo livre vai atualmente: arquivar, organizar e armazenar material online. Talvez no futuro eu faça um tutorial sobre como obter, armazenar, restaurar e arquivar adequadamente mídias físicas, mas não hoje. Hoje, estamos falando de acumulação digital.

Minhas credenciais: confia, mano. Além disso, eu arquivo material digital desde os 13 anos de idade. Atualmente, tenho quatro HDs externos abarrotados até a tampa de material religioso digital de várias partes do globo, e já fiz scraping do Internet Archive de forma tão minuciosa que o meu próprio chefe pediu meus arquivos pessoais quando o Wayback Machine saiu do ar por causa de um ataque DDoS em 2024. Já confia?

Agora, antes de entrarmos na parte prática de como fazer isso, precisamos ponderar algumas coisinhas. A primeira é que este não é um hobby barato. Não apenas exige dinheiro de verdade - não importa o quanto você tente economizar - como você também vai sangrar algo muito mais valioso: tempo. Não existe nível de automação que torne o arquivamento digital uma empreitada rápida, sem esforço e do tipo set it and forget it.

Segundo ponto: a menos que você tenha um método para a loucura, ou a menos que esteja fazendo simplesmente um arquivamento do tipo save-state (que é quando você baixa um site ou um lote de arquivos só para impedir que entrem em extinção), você vai acabar com um aterro sanitário digital gigantesco e impossível de pesquisar. Você precisa descobrir como organizar o seu tesouro e, como eu não sei quais são os seus objetivos específicos de pesquisa, você precisa fazer essa reflexão sozinho. É claro que eu ficaria feliz em ajudar você a fazer um brainstorming se quiser me mandar um e-mail, mas, fora isso, você precisa começar a esfregar os neurônios agora mesmo.

<p align="center">✧✧✧</p>

## Por onde começar

Antes de baixar um único PDF ou abrir um terminal, você precisa cravar quatro pontos inegociáveis: onde vai armazenar os dados salvos, que tipo de material está mirando, como vai organizá-lo e como pretende verificar se os seus arquivos não apodreceram na negligência.

### Onde armazenar os dados salvos

Vou dizer isso de peito aberto: **você precisa salvar os seus dados localmente**. Seja direto no seu computador (o que é uma péssima ideia, a menos que esteja salvando só um punhado de arquivos de texto ou páginas pequenas) ou em drives externos dedicados. A questão é a seguinte: se você vai investir dinheiro em algum momento do seu trabalho de arquivamento, faça isso aqui. Se você tentar comprar um HD externo de 2 TB na Shopee por 30 conto, vai descobrir do pior jeito que aquilo na verdade é um cartão SD de 16 GB colado com cola quente dentro de uma carcaça de chinesium, com firmware adulterado que sobrescreve os seus dados no segundo em que enche. Invista em uma marca legítima e de boa reputação, como Western Digital, Seagate ou Toshiba, e compre de um revendedor autorizado.

O motivo de eu ser tão taxativa sobre armazenamento local em vez de serviços de cloud é que a propriedade local é a própria essência do data hoarding em primeiro lugar. O data hoarding começou como um esforço de nerds difíceis de amar como moi, que perceberam que o internet estava constantemente à mercê da deterioração de servidores, da censura e da ganância por paywalls dos monopólios de tecnologia. Se você depende do Google Drive ou do Dropbox para abrigar o seu arquivo, está apenas confiando no próprio sistema que está tentando enganar.

E sim, não vamos ficar de rodeios: uma parte enorme do trabalho de arquivamento é pirataria. Provedores de cloud escaneiam hashes, encerram contas sem aviso prévio, mudam suas faixas de preço da noite para o dia ou simplesmente vão à falência. Mantenha as mãos no seu próprio hardware.

Ao comprar drives, preste atenção às especificações técnicas chatas. Para cold storage (arquivos que você salva e acessa apenas ocasionalmente), os discos rígidos mecânicos tradicionais (HDDs) oferecem o melhor custo-benefício por terabyte. Os solid-state drives (SSDs) são mais rápidos e menos frágeis se caírem, mas são mais caros e armazenam dados através de carga elétrica - se ficarem desconectados por anos a fio (especialmente em locais quentes como o Brazeel), essa carga vaza e você pode perder seus arquivos. Antes de jogar um único arquivo em um drive novo, formate-o em um sistema de arquivos confiável, como NTFS (se você usa estritamente Windows) ou exFAT (se transita entre Windows, Mac e Linux - apenas tome cuidado para nunca puxar o cabo durante uma transferência, já que o exFAT não tem proteção nativa contra quedas de energia). Se um dia você evoluir para um servidor Linux ou NAS dedicado (super recomendo, Linux FTW), migre para sistemas modernos e inifinitamente superiores como ZFS ou Btrfs, que previnem corrupção automaticamente. Independentemente do sistema, rode uma verificação inicial de saúde no disco novo usando uma ferramenta gratuita como o CrystalDiskInfo para ter certeza de que não comprou uma bombinha.

Por fim, mantenha a "regra 3-2-1" no fundo da mente: três cópias dos seus dados, em dois tipos diferentes de mídia, com pelo menos uma mantida fora do local físico (ou ao menos em uma caixa à prova de fogo separada se você é exagerada igual eu). No mínimo, compre drives aos pares para que o seu drive principal tenha um backup gêmeo e e nunca copie e cole pastas na mão para sincronizá-los; use ferramentas como FreeFileSync ou Rclone para espelhar apenas o que mudou sem criar bagunça.

### O que salvar

Embora seja crucial decidir o que você vai arquivar, saiba que, para 90% das pessoas, o seu escopo vai sofrer mutações com o tempo. Normalmente, começamos salvando coisas que são pessoalmente urgentesantes de perceber o quão frágil a web é e sair salvando em pânico tudo o que estiver ao redor.

Para não se afogar, defina o seu escopo antes de começar a fazer scraping. Você está coletando fontes primárias ou fontes analíticas secundárias? Material religioso é singularmente vulnerável porque pequenas congregações, pesquisadores independentes e fóruns de nicho deixam o registro de domínio expirar o tempo todo, varrendo décadas de história comunitária do mapa de um dia para o outro. Priorize primeiro o material "ameaçado de extinção" antes de se preocupar em baixar PDFs acadêmicos tradicionais que já existem em cinquenta servidores universitários.

À medida que a sua coleção cresce por diferentes subtemas, você precisará decidir como particionar o seu espaço físico. Alguns arquivistas preferem segregação física: um drive estritamente para textos litúrgicos primários e áudio, outro drive para sociologia e história acadêmicas, e um terceiro para scrapes bagunçados da web. Outros preferem comprar drives de altíssima capacidade e manter tudo junto sob uma arquitetura de pastas unificada. Se os seus interesses forem radicalmente distintos - e.g., você arquiva tanto jurisprudência islâmica do século XIX quanto rips de VHS de televangelistas modernos -, separá-los por drive torna os backups e o transporte muito mais fáceis.

### Organização

Esta é, e eu não exagero nem um pouco, a parte mais difícil de todo o hobby. Você tem essencialmente duas escolhas dolorosas: pode ordenar as coisas automaticamente usando scripts e regras de metadados, o que é rápido mas propenso a erros hilariamente idiotas, ou pode fazer isso manualmente, o que é preciso mas vai consumir o seu tempo de vida. Ou, é claro, você pode não fazer nenhum dos dois e viver como um dragão acumulando ouro.

Eu, pessoalmente, uso uma abordagem híbrida. Tenho um algoritmo de triagem amplo e geral que lança uma rede bem aberta - pescando arquivos por palavra-chave, extensão de arquivo ou domínio - e os despeja em uma pasta de preparação. Em seguida, rodo um script personalizado para separar alguns milhares de itens por vez em caixas aproximadas, passo um limpador de arquivos duplicados (recomendo o Czkawka) para eliminar tralha repetida que veio com nomes diferentes e, a partir daí, faço a ordenação manualmente em lotes, inspecionando anomalias esquisitas uma por uma. E sim, é geralmente aí que começo a xingar D'us por ter me dado esse tipo de autismo, em vez de fazer com que eu fosse super fã de Sonic ou algo do tipo.

O segredo para uma organização sã é uma convenção de nomenclatura rígida e uma árvore de pastas rasa. Evite aninhar pastas com doze níveis de profundidade; isso transforma a busca em um pesadelo e pode, de fato, quebrar caminhos de arquivo no Windows se a contagem de caracteres ficar longa demais. Em vez disso, monte uma hierarquia de topo previsível - como `Tradicao-ou-Topico > Tipo-de-Fonte > Ano` - e deixe os nomes descritivos dos arquivos fazerem o trabalho pesado. Um formato padrão como `AAAA-MM-DD_Autor-ou-Instituicao_Titulo-do-Documento_Idioma.ext` garante que os seus arquivos sejam ordenados cronologicamente por padrão e continuem identificáveis mesmo se forem separados das pastas-pai. Se você estiver arquivando PDFs digitalizados de livros religiosos antigos ou panfletos, passe-os por uma ferramenta de Reconhecimento Óptico de Caracteres (OCR), como OCRmyPDF ou Adobe Acrobat, para que o texto interno se torne pesquisável; um PDF de imagem não pesquisável é só um pouquinho melhor do que não ter o arquivo nenhum.

Quando sua coleção chegar na casa dos milhões de arquivos, abandone a busca nativa do Windows. Instale o Everything (para achar nomes de arquivos instantaneamente) ou o Recoll (para pesquisar palavras dentro do texto de milhares de PDFs e e-books ao mesmo tempo). Se você lida com bibliotecas gigantescas de livros e artigos, gerenciadores como Calibre ou Zotero também salvam vidas. Embora - e eu possa soar como uma nerd roliça e pedante... - eu recomendo abandonar o Windows hoje mesmo. É um OS babaca ultrapassado, repleto de bloatware e totalmente inútil para um arquivista. Mude para o Linux hoje e afaste-se dos descrentes!! PRAISE LINUX!!

### Manutenção, bit rot e recuperação

Depois que os seus arquivos são baixados e arrumados bonitinhos nas pastas, o seu trabalho ainda não acabou de fato. Discos rígidos se degradam com o tempo, e os arquivos podem sofrer de bit rot, em que setores magnéticos enfraquecem e bits individuais invertem sozinhos (tipo Kuru de arquivos), corrompendo um PDF ou arquivo de áudio sem que você perceba até tentar abri-lo cinco anos depois. 

Para combater isso, faça três coisas:

1. Gere checksums (como hashes SHA-256) para as suas pastas principais usando ferramentas como HashMyFiles ou comandos nativos do terminal. Um checksum funciona como uma impressão digital; se você o conferir um ano depois e a impressão tiver mudado, sabe que o arquivo está corrompido.
2. Apenas saber que um arquivo corrompeu não resolve nada se o seu backup também tiver ido pro espaço. Use ferramentas como MultiPar (Windows) ou `par2cmdline` (Linux/Mac) para gerar arquivos de recuperação `.par2` ocupando cerca de 5% a 10% do tamanho da pasta. Se um arquivo de 10 GB sofrer bit rot e perder alguns megabytes, o arquivo de paridade consegue reconstruir matematicamente os dados perdidos.
3. Nunca deixe um HD parado dentro de um armário por cinco anos seguidos, pelamor. Ligue os seus drives a cada seis meses e rode um teste de leitura completa (como um teste SMART estendido ou verificação de superfície).

<p align="center">✧✧✧</p>

## Como conseguir material

Então, você já sabe mais ou menos o que quer arquivar, sabe onde vai armazenar e tem um plano para organizar. Agora vem a parte realmente divertida: como arrancar esse material da internet e jogar nos seus drives?

A sua abordagem vai se resumir a três métodos principais, cada um com o seu próprio tipo de sofrimento:

* **Salvamento manual:** É a abordagem de tiozão de clicar com o botão direito e salvar, complementada por extensões de navegador como o SingleFile (que empacota uma página inteira, incluindo imagens e CSS, em um único arquivo HTML limpo para não quebrar offline) ou o yt-dlp usado uma URL por vez para palestras religiosas, cânticos e sermões. O salvamento manual dá precisão total e zero arquivos inúteis, tornando-o ideal para artigos acadêmicos selecionados a dedo ou páginas específicas. O contra óbvio é que é de matar por dentro de tão lento se você precisar pegar um site inteiro ou uma biblioteca enorme de PDFs.
* **Scraping e crawling automatizados:** Quando você precisa de um fórum inteiro, de um diretório completo de textos digitalizados ou de milhares de resultados de busca, você tira a artilharia pesada. Ferramentas de linha de comando como wget ou httrack conseguem espelhar sites estáticos antigos inteiros, preservando a estrutura de links para navegação offline. Para sites carregados de mídia, gallery-dl e yt-dlp (alimentados com um arquivo de texto cheio de links) arrancam canais inteiros, playlists e image boards embutindo metadados automaticamente. E se você esbarrar em sites modernos pesados em JavaScript (onde o wget falha) ou quiser salvar no formato padrão ouro dos arquivistas profissionais (WARC), use ferramentas como ArchiveBox ou Browsertrix Crawler. Por fim, se o seu alvo for código ou documentação no GitHub, não faça scraping web: use `git clone --mirror` para baixar o repositório inteiro com todo o histórico de versões. Os prós da automação são a velocidade bruta e a completude; os contras são que scrapers mal configurados baixam alegremente gigabytes de banners inúteis e loops de redirecionamento quebrados.
* **Arquivamento por terceiros:** Às vezes, a sua própria largura de banda não dá conta, ou um site está morrendo ativamente enquanto você está longe do compiurer. Enviar URLs para o Wayback Machine ou para o Archive.today joga o trabalho pesado para os servidores deles, criando um snapshot público que você pode baixar localmente depois. É uma ótima rede de segurança, embora você não deva depender exclusivamente disso, já que arquivos de terceiros podem ser atingidos por pedidos de remoção ou quedas de servidor.

Eu, por mim, uso uma combinação dos três, embora me apoie pesadamente em fazer scraping do Internet Archive com base em palavras-chave específicas - já que, no fim das contas, o meu foco principal é o arquivamento religioso. Porém, assim que você começa a automatizar requisições contra o Internet Archive (ou Wikipédia, ou repositórios acadêmicos), vai dar de cara com um muro: rate limits. Se disparar um script que martela os servidores deles rápido demais, você vai levar um erro `HTTP 429: Too Many Requests` num piscar de olhos, e o seu IP pode até pegar um banimento temporário.

O melhor jeito de evitar isso é configurar os seus scrapers para serem educados - adicione um parâmetro de sleep de 2 a 5 segundos entre as requisições, para parecer um humano rápido em vez de um ataque DDoS. Além disso, no caso específico do Internet Archive, crie uma conta gratuita e faça login na ferramenta de linha de comando (`ia configure`). Usuários autenticados ganham limites de requisição bem mais folgados e acesso a itens que ficam bloqueados para anônimos (e, se puder, doe uns trocados para ajudar a manter os servidores deles vivos, porque eles merecem).

O scraping automático é imensamente mais rápido do que ficar clicando por aí manualmente, sim, mas configurá-lo é um penhasco íngreme se você nunca encostou em uma linha de comando antes. Eu não posso dar um tutorial genérico sobre como configurar um scraper porque não conheço o seu sistema operacional, o seu nível de familiaridade com código ou a arquitetura exata dos sites que você está mirando. No entanto, você não precisa de um diploma de ciência da computação para dar um jeito nisso.

Comece pesquisando no GitHub ou em comunidades do Reddit como r/DataHoarder e r/Archiveteam usando o nome da plataforma em que você quer fazer scraping mais a palavra "scraper" ou "archiver" - há boas chances de algum gênio já ter escrito um script em Python específico para aquele site. Quando inevitavelmente der de cara com mensagens de erro, copie e cole o erro exato em um buscador ou peça a uma IA para explicar quais flags você precisa ajustar.

<p align="center">✧✧✧</p>

## Kit de ferramentas essencial para iniciantes

Se você quiser começar a montar o seu cinto de utilidades hoje mesmo, procure por estas ferramentas específicas:

* **SingleFile:** Essencial para salvar artigos individuais, posts de blog e tópicos de fórum como arquivos HTML limpos e autocontidos, sem nenhuma imagem quebrada.
* **Wget/HTTrack/ArchiveBox:** As ferramentas ideais para espelhar sites inteiros - use Wget/HTTrack para sites estáticos antigos e ArchiveBox (com formato WARC) para páginas modernas e complexas.
* **Internet Archive CLI (ia):** A ferramenta oficial de linha de comando para baixar (e enviar) coleções do Archive.org em massa usando consultas por palavras-chave e metadados.
* **JDownloader 2:** Um gerenciador de downloads gráfico que é fantástico para iniciantes que ainda não estão prontos para o terminal; copie uma página cheia de links de PDF ou MP3, e ele vai farejá-los e colocá-los na fila automaticamente.
* **OCRmyPDF:** Uma tábua de salvação para transformar livros religiosos e documentos históricos escaneados, só em imagem, em PDFs totalmente pesquisáveis por texto.
* **FreeFileSync/Rclone:** Indispensáveis para sincronizar seu HD principal com seu HD de backup sem cometer erros humanos.
* **Czkawka:** Um caçador de arquivos duplicados ultrarrápido para limpar tralha repetida depois de grandes sessões de download.
* **MultiPar (PAR2):** A ferramenta que cria arquivos de paridade capazes de consertar arquivos corrompidos pelo bit rot.
* **Everything/Recoll:** Buscadores locais instantâneos para encontrar qualquer arquivo ou palavra perdida dentro de milhões de documentos.

Comece pequeno. Escolha um site ameaçado de extinção, uma biblioteca digital obscura ou um canal do YouTube que partiria o seu coraçãozinho se sumisse amanhã, e salve direito. Quando você sentir a satisfação presunçosa de abrir um arquivo guardado localmente cinco anos depois de o site original ter saído do ar, nunca mais vai olhar para a internet do mesmo jeito. E lembre-se:

```
                .88888888:.
               88888888.88888.
             .8888888888888888.
             888888888888888888
             88' _`88'_  `88888
             88 88 88 88  88888
             88_88_::_88_:88888
             88:::,::,:::::8888
             88`:::::::::'`8888
            .88  `::::'    8:88.
           8888            `8:888.
         .8888'             `888888.
        .8888:..  .::.  ...:'8888888:.
       .8888.'     :'     `'::`88:88888
      .8888        '         `.888:8888.
     888:8         .           888:88888
   .888:88        .:           888:88888:
   8888888.       ::           88:888888
   `.::.888.      ::          .88888888
  .::::::.888.    ::         :::`8888'.:.
 ::::::::::.888   '         .::::::::::::
 ::::::::::::.8    '      .:8::::::::::::.
.::::::::::::::.        .:888:::::::::::::
:::::::::::::::88:.__..:88888:::::::::::'
 `'.:::::::::::88888888888.88:::::::::'
       `':::_:' -- '' -'-' `':_::::'`

███████ ██    ██  ██████ ██   ██                          
██      ██    ██ ██      ██  ██                           
█████   ██    ██ ██      █████                            
██      ██    ██ ██      ██  ██                           
██       ██████   ██████ ██   ██                          
                                                          
                                                          
██     ██ ██ ███    ██ ██████   ██████  ██     ██ ███████ 
██     ██ ██ ████   ██ ██   ██ ██    ██ ██     ██ ██      
██  █  ██ ██ ██ ██  ██ ██   ██ ██    ██ ██  █  ██ ███████ 
██ ███ ██ ██ ██  ██ ██ ██   ██ ██    ██ ██ ███ ██      ██ 
 ███ ███  ██ ██   ████ ██████   ██████   ███ ███  ███████ 
                                                          
                                                          
██████  ██████   █████  ██ ███████ ███████                
██   ██ ██   ██ ██   ██ ██ ██      ██                     
██████  ██████  ███████ ██ ███████ █████                  
██      ██   ██ ██   ██ ██      ██ ██                     
██      ██   ██ ██   ██ ██ ███████ ███████                
                                                          
                                                          
██      ██ ███    ██ ██    ██ ██   ██ ██                  
██      ██ ████   ██ ██    ██  ██ ██  ██                  
██      ██ ██ ██  ██ ██    ██   ███   ██                  
██      ██ ██  ██ ██ ██    ██  ██ ██                      
███████ ██ ██   ████  ██████  ██   ██ ██                  
                                                          
                                                          

