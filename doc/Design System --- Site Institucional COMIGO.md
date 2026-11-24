# **Design System \--- Site Institucional COMIGO**

**Versão:** 1.0  
**Objetivo:** definir padrões visuais e componentes reutilizáveis para o  
site institucional da COMIGO, mantendo integralmente a identidade visual  
informada.

## **Princípios do sistema**

* Preservar as cores, tipografias e o logotipo oficial da COMIGO.  
* Usar os padrões de forma consistente em todas as páginas.  
* Priorizar legibilidade, acessibilidade e navegação simples.  
* Criar componentes reutilizáveis e fáceis de implementar em CSS ou  
  Tailwind CSS.  
* Não redesenhar, recolorir, distorcer ou alterar as proporções do  
  logotipo oficial.

## **1\. Paleta de cores**

### **Cores da identidade visual**

---

Token HEX Uso

---

`color-primary` `#006633` Cor principal, links e  
ações primárias

`color-secondary` `#F4C300` Destaques e ações  
secundárias

`color-green-dark` `#0B3D2E` Fundos institucionais,  
cabeçalho ou rodapé

`color-green-light` `#4CAF50` Ícones, detalhes e  
elementos  
complementares

`color-natural-white` `#F8F8F5` Fundo claro de páginas  
e seções

## **`color-graphite` `#1A1A1A` Texto principal**

### **Cores funcionais de interface**

As cores funcionais complementam a interface e não substituem as cores  
da marca.

Token HEX Uso

---

`color-surface` `#FFFFFF` Cards, campos e superfícies  
`color-text-muted` `#666666` Texto secundário  
`color-border` `#E2E5E1` Bordas e divisórias  
`color-success` `#237A45` Confirmação de sucesso  
`color-error` `#B42318` Erros e validação  
`color-warning` `#8A5A00` Avisos  
`color-info` `#245C9C` Informações

**Orientação:** utilizar o verde COMIGO como cor de ação principal e o  
amarelo para realces. Evitar texto branco sobre amarelo; usar texto  
grafite para manter contraste.

## **2\. Tipografia**

* **Títulos:** Montserrat.  
* **Textos, menus, formulários e botões:** Roboto.  
* **Fallback de títulos:** `Arial, sans-serif`.  
* **Fallback de textos:** `Arial, sans-serif`.

### **Hierarquia tipográfica**

Elemento Desktop Tablet Mobile Peso

---

H1 48px 40px 32px 700  
H2 36px 32px 28px 700  
H3 28px 24px 22px 600  
H4 22px 20px 18px 600  
H5 18px 18px 16px 600  
Parágrafo 16px 16px 16px 400  
Texto pequeno 14px 14px 14px 400  
Legenda 12px 12px 12px 400

### **Regras de tipografia**

* Títulos: line-height entre `1.2` e `1.3`.  
* Parágrafos: line-height `1.6`.  
* Menus e botões: line-height `1.4`.  
* Evitar parágrafos muito largos; largura recomendada de leitura:  
  `60ch` a `75ch`.  
* Usar pesos `400`, `500`, `600` e `700`.  
* Não utilizar letras maiúsculas em frases longas.

## **3\. Botões**

### **Botão primário**

* Fundo: `#006633`.  
* Texto: `#FFFFFF`.  
* Altura mínima: `48px`.  
* Padding horizontal: `24px`.  
* Border radius: `8px`.  
* Fonte: Roboto, `16px`, peso `600`.

### **Botão secundário**

* Fundo: `#F4C300`.  
* Texto: `#1A1A1A`.  
* Mesma altura, espaçamento e tipografia do botão primário.

### **Botão outline**

* Fundo transparente.  
* Borda: `1px solid #006633`.  
* Texto: `#006633`.  
* Hover com fundo verde muito claro, mantendo contraste.

### **Estados dos botões**

---

Estado Estilo

---

Default Cores padrão do tipo de botão

Hover Verde profundo no primário; amarelo  
ligeiramente escurecido no  
secundário

Focus-visible Contorno de foco visível de 3px,  
com afastamento de 2px

Active Fundo mais escuro e leve redução  
visual, sem deslocamento excessivo

