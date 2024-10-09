# resumo_lab_6
Armazenamento no Azure

Bootcamp DIO Microsoft Azure Essentials - AZ-900

Serviços de Armazenamento (Storage Account) deve ter um nome único e exclusivo global (3 à 24 caracteres, letras minusculas e nº), acesso à internet, determinar serviços e redundâncias.
- Redundância de armazenamento: LRS Armazenamento de Redundância Local (Datacenter individual na região primária) Durabilidade 11 noves; ZRS de Zonas (3 Zonas de disponibilidade na região primária durabilidade 12 noves; GRS Geográfica (Datacenter único no primário e região secundária) 16 noves de durabilidade; GZRS Armazenamento de Redundância de Zona Geográfica (3 Zonas de dispinibilidade na região primária e um único datacenter na região secundária, 16 noves de durabilidade.
- Serviços de Armazenamento:
    - Blob do Azure: otimizado para armazenar quantidades massiva de dados não estruturados, como textos e dados binários. Modelo mais usado nas aplicações.
    - Discos do Azure: fornece discos para máquinas virtuais, aplicativos para outros serviços acessarem e utilizarem.
    - Fila do Azure: armazenamento de mensagem que fornece armazenamento e recuperação com configuração de destino para grandes quantidades de mensagens, cada uma com 64kb 
    - Files (Arquivos): configura armazenamento de arquivos de rede com alta disponibilidade, usar o protocolo de Blocos de Mensagens do Sevidor (mapeamento config. compartilhada de rede)
    - Tabelas do Azure: fornece uma opção de chave/atributo para armazenamento de dados estruturados não relacionaiscom um design sem esquema.
- Pontos de Extremidade Públicos do Serviço de Armazenamento:
    - Armazenamento de Blobs http://<storage-account-name>.blob.core.windows.net;
    - Data lake Gen2 http://<storage-account-name>.dfs.core.windows.net;
    - Arquivos do azure http://<storage-account-name>.file.windowns.net;
    - Armazenamento de filas http://<storage-account-name>queue.core.windowns.net;
    - Armazenamento de tabelas hrrp://<storage-account-name>.table.core.windows.net.
- Camadas de acesso de armazenamento do Azure:
  -- Frequente (dados acessados com frequência;
  -- Esporádico (dados acessados pouca frequência por pelo menos 30 dias);
  -- Frio (pouco frequente, armazenados por pelo menos 90 dias) e
  -- Arquivo Morto (rara frequência, armazenados por 180 dias).
- Migração do Azure: Azure Data Box (planos de 40 á 80TB) para locais remotos com pouca ou sem conectividade, servidor físico;
- Gerenciamento de Arquivos:
    - AzCopy utilitário de linha de comando, copiados para os Blobs ou arquivos ou para sua conta, sincronização em uma direção;
    - Gerenciador de Armazenamento do Azure: faz a cópia, move do seu computador para nuvem. Interface gráfica do usuário, baixar arquivo (semelhante ao Windows Explore) compatível sistema operacional Linux, Windows ou MacOS.
    - Sincronização de Arquivos do Azure: Sincronização (local e Azure) de forma bidirecional, mantém os arquivos acessados com frequência local enquanto libera espaço.
