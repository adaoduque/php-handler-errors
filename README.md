# PHP Handler Error
Testado no PHP 5.6, 7.0, 7.1 e 7.2, com apache 2.4


### Pra que serve ?
Coleta erros no script php de tua aplicação, e trata num outro script PHP, na mesma sessão de execução.
Com isso é possível coletar dados de sessão e variaveis post, para eventualmente simular um erro com os dados reais daquela sessão.

### Como utilizar ?
Apenas escolha um diretório para salvar o arquivo **auto_prepend.php**, agora no teu `php.ini`, inclua o path para o arquivo na diretiva **auto_prepend_file**.

```
auto_prepend_file=/path/to/auto_prepend.php
```

Para fins de testes, coloquei os erros para serem gravados num arquivo `.csv`.

OBS: Lembre-se que existe uma ordem de execução dos erros, por exemplo, erros de compilação ocorrem antes de qualquer outro.
Lembre-te meio óbvio, mas caso alguém esqueça né...

<br />
<br />
Duvidas, criticas ou sugestões:<br>
E-mail: adaoduquesn@gmail.com<br>
Telegram: @adaoDuque <br>
