![GitHub last commit (branch)](https://img.shields.io/github/last-commit/shizhao/ITN-corpus/main)
![json](https://img.shields.io/badge/json-validated-brightgreen)
![cc-by-sa 3.0](https://img.shields.io/badge/license-cc--by--sa%203.0-green)

ITN corpus is a multilingual comparable corpus that collects blurb content of  [ITN](https://en.wikipedia.org/wiki/Template:In_the_news) (In the news) on Wikipedia. Daily update.

The corpus is in json format:

```ruby
{
    'Q106823124': {
        '1664055941.0': {
            'lang': 'ru',
            'keyword': 'СоюзМС-22',
            'blurb': 'С«<ahref="https://ru.wikipedia.org/wiki/%D0%91%D0%B0%D0%B9%D0%BA%D0%BE%D0%BD%D1%83%D1%80"title="Байконур">Байконура</a>»стартовалкосмическийкорабль<b>«<ahref="https://ru.wikipedia.org/wiki/%D0%A1%D0%BE%D1%8E%D0%B7_%D0%9C%D0%A1-22"title="Союз МС-22">СоюзМС-22</a>»</b>стремячленами<ahref="https://ru.wikipedia.org/wiki/%D0%9C%D0%9A%D0%A1-68"title="МКС-68">68-йдолговременнойэкспедицииМКС</a>.'
        },
        '1664158103.0': {
            'lang': 'zh',
            'keyword': '联盟MS-22',
            'blurb': '搭載俄羅斯與美國太空人的<b><ahref="https://zh.wikipedia.org/wiki/%E8%81%94%E7%9B%9FMS-22"title="联盟MS-22">聯盟MS-22</a></b><small>（图）</small>自哈萨克斯坦<aclass="mw-redirect"href="https://zh.wikipedia.org/wiki/%E6%8B%9C%E7%A7%91%E5%8A%AA%E7%88%BE%E5%A4%AA%E7%A9%BA%E7%99%BC%E5%B0%84%E5%A0%B4"title="拜科努爾太空發射場">拜科努尔航天发射场</a>發射升空，並與<aclass="mw-redirect"href="https://zh.wikipedia.org/wiki/%E5%9C%8B%E9%9A%9B%E5%A4%AA%E7%A9%BA%E7%AB%99"title="國際太空站">國際太空站</a>完成對接。'
        }

```
Json keys description:

- **`Q106823124`:** [QID](https://www.wikidata.org/wiki/Help:Items) of a Wikidata item, represent the same topics in this set of corpora
- **`1664055941.0`:** Unix timestamp, get the time of the sentence
- **`lang`:** The language code of this sentence (see https://meta.wikimedia.org/wiki/Table_of_Wikimedia_projects)
- **`keyword`:** The subject of this sentence, described in that language
- **`blurb`:** A sentence about the news brief description (see https://en.wikipedia.org/wiki/Blurb), with HTML tags

An example using this corpus： [ITN Syndication](https://itnsyn.toolforge.org/)

## Statistics
![subjects](https://img.shields.io/badge/subjects-%3E200-blue)
![sentences](https://img.shields.io/badge/sentences-%3E2000-blue)
![languages](https://img.shields.io/badge/languages-52-blue)

For more details on the statistics about this corpus, see: [stat.txt](./stat.txt)

## License
<p xmlns:cc="http://creativecommons.org/ns#" >
<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/sa.svg?ref=chooser-v1">
 
This work is licensed under <a href="http://creativecommons.org/licenses/by-sa/3.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-SA 3.0</a></p>
