# Ucommerce - Plugin - Banners

## [< voltar para home](/UcommerceDocs)

## Implementar banner no template

Para carregar os banners, será enviado uma array com os parâmetro desejados.

| PARAMETROS |                                                        VALOR |
| ---------- | -----------------------------------------------------------: |
| category   | `banner-home` (tipo de banner), este valor é definido no painel de admin. Em banners e em gerenciar categoria. Para exibir todas as categorias pode ser colocado o parâmetro `all` |
| format     | `slide` este parâmetro não é obrigatório, se nele for colocado `slide` a coleção de banner será transformado em um carrossel |

------

### Exemplo

```php
<?php banners('banners') -> getBanners(array(
    "category" => "banner-home",
    "format" => "slide"
)); ?>
    
    
    /* Exemplo de retorno
    	<div class="ucbanner ucslide">
    		<div class="ucbanner_content">
        		<img src="https://www.enderecodaloja.com.br/wordpress/wp-content/uploads/2019/03/banner_home_03.png">
   			</div>
    		<div class="ucbanner_content">
        		<img src="https://www.enderecodaloja.com.br/wordpress/wp-content/uploads/2019/03/banner_home_02.png">
            </div>
        </div>
    */
```



## [< voltar para home](/UcommerceDocs)