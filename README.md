# LIMA - Linguagem de Marcação

![LIMA](https://img.shields.io/badge/linguagem-marcação-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Sobre

**LIMA** é uma linguagem de marcação desenvolvida para estruturação de dados com foco em clareza, simplexidade e extensibilidade. Similar ao XML, LIMA oferece um formato textual para representar informações hierárquicas e estruturadas.

## Características

- ✅ **Sintaxe Clara e Intuitiva** - Tags descritivas e estrutura hierárquica
- ✅ **Baseada em XML** - Padrão estabelecido e amplamente adotado
- ✅ **Extensível** - Crie suas próprias tags e estruturas
- ✅ **Legível** - Formato de texto puro, fácil de ler e manter
- ✅ **Estruturada** - Suporta dados aninhados e complexos
- ✅ **Validável** - Pode ser validada contra esquemas

## Estrutura do Projeto

```
LIMA/
├── README.md
└── s1_at2_r1_lima/
    ├── ex01_CadastrodeLivro_XML/          # Cadastro de Livros
    ├── ex02_CadastrodeLAluno_XML/         # Cadastro de Alunos
    ├── ex03_CadastrodeEmpresa_XML/        # Cadastro de Empresas
    ├── ex04_PedidodeVenda_XML/            # Pedidos de Venda
    ├── ex05_CadastrodeProduto_XML/        # Cadastro de Produtos
    └── ex06_SistemaEscolar_XML/           # Sistema Escolar
```

## Sintaxe Básica

### Estrutura Fundamental

```xml
<?xml version="1.0" encoding="UTF-8"?>
<raiz>
    <elemento atributo="valor">
        Conteúdo de texto
    </elemento>
    <elemento_vazio />
</raiz>
```

### Elementos

- **Tags de abertura e fechamento**: `<tag>conteúdo</tag>`
- **Atributos**: `<tag atributo="valor">conteúdo</tag>`
- **Elementos vazios**: `<tag />`

### Exemplo Prático - Cadastro de Livro

```xml
<?xml version="1.0" encoding="UTF-8"?>
<livro id="001">
    <titulo>O Senhor dos Anéis</titulo>
    <autor>J.R.R. Tolkien</autor>
    <ano_publicacao>1954</ano_publicacao>
    <categoria>Ficção Científica</categoria>
    <preco moeda="BRL">89.90</preco>
</livro>
```

## Exemplos de Uso

### Cadastro de Aluno

```xml
<?xml version="1.0" encoding="UTF-8"?>
<aluno matricula="2024001">
    <nome>João Silva</nome>
    <data_nascimento>2005-03-15</data_nascimento>
    <email>joao.silva@escola.edu.br</email>
    <endereco>
        <rua>Rua Principal</rua>
        <numero>123</numero>
        <cidade>São Paulo</cidade>
        <estado>SP</estado>
    </endereco>
</aluno>
```

### Cadastro de Empresa

```xml
<?xml version="1.0" encoding="UTF-8"?>
<empresa cnpj="12.345.678/0001-99">
    <razao_social>Empresa LTDA</razao_social>
    <nome_fantasia>Empresa</nome_fantasia>
    <data_fundacao>2010-05-20</data_fundacao>
    <contatos>
        <telefone tipo="comercial">11-3456-7890</telefone>
        <email>contato@empresa.com.br</email>
    </contatos>
</empresa>
```

### Pedido de Venda

```xml
<?xml version="1.0" encoding="UTF-8"?>
<pedido numero="PED-2024-001" data="2024-01-15">
    <cliente id="001">João Silva</cliente>
    <itens>
        <item numero="1">
            <produto id="P001">Produto A</produto>
            <quantidade>5</quantidade>
            <valor_unitario>10.00</valor_unitario>
        </item>
    </itens>
    <total>50.00</total>
</pedido>
```

## Boas Práticas

### ✓ Recomendado

- Use nomes descritivos para tags
- Mantenha a estrutura hierárquica clara
- Indente corretamente o código
- Use atributos para metadados
- Documente suas estruturas customizadas

```xml
<!-- Bom -->
<estudante id="123">
    <informacoes_pessoais>
        <nome_completo>Maria Santos</nome_completo>
        <data_nascimento>2004-07-10</data_nascimento>
    </informacoes_pessoais>
</estudante>
```

### ✗ Evite

- Tags vagas ou ambíguas
- Estruturas muito profundas
- Misturar dados em texto com estrutura
- Inconsistência no nomeamento

```xml
<!-- Ruim -->
<dados>
    <d1>Maria</d1>
    <d2>
        <x>2004-07-10</x>
    </d2>
</dados>
```

## Exercícios Inclusos

1. **ex01_CadastrodeLivro_XML** - Estruturação de dados de livros
2. **ex02_CadastrodeLAluno_XML** - Dados estudantis e informações pessoais
3. **ex03_CadastrodeEmpresa_XML** - Informações corporativas
4. **ex04_PedidodeVenda_XML** - Processos comerciais
5. **ex05_CadastrodeProduto_XML** - Catálogo de produtos
6. **ex06_SistemaEscolar_XML** - Sistema completo de gestão escolar

## Ferramentas Úteis

- **Editores**: VS Code, Sublime Text, Notepad++
- **Validadores**: XSD (XML Schema Definition)
- **Parsers**: Bibliotecas para linguagens diversas (DOM, SAX)
- **Ferramentas Online**: XML Validators, Pretty Printers

## Conversão de Formatos

LIMA/XML pode ser facilmente convertido para:
- **JSON** - Formato alternativo moderno
- **CSV** - Para dados tabulares
- **SQL** - Para armazenamento em banco de dados
- **HTML** - Para apresentação em navegadores (via XSLT)

## Recursos Adicionais

- [XML W3C](https://www.w3.org/XML/)
- [XML Schema](https://www.w3.org/XML/Schema)
- [XSLT Transformações](https://www.w3.org/TR/xslt)

## Licença

Este projeto está sob licença MIT. Veja o arquivo LICENSE para mais detalhes.

## Autor

Desenvolvido como material educacional para aprendizado de linguagens de marcação.

---

**Última atualização**: Julho de 2026