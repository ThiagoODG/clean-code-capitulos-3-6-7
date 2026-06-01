📚 Reflexões sobre Clean Code: Funções, Objetos e Tratamento de Erros
Recentemente, realizei a leitura dos capítulos 3, 6 e 7 do livro Clean Code de Robert C. Martin, uma das principais referências quando o assunto é desenvolvimento de software de qualidade.
Embora muitas vezes a pressão por entregar funcionalidades rapidamente faça com que o foco esteja apenas em "fazer funcionar", a leitura desses capítulos reforça uma ideia importante: código é lido muito mais vezes do que é escrito. Por isso, escrever código limpo não é apenas uma boa prática, mas uma responsabilidade com os futuros mantenedores do sistema — incluindo nós mesmos.
________________________________________
🔹 Capítulo 3 — Funções
O capítulo sobre funções apresenta um princípio simples, mas extremamente poderoso: uma função deve fazer apenas uma coisa, e fazê-la bem.
Ao longo da leitura, fica claro que funções pequenas e com responsabilidades bem definidas tornam o código mais fácil de entender, testar e modificar. Além disso, nomes claros e descritivos ajudam a transformar o código em uma espécie de documentação natural.
Principais aprendizados
•	Criar funções curtas e objetivas. 
•	Evitar excesso de parâmetros. 
•	Utilizar nomes que expressem claramente a intenção da função. 
•	Separar responsabilidades. 
•	Reduzir efeitos colaterais desnecessários. 
Exemplo
❌ Menos legível:
public void processarUsuario(Usuario usuario) {
    validar(usuario);
    salvar(usuario);
    enviarEmail(usuario);
}
✅ Mais organizado:
public void cadastrarUsuario(Usuario usuario) {
    validarUsuario(usuario);
    salvarUsuario(usuario);
    notificarCadastro(usuario);
}
A diferença pode parecer pequena, mas a intenção do código fica muito mais evidente.
________________________________________
🔹 Capítulo 6 — Objetos e Estruturas de Dados
Neste capítulo, o autor explora a diferença entre objetos e estruturas de dados, um conceito fundamental para quem trabalha com programação orientada a objetos.
Objetos devem encapsular informações e disponibilizar comportamentos. Já estruturas de dados servem principalmente para armazenar e transportar informações.
O grande aprendizado aqui é compreender que expor detalhes internos de um objeto cria dependências desnecessárias e aumenta o acoplamento entre componentes.
Principais aprendizados
•	Priorizar encapsulamento. 
•	Trabalhar com abstrações. 
•	Evitar dependências excessivas. 
•	Reduzir o acoplamento entre módulos. 
•	Tornar o sistema mais flexível para futuras alterações. 
Quando os objetos escondem seus detalhes internos e expõem apenas comportamentos necessários, o sistema se torna mais resistente a mudanças.
________________________________________
🔹 Capítulo 7 — Tratamento de Erros
O tratamento de erros é frequentemente tratado como algo secundário durante o desenvolvimento, mas este capítulo mostra que ele é parte fundamental da qualidade do software.
Um dos conceitos mais marcantes é que o fluxo principal da aplicação deve permanecer limpo e fácil de entender. Quando a lógica de negócio fica misturada com diversas verificações de erro, o código se torna confuso e difícil de manter.
Principais aprendizados
•	Utilizar exceções em vez de códigos de erro. 
•	Criar mensagens de erro claras e úteis. 
•	Evitar retornar valores null sempre que possível. 
•	Separar a lógica principal do tratamento de exceções. 
•	Facilitar a identificação e correção de problemas. 
Exemplo
❌ Retornando código de erro:
if (usuario == null) {
    return -1;
}
✅ Utilizando exceção:
if (usuario == null) {
    throw new UsuarioNaoEncontradoException();
}
Dessa forma, o código principal permanece mais limpo e a responsabilidade pelo tratamento do erro fica centralizada.
________________________________________
💡 Minha reflexão
A leitura desses capítulos reforçou uma percepção importante: escrever código limpo não significa apenas seguir padrões ou regras estéticas. Trata-se de criar soluções que possam ser compreendidas, evoluídas e mantidas por outras pessoas ao longo do tempo.
Funções pequenas, objetos bem encapsulados e um tratamento de erros consistente contribuem diretamente para a construção de sistemas mais confiáveis e sustentáveis.
Muitas vezes, a diferença entre um projeto fácil e um projeto difícil de manter não está na tecnologia utilizada, mas na qualidade das decisões tomadas durante a escrita do código.
Como desenvolvedores, não escrevemos software apenas para computadores executarem. Escrevemos, principalmente, para que outros desenvolvedores consigam compreender o que foi construído.
________________________________________
📖 Referência
Clean Code: A Handbook of Agile Software Craftsmanship
Autor: Robert C. Martin
