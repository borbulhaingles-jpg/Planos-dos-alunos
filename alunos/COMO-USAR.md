# Portal dos Alunos · Karol English

## Estrutura de pastas

```
alunos/
├── maria-joao/
│   ├── index.html          ← portal da aluna (edite aqui todo mês)
│   ├── planos/
│   │   ├── junho-2025.html
│   │   └── maio-2025.html
│   ├── aulas/
│   │   ├── aula-10jun2025.pdf
│   │   └── aula-03jun2025.pdf
│   └── materiais/
│       └── vocab-present-perfect.pdf
│
├── joao-silva/             ← próximo aluno (copie a pasta maria-joao)
│   └── index.html
│
└── COMO-USAR.md            ← este arquivo
```

---

## Adicionar um novo aluno

1. Copie a pasta `maria-joao/` inteira
2. Renomeie para o nome do aluno (ex: `joao-silva`)
3. Abra `index.html` e edite o bloco no topo:

```js
const ALUNO = {
  nome:    "João Silva",
  iniciais:"JS",
  nivel:   "A2 · Iniciante",
  dia_hora:"Quintas 18h",
  desde:   "Junho 2025"
};
```

4. Limpe os arrays `PLANOS`, `AULAS_AO_VIVO` e `MATERIAIS` (deixe só os comentários)
5. Envie o link para o aluno: `seusite.github.io/alunos/joao-silva`

---

## Adicionar plano mensal novo

1. Crie o arquivo do plano em `planos/julho-2025.html`
   (copie `junho-2025.html` e edite o conteúdo)
2. No `index.html` do aluno, adicione uma linha no array `PLANOS`:

```js
{ mes: "Julho 2025", data_envio: "01/07/2025", semanas: 4, status: "novo", link: "planos/julho-2025.html" },
```

3. Mude o mês anterior de `"novo"` para `"concluido"`

---

## Adicionar material de aula ao vivo

No `index.html` do aluno, adicione uma linha no array `AULAS_AO_VIVO`:

```js
{ data: "17/06/2025", tema: "Conditionals · If Clauses", tipo: "pdf", link: "aulas/aula-17jun2025.pdf" },
```

Coloque o arquivo PDF na pasta `aulas/`.

---

## Subir no GitHub Pages (passo a passo)

1. Acesse github.com e crie uma conta (gratuito)
2. Clique em **New repository** → nome: `alunos` → marque **Public** → clique **Create**
3. Na página do repositório, clique em **uploading an existing file**
4. Arraste toda a pasta `alunos/` para a área de upload
5. Clique em **Commit changes**
6. Vá em **Settings → Pages → Branch: main → / (root)** → clique **Save**
7. Aguarde 1-2 minutos. O site estará em:
   `https://seuusername.github.io/alunos/maria-joao`

### Atualizar depois (todo mês)

1. Acesse github.com/seuusername/alunos
2. Navegue até o arquivo que quer atualizar
3. Clique no ícone de lápis (editar) ou em **Add file → Upload files**
4. Faça a alteração e clique em **Commit changes**
5. O site atualiza automaticamente em segundos

---

## Status dos planos

| Status     | Aparece como       |
|------------|--------------------|
| `novo`     | Badge roxo "Novo"  |
| `andamento`| Badge verde "Em andamento" |
| `concluido`| Badge verde "Concluído" |

## Tipos de arquivo

| Tipo        | Ícone |
|-------------|-------|
| `pdf`       | 📄    |
| `slides`    | 📊    |
| `exercicio` | 📝    |
| `audio`     | 🎧    |
| `link`      | 🔗    |
