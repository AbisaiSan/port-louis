## Tecnologias utilizadas

1 - Vue -> <script src="https://cdn.jsdelivr.net/npm/vue@2"></script>
2 - TailwindCss -> <link href="https://unpkg.com/tailwindcss@^2/dist/tailwind.min.css" rel="stylesheet">
3 - Vuelidate -> <script src="vuelidate/dist/vuelidate.min.js"></script>
4 - Vuex -> <script src="https://cdn.jsdelivr.net/npm/es6-promise@4/dist/es6-promise.auto.js"></script>
5 - V-mask -> <script src="https://cdn.jsdelivr.net/npm/v-mask/dist/v-mask.min.js"></script>

## Doc Lista de Contatos - Tecnologias utilizadas

### Css
Utilizei como framework css o tailwind que atende os criterios do material design
Optei por ele pela facilidade seja no uso de suas classes, ou na facilidade de criar novas ou alterar as existentes caso seja necessário no projeto. Fora a otima documentação e comunidade do TailwindCss.

### Form
Para as validações dos campos utilizei o Vuelidate por ser uma lib disponibilizada pelo proprio vue além de facilidade quanto ao uso, e documentação. Além de que as validações são completamente dissociadas do modelo, podendo no projeto definir as regras para o modelo do projeto.
Quanto a mascara achei por bem não utilizar regex apesar que seria o uso de uma lib a menos, mas optei pelo o uso do v-mask uma lib para o vue que torna o processo mais simples, e bem util e de facil modificação se necessário.

### VueJS 2.x

Na construção utilizei apenas o vue2 como o projeto ficou completamente em único arquivo html achei por bem não utilizar vuex para o gerenciamento de estado, nem mesmo fiz o uso de props ou eventBus.
Dado a simplicidade de usar apenas um unico arquivo achei melhor assim, apenas com metodos e as diretivas é possivel fazer muita coisa.
Também não fiz uso da criação de componentes pois o a estrutura html é simples. Todavia caso eu tivesse optado por dividir em componentes usaria a estrutura do atomic design em projetos vue-cli, e neste utilizaria assim:

{
    ButtonAdd -> Botão em azul para a criação de um novo contato
    Modal,
    Form -> Apenas os inputs do formulario e Botão para salvar ou editar (Podendo criar um componente apenas para esse botão)
    DataTable,
    ListContact -> Contendo as td's do DataTable,
    ButtonEdit,
    ButtonDelete,
}

link da aplicação: https://listacontatos.netlify.app/