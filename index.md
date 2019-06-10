# Ucommerce - Plugins - Banner Régua

[TOC]



## Inserir o banner régua

### Para verificar se o banner régua esta ativo
```php
<?php
	banners("bannerRuler") -> getAtv("desktop"); // Para banners no desktop
	// Retorna true ou false
	banners("bannerRuler") -> getAtv("mobile");	// Para banners no mobile
	// Retorna true ou false
?>
```
Causo o banner régua não esteja ativo, ele não retornara nenhum item.

Por default o Banner régua vem configurado como ```true```, se as configurações do painel do administrador não forem alteradas.

Após a alteração serão exibidos as configurações definidas no painel. 

------

### Para pegar todos os itens

```php
<?php
	banners("bannerRuler") -> getItens("all", "Desktop");
	/* Retorna
	** Array ( [0] => banner_ruler_item Object ( [image] => *link_da_imagem* [title] => Titulo [subtitle] => Subtitulo [status] => *true ou false* ) ) 
	*/
?>
```
| Parametros |      Valores      |
| :--------: | :---------------: |
|   itens    |        all        |
|   device   | Desktop ou Mobile |

Ira retornar todos os itens do banner régua se tiverem com o status ativos(```true```).

------

### Para pegar um item especifico do banner régua

```php
<?php
	  banners("bannerRuler") -> getItens("1...4", "Desktop");  // É aceito de 1 a 4 , em device defina se é Desktop ou  Mobile
	  
	/* Retorna
	** Array ( [0] => banner_ruler_item Object ( [image] => *link_da_imagem* [title] => Titulo [subtitle] => Subtitulo [status] => *true ou false* ) ) 
	*/
?>
```
| Parametros |      Valores      |
| :--------: | :---------------: |
|   Itens    |     1 . . . 4     |
|   Device   | Desktop ou Mobile |

Causo algum dos itens esteja marcado para não exibir, não será retornado nenhum parâmetro, apenas os itens ativos serão exibidos.

Por default eles são configurados como ``` true```, se as configurações do painel do administrador não forem alteradas.

Após a alteração serão exibidos as configurações definidas no painel.
