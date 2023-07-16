/**
 * Make all link to another domain to open in a named window or tab
 * @param {String} host The base domain.
 * @param {String} target The window or tab name.
 * @returns {Number} Total of links affected
 */
function link2Target(host, target) {
    target = [target === undefined? "_blank": target].join("");
    host = [host === undefined? window.location.host: host].join("");

    var regexp = new RegExp("^(https?:\/\/)?" + host.split(".").join("\\.") , "i");
    var links = document.getElementsByTagName("a");
    var link = links.item(0);
    var count = 0;

    for (var i = 0; link !== null; link = links.item(++i)) {
        if (!regexp.test(link.href)){
            link.setAttribute("target", target);
            ++count;
        }
    }

    return count;
}

![](logo2.png)

<sub>Meu portfólio de projetos em análise de dados.</sub>

Sou um analista de dados com mais de 10 anos de experiência em liderança e gestão em diversas áreas de negócio. Com formação em Gestão Financeira pela ULBRA e Analista de Dados pela Data Science Academy (com habilidades em SQL, Python, Power BI e DAX), e MBA em Tecnologia para Negócios: AI, Data Science e Big Data pela PUC/RS.

**Habilidades em:** Python, SQL, Power BI e gestão de negócios.

**Links:**
* [LinkedIn](https://www.linkedin.com/in/rodrigo-xavier-dos-santos-75174110a/)
* [Medium](https://medium.com/@rodrigo.analise.dados)



## Projetos:
Análise de dados com SQL:

* **Análise exploratória de dados reais do Covid-19 com SQL:** https://bit.ly/3cvnzQN

Análise de dados com Python:

* **Limpeza, tratamento e preparação dos dados de acidentes de trânsito no Brasil em 2022:** http://bit.ly/3iATaTG

##

Análise de dados no Power BI:
* [Dashboard de vendas](https://app.powerbi.com/view?r=eyJrIjoiOTVjNjc1YTAtNWRkOS00ZTVkLWI5NzktM2VhODFlOGRhZGJkIiwidCI6ImUxMzc4OGViLTFkM2ItNDhkMi1iMTlmLTdmZTIyNjJhNjAyMyJ9)
* <a href="https://app.powerbi.com/view?r=eyJrIjoiMjlhOGZjMTktYTQ0MC00MDc2LTljZDAtMzQ0NjY3NjlkYWQ2IiwidCI6ImUxMzc4OGViLTFkM2ItNDhkMi1iMTlmLTdmZTIyNjJhNjAyMyJ9" target="_blank">Dashboard do financeiro</a>
##

