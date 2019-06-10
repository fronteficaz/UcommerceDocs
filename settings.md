# Ucommerce - Plugin - Settings

## [< voltar para home](/UcommerceDocs)

## Pegar os itens de configurações

| TIPO DE PARAMETROS                                           |                                VALORES |
| :----------------------------------------------------------- | -------------------------------------: |
| Todas as configurações                                       |                 ` getSettings("all") ` |
| Todos os valores de uma configuração específica              | ` getSettings("rede_sociais", "all") ` |
| Valor de uma configuração específica e de uma posição específica |     ` getSettings("rede_sociais", 3) ` |

```php
getSettings("typo_de_configuração", "posição_do_campo");
```

```php
/* =========== Pegar todas as configurações =========== */
<?php echo getSettings("all"); ?>
    /*	==== Exempplo de retorno
    	array(11) {
          ["telefone"]=>
          array(1) {
            ["input0"]=>
            string(15) "(**) *****-****"
          }
          ["whatsapp"]=>
          array(1) {
            ["input0"]=>
            string(15) "(**) *****-****"
          }
          ["endereco"]=>
          array(1) {
            ["input0"]=>
            string(6) "..."
          }
          ["descricao_da_empresa"]=>
          array(1) {
            ["input0"]=>
            string(6) "..."
          }
          ["rede_sociais"]=>
          array(5) {
            ["input0"]=>
            string(8) "..."
            ["input1"]=>
            string(7) "..."
            ["input2"]=>
            string(7) "..."
            ["input3"]=>
            string(7) "..."
            ["input4"]=>
            string(7) "..."
          }
          ["formas_de_envio"]=>
          array(1) {
            ["input0"]=>
            string(3) "..."
          }
          ["formas_de_pagamento"]=>
          array(1) {
            ["input0"]=>
            string(7) "..."
          }
          ["horario_de_atendimento"]=>
          array(1) {
            ["input0"]=>
            string(7) "..."
          }
          ["e_mail"]=>
          array(1) {
            ["input0"]=>
            string(30) "..."
          }
          ["rasao_social"]=>
          array(1) {
            ["input0"]=>
            string(6) "..."
          }
          ["cnpj"]=>
          array(1) {
            ["input0"]=>
            string(18) "..."
          }
        }
    */
```

```php
/* =========== Pegar todas as configurações de um tipo específico =========== */
    
    <?php echo getSettings("rede_sociais", "all"); ?>
    
    /* ==== Exempplo de retorno
    
        array(5) {
          ["input0"]=>
          string(8) "..."
          ["input1"]=>
          string(7) "..."
          ["input2"]=>
          string(7) "..."
          ["input3"]=>
          string(7) "..."
          ["input4"]=>
          string(7) "..."
        }
    
    */
```

```php
  /* =========== Pegar valor de um configuração específica =========== */
    
    <?php echo getSettings("rede_sociais", 3); ?>
    
    /* ==== Exempplo de retorno
    	string(7) "..."
	*/
```

## [< voltar para home](/UcommerceDocs)