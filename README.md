# Problemas

<details><summary>1 - Ausência de controle das informações da entidade</summary>
    <p>
        <table>
            <tbody>
                <tr>
                    <th style="width: 25%;">
                        Problema
                    </th>
                    <td>
                        Desafio Descomplica
                    </td>
                </tr>
                <tr>
                    <th style="width: 25%;">
                        Afeta
                    </th>
                    <td>
                        Entidade/Diretoria/Funcionários/Clientes
                    </td>
                </tr>
                <tr>
                    <th style="width: 25%;">
                        Desfio
                    </th>
                    <td>
                        Construir uma stack de infraestrutura que provisione um ambiente para rodar uma aplicação backend rest hipotética, com duas                                 réplicas respondendo em um Load Balancer, uma aplicação frontend estática também com duas réplicas, ambas as aplicações respondendo                         pelo mesmo DNS, porém com contextos distintos, utilizando umAPI gateway para direcionamento das requisições
                    </td>
                </tr>
                <tr>
                    <th style="width: 25%;">
                        Solução
                    </th>
                    <td>
                       Construida a Stack como proposto usando as tecnologias Docker, Terraform e GitHub.
                       Note que foi dividido em duas branchs uma para a parte de infraestrutura e a outra para a parte da aplicaç
                       Veja que temos uma pasta com os módulos, e para cada módulo também temos uma pasta com o nome e os arquivos .tf dentro.
                       O módulo de network contém toda a configuração de rede (vpc, subnet, internet gateway, nat gateway, rotas, etc).
                       O módulo master contém a configuração do control plane do EKS.
                       O módulo node contém as configurações dos workers.
                       Por último temos os arquivos na raíz do projeto que farão o uso e a junção de todos os módulos
                    </td>
                </tr>
            </tbody>
        </table>
    </p>
</details>
