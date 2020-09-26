<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

## Backapi

Uma simples API rest em Laravel. Fique á vontade para usar esse repositório como um base para projetos pessoais em Laravel. 

- Docker
- xdebug
- Ferramentas de qualidade de código e cobertura de testes (baseado nos padrões da LeroyMerlyn)

### Instruções:

#### Requisitos:
 
 - docker-compose
 
#### Build:
 
 - clone este repositório
 - Construa os serviços com ``` docker-compose up -d ```
 - Ele irá criar dois serviços, web e db, olhe o Dockerfile para detalhes de imagens, versões, portas, a pasta environment tem arquivos de configuração adicional
 - Execute o composer install dentro do container web: ``` docker-compose exec web composer install ```
 - O GrumpPHP está configurado para analisar o código antes dos commits.
 - Para rodar manualmente o PHPUnit, phpstan e demais ferramentas, use o container web:
 - ex: ``` docker-compose exec web vendor/bin/phpunit ```
 ``` docker-compose exec web vendor/bin/phpcs --memory-limit=1G ```
 
## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
