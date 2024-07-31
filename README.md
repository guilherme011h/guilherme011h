// Script para vr.code.dev

// Definição de uma classe para representar Filmes
class Filme {
    constructor(titulo, diretor, ano, genero, avaliacao) {
        this.titulo = titulo;
        this.diretor = diretor;
        this.ano = ano;
        this.genero = genero;
        this.avaliacao = avaliacao;
    }

    // Método para obter uma representação textual do filme
    getInfo() {
        return `${this.titulo} (${this.ano}) - Dirigido por ${this.diretor}. Gênero: ${this.genero}. Avaliação: ${this.avaliacao}/5`;
    }
}

// Definição de uma classe para representar Séries
class Serie {
    constructor(titulo, criador, ano, genero, numTemporadas) {
        this.titulo = titulo;
        this.criador = criador;
        this.ano = ano;
        this.genero = genero;
        this.numTemporadas = numTemporadas;
    }

    // Método para obter uma representação textual da série
    getInfo() {
        return `${this.titulo} (${this.ano}) - Criado por ${this.criador}. Gênero: ${this.genero}. ${this.numTemporadas} temporadas disponíveis.`;
    }
}

// Exemplos de filmes e séries
let filmes = [
    new Filme("Interestelar", "Christopher Nolan", 2014, "Ficção Científica", 4.5),
    new Filme("O Poderoso Chefão", "Francis Ford Coppola", 1972, "Crime", 5),
    new Filme("Pantera Negra", "Ryan Coogler", 2018, "Ação", 4)
];

let series = [
    new Serie("Stranger Things", "Irmãos Duffer", 2016, "Ficção Científica", 3),
    new Serie("Breaking Bad", "Vince Gilligan", 2008, "Drama", 5),
    new Serie("Game of Thrones", "David Benioff, D.B. Weiss", 2011, "Fantasia", 8)
];

// Função para listar todos os filmes
function listarFilmes() {
    console.log("===== Filmes Disponíveis =====");
    filmes.forEach(filme => {
        console.log(filme.getInfo());
    });
    console.log("===============================");
}

// Função para listar todas as séries
function listarSeries() {
    console.log("===== Séries Disponíveis =====");
    series.forEach(serie => {
        console.log(serie.getInfo());
    });
    console.log("===============================");
}

// Chamada das funções para listar filmes e séries
listarFilmes();
listarSeries();