Disabled Opacidade reduzida, cursor  
desativado e sem ação

## **Loading Indicador de carregamento e botão**

## **temporariamente desativado**

Transição recomendada: `200ms ease`.

## **4\. Formulários**

### **Campos padrão**

* Altura: `48px`.  
* Textarea: altura mínima `120px`.  
* Padding: `12px 16px`.  
* Borda: `1px solid #E2E5E1`.  
* Border radius: `8px`.  
* Fundo: `#FFFFFF`.  
* Texto: `#1A1A1A`.  
* Placeholder: `#666666`.  
* Espaçamento entre campos: `16px`.

### **Regras**

* Cada campo deve possuir label visível.  
* Placeholder não deve substituir o label.  
* Campos obrigatórios devem ser identificados.  
* Mensagens de erro devem explicar como corrigir o problema.  
* Em erro, usar borda `#B42318` e texto de apoio correspondente.  
* Em foco, destacar a borda verde e exibir indicador acessível.  
* Botões de envio devem seguir o padrão de botão primário.

## **5\. Cards e elementos reutilizáveis**

### **Card padrão**

* Fundo: `#FFFFFF`.  
* Borda: `1px solid #E2E5E1`.  
* Border radius: `12px`.  
* Padding: `24px`.  
* Sombra: `0 2px 6px rgba(0, 0, 0, 0.06)`.  
* Título: Montserrat, `20px`, peso `600`.  
* Texto: Roboto, `16px`, line-height `1.6`.  
* Imagens: proporção `16:9`, com `object-fit: cover`.

### **Variações**

* **Card de serviço:** ícone ou imagem, título, descrição e link.  
* **Card de notícia:** imagem, categoria, data, título e link "Leia  
  mais".  
* **Card institucional:** imagem, título e resumo.  
* **Card de destaque:** fundo verde profundo, texto branco e CTA.  
* **Card de estatística:** número em destaque, rótulo e descrição  
  curta.

### **Componentes reutilizáveis**

Componente Descrição

---

`Header` Logotipo, navegação e CTA  
`Footer` Informações institucionais, contatos e redes sociais  
`Hero` Imagem de destaque, título, texto e CTA  
`SectionTitle` Título e descrição de seção  
`Button` Botões primários, secundários e outline  
`ServiceCard` Card de serviço  
`NewsCard` Card de notícia  
`InstitutionalCard` Card institucional  
`Breadcrumb` Caminho de navegação  
`FormField` Campo de formulário com label e validação  
`ContactInfo` Dados de contato  
`Pagination` Paginação de notícias  
`Badge` Categoria ou etiqueta  
`Modal` Janela de confirmação ou informação

## **6\. Bordas, sombras e espaçamentos**

### **Border radius**

Token Valor

---

`radius-sm` 4px  
`radius-md` 8px  
`radius-lg` 12px  
`radius-xl` 16px  
`radius-pill` 999px

### **Sombras**

```
--shadow-sm: 0 2px 6px rgba(0, 0, 0, 0.06);
--shadow-md: 0 4px 16px rgba(0, 0, 0, 0.10);
--shadow-lg: 0 8px 24px rgba(0, 0, 0, 0.14);
```

### **Escala de espaçamento**

Token Valor

---

`space-1` 4px  
`space-2` 8px  
`space-3` 12px  
`space-4` 16px  
`space-5` 24px  
`space-6` 32px  
`space-7` 48px  
`space-8` 64px  
`space-9` 96px

Usar essa escala para margens, paddings, distância entre seções e  
espaçamento interno de componentes.

## **7\. Responsividade**

### **Breakpoints**

Nome Largura

---

`sm` 640px  
`md` 768px  
`lg` 1024px  
`xl` 1280px  
`2xl` 1536px

### **Regras**

* Mobile: conteúdo em uma coluna e navegação compacta.  
* Tablet: usar duas colunas quando houver espaço adequado.  
* Desktop: utilizar grid de até 12 colunas.  
* Cards: três colunas no desktop, duas no tablet e uma no mobile.  
* Imagens devem manter proporção e não deformar.  
* Botões podem ocupar largura total no mobile.  
* Formulários devem ser organizados em uma coluna em telas pequenas.  
* Evitar rolagem horizontal.  
* Alvos de toque devem ter pelo menos `44px` de altura/largura.

