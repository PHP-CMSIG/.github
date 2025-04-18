# PHP CMS-IG

PHP CMS-IG stands for **PHP Content Management System Interop Group** as a reference to the [PHP FIG](https://www.php-fig.org/) (PHP Framework Interop Group).

A happy coincidence [@chirimoya](https://github.com/chirimoya) and [@bmack](https://github.com/bmack) met each other years ago before they did work
on different Content Management Systems and stayed in contact. Also on different Symfony events core developers of Sulu and Contao met each other from time to time.

As core developers of different Content Management Systems we are facing similar issues, and we want to work together to solve them in a common way.

 - [Contao](https://contao.org) ([@toflar](https://github.com/toflar))
 - [Sulu](https://sulu.io) ([@alexander-schranz](https://github.com/alexander-schranz), [@chirimoya](https://github.com/chirimoya))
 - [TYPO3](https://typo3.org) ([@bmack](https://github.com/bmack))

## What do we already share?

The [PHP Language](https://www.php.net/) is not the only part we are already sharing. 

The following packages are already shared between the different Content Management Systems,
using similar third party packages make each single CMS more stable and secure.

 - [Symfony Stack](https://symfony.com) (Contao, Sulu, TYPO3)
 - [Doctrine/DBAL](https://github.com/doctrine/dbal) (Contao, Sulu, TYPO3)
 - [Symfony CMF Routing](https://github.com/symfony-cmf/routing-bundle) (Contao, Sulu)
 - [Imagine](https://github.com/php-imagine/Imagine), [Contao/Imagine-SVG](https://github.com/contao/imagine-svg) (Contao, Sulu)
 - [Toflar/psr6-symfony-http-cache-store](https://github.com/Toflar/psr6-symfony-http-cache-store) (Contao, Sulu)
 - [Flysystem](https://github.com/thephpleague/flysystem), [Flysystem Bundle](https://github.com/thephpleague/flysystem-bundle) (Contao, Sulu)

## What are we working on?

There are some common issues we want to solve, which we are working inside this Github Organisation:

### SEAL - Search Engine Abstraction Layer

<div align="left">
    <img alt="SEAL Logo with an abstract seal sitting on a telescope." src="https://avatars.githubusercontent.com/u/120221538?s=400&v=6" width="50" height="50">
</div>

A website search is a common feature for all Content Management Systems, but we were all not really happy with the existing solutions. With SEAL the Search Engine Abstraction Layer
we want to provide a common way to communicate with different search engines (Elasticsearch, Opensearch, Algolia, Meilisearch, Loupe, Redisearch, Solr, Typesense).

[SEAL Github Repository](https://github.com/PHP-CMSIG/search)

### HTTPList

There are a lot of different tracking parameters and cookies around today. As CMS we want to provide website pages as fast
as possible and ignore tracking parameters so server side http caches has more cache hits. With a collection of known
query and cookie parameters we can provide better caching and canonical URL handling for each CMS.

[HTTPList Github Repository](https://github.com/PHP-CMSIG/Http-List)
