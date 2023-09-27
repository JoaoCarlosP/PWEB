function computerChoose() {
    const options = ["pedra", "papel", "tesoura"];
    const index = Math.floor(Math.random() * 3);
    return options[index];
}

function checkWinner(userChoose, computerChoose) {
    if (userChoose === computerChoose) {
        return "Empate!";
    } else if (
        (userChoose === "pedra" && computerChoose === "tesoura") ||
        (userChoose === "tesoura" && computerChoose === "papel") ||
        (userChoose === "papel" && computerChoose === "pedra")
    ) {
        return "Você venceu!";
    } else {
        return "O computador venceu!";
    }
}

function game() {
    alert("Bem-vindo ao jogo Pedra, Papel ou Tesoura!");
    const userChoose = prompt("Escolha pedra, papel ou tesoura:").toLowerCase();

    if (["pedra", "papel", "tesoura"].indexOf(userChoose) === -1) {
        alert("Escolha inválida. Por favor, escolha pedra, papel ou tesoura.");
        return;
    }

    const resultComputerChoose = computerChoose();
    const computChoose = resultComputerChoose;

    alert(`Você escolheu: ${userChoose}`);
    alert(`O computador escolheu: ${computChoose}`);

    const result = checkWinner(userChoose, resultComputerChoose);
    alert(result);
}

game();