### **Container**

```
.container {
  width: 100%;
  max-width: 1200px;
  margin-inline: auto;
  padding-inline: 24px;
}

@media (max-width: 767px) {
  .container {
    padding-inline: 16px;
  }
}
```

## **8\. Componentes por página**

---

Página Componentes

---

Início Header, Hero, SectionTitle,  
ServiceCard, NewsCard, CTA, Footer

Sobre a COMIGO Header, Breadcrumb, SectionTitle,  
InstitutionalCard, imagens, Footer

Produtos e Serviços Header, Breadcrumb, ServiceCard,  
Button, Footer

Notícias Header, Breadcrumb, NewsCard,  
Badge, Pagination, Footer

Notícia completa Header, Breadcrumb, título, imagem,  
conteúdo e notícias relacionadas

Contato Header, ContactInfo, FormField,  
Button, Footer

## **Área do Cooperado Header, formulário de login,**

## **Button, mensagens de validação,**

## **Footer**

## **9\. Tokens CSS**

```
:root {
  /* Brand colors */
  --color-primary: #006633;
  --color-secondary: #F4C300;
  --color-green-dark: #0B3D2E;
  --color-green-light: #4CAF50;
  --color-natural-white: #F8F8F5;
  --color-graphite: #1A1A1A;

  /* Interface colors */
  --color-surface: #FFFFFF;
  --color-text-muted: #666666;
  --color-border: #E2E5E1;
  --color-success: #237A45;
  --color-error: #B42318;
  --color-warning: #8A5A00;
  --color-info: #245C9C;

  /* Typography */
  --font-heading: "Montserrat", Arial, sans-serif;
  --font-body: "Roboto", Arial, sans-serif;

  --font-size-h1: 48px;
  --font-size-h2: 36px;
  --font-size-h3: 28px;
  --font-size-body: 16px;
  --font-size-small: 14px;

  /* Radius */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
  --radius-pill: 999px;

  /* Spacing */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-5: 24px;
  --space-6: 32px;
  --space-7: 48px;
  --space-8: 64px;
  --space-9: 96px;

  /* Shadows and motion */
  --shadow-sm: 0 2px 6px rgba(0, 0, 0, 0.06);
  --shadow-md: 0 4px 16px rgba(0, 0, 0, 0.10);
  --shadow-lg: 0 8px 24px rgba(0, 0, 0, 0.14);
  --transition-fast: 200ms ease;
}
```

## **10\. Exemplo de implementação Tailwind CSS**

A paleta pode ser adicionada à configuração do Tailwind como tokens de  
tema. Exemplo conceitual:

```
theme: {
  extend: {
    colors: {
      comigo: {
        primary: "#006633",
        secondary: "#F4C300",
        dark: "#0B3D2E",
        light: "#4CAF50",
        natural: "#F8F8F5",
        graphite: "#1A1A1A"
      }
    },
    fontFamily: {
      heading: ["Montserrat", "Arial", "sans-serif"],
      body: ["Roboto", "Arial", "sans-serif"]
    },
    borderRadius: {
      sm: "4px",
      md: "8px",
      lg: "12px",
      xl: "16px"
    }
  }
}
```

## **11\. Regras de consistência e identidade**

1. Não modificar as cores oficiais da identidade visual.  
2. Não redesenhar, recolorir ou distorcer o logotipo.  
3. Usar Montserrat nos títulos e Roboto nos textos.  
4. Reutilizar os componentes definidos em todas as páginas.  
5. Não criar estilos isolados quando houver um componente padrão.  
6. Garantir contraste, foco visível e navegação por teclado.  
7. Conferir a documentação com o manual oficial da marca antes da  
   publicação.

## **12\. Resultado esperado**

Este Design System fornece uma base visual consistente e reutilizável  
para o site institucional da COMIGO. A aplicação dos tokens e  
componentes deve facilitar a manutenção, acelerar o desenvolvimento e  
preservar a identidade visual original da empresa.

