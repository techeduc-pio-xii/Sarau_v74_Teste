Meu Livro Ganha Vida - Sarau | Vídeos locais e projetos portáteis

VÍDEOS ORIGINAIS NA ABA "VÍDEOS"
- Na aba "Vídeos", toque em "Selecionar vídeo".
- Escolha um vídeo salvo em Arquivos ou Fotos do iPad (MP4/MOV compatível).
- O Chroma Key é processado localmente no próprio iPad/navegador.
- A aplicação mantém uma cópia local separada do vídeo original no IndexedDB do Safari/PWA.
- O vídeo não é enviado para servidores externos.
- É possível manter vários vídeos no mesmo iPad e escolher entre eles pela lista "Vídeos já salvos neste iPad".

SALVAR E ABRIR PROJETOS COM O VÍDEO
- O botão "Salvar" gera um pacote ZIP do projeto.
- Dentro do ZIP, o arquivo projeto.json guarda a composição, os quadros, as referências aos elementos e a narração.
- Se o projeto utilizar um vídeo, o original acompanha o ZIP como arquivo separado em midia/video-original.ext.
- O vídeo não é incorporado ao JSON nem convertido em base64: permanece como arquivo independente dentro do pacote.
- Ao abrir o ZIP em outro iPad, a aplicação importa o vídeo para o armazenamento local daquele aparelho e restaura o projeto com o vídeo associado.
- Projetos JSON antigos continuam podendo ser abertos. Se dependerem de um vídeo que não esteja salvo naquele iPad, será necessário selecioná-lo novamente.
- O ZIP é armazenado sem compactação dos vídeos para evitar processamento desnecessário e reduzir o tempo de espera. Portanto, o tamanho do pacote será próximo ao tamanho do vídeo original.

PUBLICAÇÃO E USO
- Publique a pasta em um endereço HTTPS (por exemplo, GitHub Pages).
- Abra o endereço pelo Safari no iPad.
- Na primeira utilização, adicione a aplicação à Tela de Início, se desejar.
- Para gravar narração pelo microfone, o navegador precisa estar em HTTPS e receber permissão de microfone.

PRIVACIDADE E LIMITAÇÕES
- O código desta versão não envia os vídeos selecionados para APIs ou servidores externos.
- A cópia de trabalho fica no armazenamento do Safari/PWA daquele iPad e perfil do navegador.
- O pacote ZIP salvo pelo usuário contém o projeto e o vídeo original; deve ser guardado em local aprovado pela instituição, pois pode conter imagem e voz de alunos.
- O navegador pode remover dados locais em situações de falta de espaço, limpeza de dados ou gerenciamento do dispositivo. A aplicação solicita persistência quando disponível, mas isso não substitui backup.
- A versão limita o vídeo selecionado a 500 MB. Recomenda-se utilizar vídeos curtos e comprimidos.
- Testar importação/exportação de ZIP, formatos MP4/MOV, áudio, exportação e desempenho do Chroma Key em cada modelo de iPad antes do uso com alunos.
