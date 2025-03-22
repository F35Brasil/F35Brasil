<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Cadastro de Cliente</title>
</head>
<body>
    <main></main>
    <h1>Cadastro de Cliente</h1>
    <form action="cadastraCliente.php" method="post"></form>
    <fieldset>
        <legend>
            Dados Pessoais
        </legend>
        <div> 
            <label for="nome">Nome (obrigatório):</label>
        <input type="text" id="nome" name="nome" required minlength="2" maxlength="50">
        </div>
        <div>
            <label for="email">E-mail (obrigatório):</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div>
            <label for="cpf">CPF (obrigatório):</label>
            <input type="text" id="cpf" name="cpf" required pattern="\d{3}\.\d{3}\.\d{3}-\d{2}">
        </div>       
        <div>
            <label for="idade">Idade (obrigatório):</label>
            <input type="number" id="idade" name="idade" required>
        </div>
        <div>
            <label for="telefone">Telefone (obrigatório):</label>
            <input type="tel" id="telefone" name="telefone" required>
        </div>
       <div>
        <label for="data_nascimento">Data de Nascimento (opcional):</label>
        <input type="date" id="data_nascimento" name="data_nascimento">
       </div>
    <div>
    Sexo (opcional):
            <input type="radio" id="sexo_masculino" name="sexo" value="masculino">
            <label for="sexo_masculino">Masculino</label>
            <input type="radio" id="sexo_feminino" name="sexo" value="feminino">
            <label for="sexo_feminino">Feminino</label>
            <input type="radio" id="sexo_outro" name="sexo" value="sexo_outro">
            <label for="sexo_outro">Outro</label>
</div>
<div>
    Estado Civil (opcional):
        <input type="radio" id="casado" name="Estado Civil" value="casado">
        <label for="casado">Casado</label>
        <input type="radio" id="solteiro" name="Estado Civil" value="solteiro">
        <label for="solteiro">Solteiro</label>
</div>
</fieldset>
<fieldset>
    <legend>Endereço de Entrega</legend>
<div>
    <label for="idcep">Cep (obrigatorio):</label>
    <input type="number" id="idcep" name="Cep">
</div>
<div>
    <label for="tipo_logradouro">Tipo de Logradouro (obrigatório):</label>
            <select id="tipo_logradouro" name="tipo_logradouro">
                <option value="">Selecione</option>
                <option value="rua">Rua</option>
                <option value="avenida">Avenida</option>
                <option value="praca">Praça</option>
            </select>         
</div>
<div>
    <label for="logradouro">Logradouro (obrigatório):</label>
    <input type="text" id="logradouro" name="logradouro">
</div>
<div> 
    <label for="bairro">Bairro (obrigatório):</label>
    <input type="text" id="bairro" name="bairro">
</div>
<div>
    <label for="cidade">Cidade (obrigatório):</label>
    <input type="text" id="cidade" name="cidade">
</div>
    <div>
    <label for="estado">Estado (obrigatório):</label>
    <input type="text" id="estado" name="estado">
</div>
</fieldset>
 <fieldset>
     <legend>
        Informações Adicionais
     </legend>
<div>
    <input type="checkbox" id="interesse_filmes" name="interesses[]" value="filmes">
    <label for="interesse_filmes">Filmes</label>
</div>
<div>
    <input type="checkbox" id="interesse_informatica" name="interesses[]" value="informatica">
    <label for="interesse_informatica">Informática</label> 
</div>
<div>
    <input type="checkbox" id="interesse_games" name="interesses[]" value="games">
    <label for="interesse_games">Games</label>
</div>
<div>
    <input type="checkbox" id="interesse_livros" name="interesses[]" value="livros">
     <label for="interesse_livros">Livros</label>
</div>
<div>
    <input type="checkbox" id="interesse_roupas" name="interesses[]" value="roupas">
    <label for="interesse_roupas">Roupas</label><br><br>
</div>
<div>
    <label for="informacoes_complementares">Informações Complementares (opcional):</label>
    <textarea id="informacoes_complementares" name="informacoes_complementares" rows="4" cols="50"></textarea>
</div>
<div>
    <label for="arquivo">Anexar Arquivo (opcional):</label>
    <input type="file" id="arquivo" name="arquivo">
</div>
     </fieldset>
    <input type="submit" value="Cadastrar">
    <footer>Cadastro Padrão</footer>
</body>
</html>




     
    


