<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Untitled Document</title>
<script src="SpryAssets/SpryValidationTextField.js" type="text/javascript"></script>
<link href="SpryAssets/SpryValidationTextField.css" rel="stylesheet" type="text/css">
</head>

<body style="background-color:#CF6; font-family:Tahoma; color:#00C !important;">
<h2 align="center">Trabalhando com formulário &quot;Parte 5-3&quot;
</h2>
<form name="form1" method="post" action="">
  <table width="600" border="0" align="center" cellpadding="10">
    <tr>
      <td width="283" align="right">Nome:</td>
      <td width="285"><label for="nome"></label>
      <input name="nome" type="text" id="nome" size="40"></td>
    </tr>
    <tr>
      <td align="right">CPF:</td>
      <td><label for="cpf"></label>
        <span id="sprytextfield1">
        <input type="text" name="cpf" id="cpf">
      <span class="textfieldRequiredMsg">Campo Obrigatório.</span><span class="textfieldInvalidFormatMsg">Formato Inválido.</span></span></td>
    </tr>
    <tr>
      <td align="right">Endereço:</td>
      <td><label for="endereco"></label>
      <input name="endereco" type="text" id="endereco" size="40"></td>
    </tr>
    <tr>
      <td align="right">CEP:</td>
      <td><label for="cep"></label>
        <span id="sprytextfield2">
        <input type="text" name="cep" id="cep">
      <span class="textfieldRequiredMsg">Cep e Obrigatório.</span><span class="textfieldInvalidFormatMsg">Formato Inválido.</span></span></td>
    </tr>
    <tr>
      <td align="right">Empresa:</td>
      <td><label for="empresa"></label>
      <input name="empresa" type="text" id="empresa" size="20"></td>
    </tr>
    <tr>
      <td align="right">CNPJ:</td>
      <td><label for="cnpj"></label>
        <span id="sprytextfield3">
        <input type="text" name="cnpj" id="cnpj">
      <span class="textfieldRequiredMsg">CNPJ é Obrigatótio.</span><span class="textfieldInvalidFormatMsg">Formato Inválido.</span></span></td>
    </tr>
    <tr>
      <td><input type="submit" name="enviar" id="button" value="Enviar"></td>
      <td>&nbsp;</td>
    </tr>
  </table>
</form>
<p>&nbsp;</p>
<script type="text/javascript">
var sprytextfield1 = new Spry.Widget.ValidationTextField("sprytextfield1", "custom", {pattern:"000.000.000-00", hint:"000.000.000-00", useCharacterMasking:true});
var sprytextfield2 = new Spry.Widget.ValidationTextField("sprytextfield2", "custom", {pattern:"00.000-000", hint:"00.000-000", useCharacterMasking:true});
var sprytextfield3 = new Spry.Widget.ValidationTextField("sprytextfield3", "custom", {pattern:"00.000.000/0000-00", hint:"00.000.000/0000-00", useCharacterMasking:true});
</script>
</body>
</html>
