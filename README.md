<!DOCTYPE html>
<html>
<head>
    <title>Link PIX</title>
</head>
<body>
    <a id="pixLink" href="#" onclick="copyToClipboard()">Clique aqui para copiar o PIX</a>

    <script>
        function copyToClipboard() {
            // Código PIX que você deseja copiar
            const pixCode = "00020126650014br.gov.bcb.pix013656605b1b-aa4d-4165-9bb6-c03b1269b8e50203Pix5204000053039865802BR5925RICARDO ALEX FALACIO NASC6008BLUMENAU62110507Ricardo63042B81";

            // Cria um elemento temporário para copiar o código PIX
            const tempInput = document.createElement("input");
            tempInput.setAttribute("value", pixCode);

            // Anexa o elemento ao corpo do documento
            document.body.appendChild(tempInput);

            // Selecione o conteúdo do elemento
            tempInput.select();

            // Copia o conteúdo selecionado
            document.execCommand("copy");

            // Remove o elemento temporário
            document.body.removeChild(tempInput);

            // Pode adicionar uma mensagem de sucesso ou fazer redirecionamento aqui, se desejado
            alert("O código PIX foi copiado para a área de transferência!");
        }
    </script>
</body>
</html>
