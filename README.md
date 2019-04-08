## Hg-loading - Plugin JQuery para loadings de pagina.

## Seja bem vindo !

Esse plug-in tem como finalidade exibir uma imagem de carregando *"loading"*.

O acionamento do carregando, é uma chamada simples de javascript, e pode ser  acionado e ocultado facilmente.  

Uma das vantagens de usar esse plugin é que o desenvolvedor nao necessita se preocupar com a codificação HTML, pois as tags são inseridas dinamicamente aos elementos da pagina.

## Como usar

O requisito básico para uso do plugin, é o Jquery. chame-o **antes** de chamar js do plugin. pode ser inserido tanto no final da tag body, quanto no head do HTML.

O download do plugin pode ser feito por aqui no git, e a chamada do JQuery pode ser feita por CDN, conforme o código demo.

Para mostrar o loading:

    $.showLoading();

Para ocultar o loading:

      $.hideLoading();

Adicionalmente, você pode personalizar alguns itens do plugin, trocando a imagem do centro, ou colocando classes css que podem conter animações e muito mais.

## Parametros possíveis

    $.showLoading( 
    { 
	    body:  "", 
	    // the dialog body html 
	    loadingClass:  "", 
	    // Additional css for ".Loading" ".fade",
	    loadingDialogClass:  "", 
	    // Additional css for ".Loading-dialog", like "Loading-lg" or "Loading-sm" for sizing 
	    options:  null, 
	    target:  "", 
	    imgLoading:  "assets/img/loading.svg", 
	    // Events: 
	    onCreate:  null, // Callback, called after the Loading was created 
	    onDispose:  null, // Callback, called after the Loading was disposed 
	    onSubmit:  null  // Callback of $.showConfirm(), called after yes or no was pressed 
	} );
