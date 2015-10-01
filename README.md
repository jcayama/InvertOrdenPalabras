# InvertOrdenPalabras
# Funcion que Invierte el orden de las palabras en una cadena
<HTML>
<HEAD>
<SCRIPT>
function revWords(str){
   words = str.split(" ");
   j = words.length - 1;
   backWords = new Array(); 
   for (i=0 ; i < words.length ; i++){
      backWords[j] = words[i];
      j--
   }         
   document.theForm.results.value = backWords.join(" ");
}
</SCRIPT>
</HEAD>
<BODY>
<FORM name="theForm">
Introduzca una frase:
<TEXTAREA name=inStr rows=5 cols=90>
</TEXTAREA>
<INPUT type=button value="Frase Invertida" onClick="revWords(document.theForm.inStr.value)";>
<INPUT type=button name="theButton" value="Limpiar Resultado" onClick='document.theForm.results.value=""';>
Resultado<br>
<TEXTAREA name=results rows=5 cols=90>
</TEXTAREA>

</FORM>  
</BODY>
</HTML>
