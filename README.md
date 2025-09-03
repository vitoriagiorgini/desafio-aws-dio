# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data**: 07/09/2025
**Empresa**: Abstergo Industries
**Responsável**: Vitória Beatriz C. Giorgini

## Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Vitória Beatriz C. Giorgini.
O objetivo do projeto foi elencar 3 serviços AWS que contribuíssem para a diminuição de custos imediatos, além de otimizar o uso de infraestrutura em nuvem, garantindo maior escalabilidade, segurança e eficiência.

## Descrição do Projeto

O projeto de implementação de ferramentas foi pensado em três etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

### Etapa 1: 
- **Nome da ferramenta:** Amazon EC2 Auto Scalling
- **Foco da ferramenta:** Gerenciamento automático e otimização de servidores virtuais (instâncias EC2) na nuvem.
- **Descrição de caso de uso:** O EC2 Auto Scaling é como um "gerente automático" de servidores. Ele monitora o uso dos seus aplicativos e, quando percebe que a demanda está crescendo, ele automaticamente liga mais instâncias EC2 para dar conta do recado. E o mais legal é que, quando a demanda diminui, ele desliga as instâncias que não são mais necessárias. Isso é super importante para a diminuição de custos imediatos porque a Abstergo Industries passa a pagar apenas pelos servidores que estão sendo usados no momento, sem desperdiçar dinheiro com capacidade ociosa. É um sistema que se ajusta automaticamente, garantindo que a empresa tenha sempre a quantidade certa de recursos, nem mais, nem menos. Isso também ajuda a manter os serviços online e rápidos para os usuários, mesmo em picos de acesso. Este recurso ajuda a "parar de tentar adivinhar a capacidade", garantindo que os recursos estejam sempre alinhados com a necessidade real, o que é um fator crucial para a economia.

### Etapa 2: 
- **Nome da ferramenta:** Amazon ElastiCache 
- **Foco da ferramenta:** Adicionar uma camada de cache de alta performance para reduzir a carga em bancos de dados e acelerar a recuperação de dados.
- **Descrição de caso de uso:** O ElastiCache é como uma "memória super-rápida" para os dados mais acessados, ele funciona como uma espécie de "memória super-rápida" para armazenar temporariamente os dados mais acessados pelas aplicações. Com o ElastiCache, os dados mais populares ficam organizados logo na entrada, facilitando o acesso imediato. Isso significa que, para dados que são lidos com frequência (como informações de perfil de usuário ou catálogos de produtos), sem precisar ir até o banco de dados principal toda hora. Isso reduz a carga no banco de dados, o que pode permitir usar um banco de dados menor e mais barato (redução de custos), e deixa as aplicações muito mais rápidas para os usuários (melhora da qualidade e experiência). O ElastiCache, ao servir dados a partir de um cache em memória, não só acelera a entrega de conteúdo, mas também alivia a pressão sobre o banco de dados principal, permitindo que a Abstergo Industries possa otimizar sua infraestrutura de dados e, consequentemente, seus custos, enquanto oferece uma experiência mais fluida para os usuários.

### Etapa 3: 
- **Nome da ferramenta:** Amazon S3 
- **Foco da ferramenta:** Armazenamento de objetos com otimização automática de custos através de diferentes classes de armazenamento.
- **Descrição de caso de uso:** O Amazon S3 (Simple Storage Service), é o serviço de armazenamento de objetos da AWS. O S3 é super versátil para guardar qualquer tipo de arquivo, desde fotos e vídeos até backups e documentos. O segredo para a redução de custos está nas diferentes "classes de armazenamento" que o S3 oferece. A grande sacada para a Abstergo Industries foi implementar o **S3 Intelligent-Tiering**. Este recurso é vantajoso e benéfico porque ele automaticamente move os seus dados entre as classes de armazenamento mais econômicas, dependendo de como você os usa. Se um arquivo que é muito acessado de repente para de ser acessado, o Intelligent-Tiering move ele para uma classe mais barata, e se você voltar a acessá-lo, ele o move de volta para uma classe de acesso rápido. Isso significa que a Abstergo Industries não precisa se preocupar em decidir onde guardar cada arquivo para economizar, pois o S3 faz isso de forma inteligente e automática, garantindo que os custos com armazenamento sejam sempre os mais otimizados possíveis, sem precisar de intervenção manual constante. A utilização estratégica das classes de armazenamento do S3, especialmente com o Intelligent-Tiering, permite que a Abstergo Industries "beneficie-se de enormes economias de escala" ao ajustar dinamicamente o custo de armazenamento à real necessidade de acesso aos dados.

## Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como esperado a redução de custos, a construção de uma infraestrutura mais inteligente e flexível, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos

Aqui estão alguns links de referência da documentação da AWS e dos materiais de estudo que foram consultados durante este projeto, que ajudam a entender melhor os serviços abordados e suas funcionalidades:

*   **Amazon EC2 Auto Scaling**:
    *   <https://aws.amazon.com/pt/ec2/autoscaling/>
    *   <https://docs.aws.amazon.com/pt_br/autoscaling/ec2/userguide/ec2-auto-scaling-predictive-scaling.html>
    *   <https://docs.aws.amazon.com/pt_br/AWSEC2/latest/UserGuide/concepts.html>
    *   SLIDES DA DIO

*   **Amazon ElastiCache**:
    *   [aws.amazon.com](https://aws.amazon.com/pt/elasticache/)
    *   SLIDES DA DIO

*   **Amazon S3 e Classes de Armazenamento**:
    *   <https://docs.aws.amazon.com/pt_br/AmazonS3/latest/userguide/Welcome.html>
    *   <https://aws.amazon.com/pt/s3/storage-classes/>
    *   <https://docs.aws.amazon.com/pt_br/AmazonS3/latest/userguide/intelligent-tiering-overview.html>
    *   <https://aws.amazon.com/pt/what-is/cloud-storage/>
    *   SLIDES DA DIO

*   **Conceitos Gerais da Nuvem (introducao-a-cloud.pdf)**:
    *  <https://aws.amazon.com/pt/what-is-cloud-computing/>
    *  <https://docs.aws.amazon.com/pt_br/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html>
    *  SLIDES DA DIO

---

**Assinatura do Responsável pelo Projeto**:

Vitória Beatriz C. Giorgini
