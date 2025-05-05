function calculadoraRankeada (vitorias, derrotas){

const saldoVitorias = vitorias - derrotas;
let nivel = " ";

if (vitorias < 10){
    nivel = "Ferro"
}else if(vitorias <= 20){
    nivel = "Bronze"
}else if(vitorias <= 50){
    nivel = "Prata"
}else if (vitorias <= 80){
    nivel = "Ouro"
}else if (vitorias <= 90){
    nivel = "Diamante"
}else if (vitorias <= 100){
    nivel = "Léndario"
}else{
    nivel = "Mortal"
}
return "O Heroi tem saldo de " + saldoVitorias + "está no nível de  " + nivel;

}

const vitorias = 75;
const derrota = 20;
const resultado = calculadoraRankeada(vitorias, derrota);

console.log("resultado")
