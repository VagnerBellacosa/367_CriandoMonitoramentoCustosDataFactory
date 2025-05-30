# 367_CriandoMonitoramentoCustosDataFactory
 Criando um Monitoramento de Custos no Data Factory



###### DESCRIÇÃO

Neste projeto, é apresentada uma visão prática do ambiente Azure a partir da criação de recursos com uma conta gratuita de estudante. O foco está em configurar o Azure Data Factory e preparar o ambiente para monitorar o uso e os custos dos recursos implantados. São abordados temas como: estruturação de assinaturas, criação de grupos de recursos, boas práticas de nomenclatura, personalização de dashboards, utilização de métricas e alertas de custo. Também é demonstrada a criação de templates de infraestrutura como código (ARM Templates) e a utilização do Azure Cloud Shell para automações via linha de comando. O projeto oferece um passo a passo completo desde a criação do recurso até a visualização dos dados de consumo, promovendo uma compreensão clara sobre o controle de custos e a organização de recursos dentro do Azure.

**Azure Data Factory****Azure****Azure Databricks**

------

###### Full-Stack

###### Intermediário

------

###### ESPECIALISTA

![author](https://hermes.dio.me/users/author/photos/61268924-081c-452f-8eab-e2dae323a9ba.jfif)

###### Carol Lavecchia

Founder & CTO at Invictus Data & AI, Invillia[**](https://www.linkedin.com/in/caroline-lavecchia/?originalSubdomain=br)



https://web.dio.me/lab/criando-um-monitoramento-de-custos-no-data-factory/learning/d2abf29d-8283-469d-829e-f0142be6b7c9



[**](https://web.dio.me/play)

##### Criando um Monitoramento de Custos no Data Factory



<iframe id="ytc44" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Introdução" width="100%" height="100%" src="https://www.youtube.com/embed/1GmNrjzCSgo?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2Fa1819c5f-fa66-421a-aca1-f1cfc5b8e786%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>



<iframe id="ytc56" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Visão Geral da Microsoft Azure" width="100%" height="100%" src="https://www.youtube.com/embed/1LeKwqoyigk?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2Fda244df0-2273-44ac-88ab-cc3c773efcc9%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>



<iframe id="ytc68" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Criar um recurso" width="100%" height="100%" src="https://www.youtube.com/embed/lehvrf8awos?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2F5436c467-63e7-414b-9137-f9a54de19837%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>



<iframe id="ytc80" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Meu Dashboard" width="100%" height="100%" src="https://www.youtube.com/embed/UKDti5aQAwY?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2Fec8369d7-65bb-4385-a6e9-4af3d9ead2f3%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>





<iframe id="ytc92" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Criar um Data Factory parte 1" width="100%" height="100%" src="https://www.youtube.com/embed/sFmUPF2vI6c?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2F6d5c62fd-d46e-4183-bad0-62c4887e1aa3%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>





<iframe id="ytc104" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Criar um Data Factory parte 2" width="100%" height="100%" src="https://www.youtube.com/embed/Vexj5wQUi7s?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2Fac66a4cf-4cee-4665-b38a-1b59392df5b4%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>





<iframe id="ytc116" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Revisando o recurso criado" width="100%" height="100%" src="https://www.youtube.com/embed/Z024-BGUUN0?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2Fd2abf29d-8283-469d-829e-f0142be6b7c9%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>





<iframe id="ytc128" frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Encerramento" width="100%" height="100%" src="https://www.youtube.com/embed/J-9gMh6JkG0?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1&amp;forigin=https%3A%2F%2Fweb.dio.me%2Flab%2Fcriando-um-monitoramento-de-custos-no-data-factory%2Flearning%2F39999708-6e21-4260-a7dc-fb9cd66a675f%3Fback%3D%2Fplay&amp;aoriginsup=1&amp;vf=6" data-gtm-yt-inspected-21="true" data-gtm-yt-inspected-29="true" style="box-sizing: inherit; max-width: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>





Introdução

Visão Geral da Microsoft Azure

Criar um recursoMeu Dashboard

Criar um Data Factory parte 1

Criar um Data Factory parte 2

Revisando o recurso criado

Encerramento

Materiais de Apoio
