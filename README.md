# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário FEI, como parte dos requisitos necessários para aprovação na disciplina de **Interface Humano-Computador (CC8122)** do curso de Ciência da Computação, orientado pelo Prof. Dr. Plinio Thomaz Aquino Junior.

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) intitulado**“Desenvolvimento de Sistema de Apoio ao Diagnóstico de Pneumonia em Radiografias de Tórax utilizando Inteligência Artificial Explicável”**,sob orientação do Prof. Dr. Flavio Tonidandel e desenvolvido por:

- **Enzo Pacheco Porfirio** – 22.225.011-0
- **Gabriel Destro** – 24.122.059-9

---

## 📖 Resumo

A aplicação proposta é uma **plataforma web** que tem como objetivo **apoiar médicos no diagnóstico de pneumonia** a partir de radiografias de tórax.
O foco central é a **interface**, garantindo que os resultados apresentados pela inteligência artificial sejam **compreensíveis, confiáveis e integrados ao fluxo clínico do usuário**.

O sistema busca responder a questões como:

- Como apresentar resultados de forma **clara** e **rápida** no ambiente clínico?
- Como transmitir **confiança** ao profissional de saúde, evitando a sensação de “caixa-preta”?
- Como tornar a ferramenta **intuitiva e não invasiva**, respeitando a rotina clínica?

---

## 🎯 Introdução

O propósito do projeto é **projetar uma interface acessível** para sistemas de apoio ao diagnóstico por imagem.
Enquanto muitos softwares existentes oferecem apenas um valor numérico ou classificação, a nossa proposta busca apresentar informações de forma **visual, explicativa e alinhada às expectativas dos médicos**.

Principais benefícios oferecidos:

- **Suporte ao diagnóstico** sem substituir a decisão clínica.
- **Clareza e interpretabilidade** das decisões da IA.

---

## 🩺 Contexto de uso

- **Usuários**: médicos e profissionais de diagnóstico por imagem.
- **Tarefas**: carregar uma radiografia, visualizar o resultado e interpretar a imagem fornecida pelo sistema.
- **Equipamentos**: notebooks, desktops e tablets conectado à internet.
- **Ambiente**: consultórios, hospitais e clínica.
- **Fator social**: tempo limitado, decisões críticas e pressão por resultados.

---

## 🎯 Público-Alvo

O público principal são **médicos e profissionais da saúde** que lidam com diagnóstico por imagem.Características:

- **Demográficas**: profissionais da área médica, com faixa etária entre 25 e 75 anos.
- **Comportamentais**: necessitam de rapidez, clareza e confiabilidade nos resultados.
- **Psicográficas**: valorizam ferramentas que não interrompam ou atrapalhem o fluxo clínico.
- **Geográficas**: hospitais, clínicas e consultórios, desde áreas rurais até grandes centros urbanos.

---

## 🔍 Análise de Concorrência

Realizou-se uma análise de sistemas e ferramentas existentes voltados à visualização de imagens médicas e diagnóstico de pneumonia por radiografia de tórax.

### **Sistemas Analisados:**

#### **1. CheXNet (Stanford)**

**Descrição**: Sistema de deep learning desenvolvido pela Universidade de Stanford em 2017 para detecção de pneumonia em radiografias de tórax.

**Criadores**: Equipe de pesquisa liderada por Pranav Rajpurkar, Jeremy Irvin e outros pesquisadores da Stanford University.

**Funcionamento**: Utiliza uma rede neural convolucional (CNN) treinada com mais de 100.000 radiografias do NIH Chest X-ray Dataset. O sistema analisa imagens e retorna probabilidades de diferentes condições pulmonares, incluindo pneumonia.

- **Pontos Fortes**: Alta precisão diagnóstica, validação em grandes datasets
- **Pontos Fracos**: Interface limitada, resultados apresentados apenas como probabilidades numéricas
- **Diferencial**: Foco exclusivo em precisão, sem preocupação com usabilidade clínica

#### **2. Google Health AI**

**Descrição**: Plataforma de inteligência artificial médica desenvolvida pelo Google, parte do Google Cloud Healthcare API.

**Criadores**: Google Health, divisão de saúde do Google focada em tecnologias médicas.

**Funcionamento**: Oferece APIs e ferramentas para análise de imagens médicas, incluindo detecção de anomalias em radiografias. Integra-se com sistemas hospitalares existentes e oferece dashboards para visualização de resultados.

- **Pontos Fortes**: Integração com sistemas hospitalares, interface moderna
- **Pontos Fracos**: Complexidade excessiva, curva de aprendizado íngreme
- **Diferencial**: Solução completa para hospitais, mas pode ser excessiva para clínicas menores

#### **3. PACS (Picture Archiving and Communication System)**

**Descrição**: Sistema padrão da indústria médica para armazenamento, transmissão e visualização de imagens médicas digitais.

**Criadores**: Desenvolvido por múltiplas empresas (GE, Siemens, Philips, etc.) seguindo padrões DICOM estabelecidos pela indústria.

**Funcionamento**: Sistema de arquivamento e comunicação de imagens que permite aos médicos visualizar, armazenar e compartilhar exames radiológicos. Funciona como um banco de dados centralizado para imagens médicas com ferramentas de visualização integradas.

- **Pontos Fortes**: Padrão da indústria, integração completa com workflow clínico
- **Pontos Fracos**: Interfaces antiquadas, falta de recursos de IA explicável
- **Diferencial**: Infraestrutura robusta, mas sem foco em interpretabilidade

#### **4. Sistemas de Radiologia Comerciais (GE, Siemens, Philips)**

**Descrição**: Soluções proprietárias desenvolvidas por grandes empresas de equipamentos médicos para análise de imagens radiológicas.

**Criadores**: General Electric (GE), Siemens Healthineers, Philips Healthcare - empresas líderes em equipamentos médicos.

**Funcionamento**: Sistemas integrados que combinam hardware de aquisição de imagens (tomógrafos, ressonâncias) com software de análise. Utilizam algoritmos proprietários de IA para detecção de anomalias e oferecem ferramentas de pós-processamento de imagens.

- **Pontos Fortes**: Hardware otimizado, integração nativa com equipamentos
- **Pontos Fracos**: Alto custo, dependência de equipamentos específicos
- **Diferencial**: Soluções proprietárias, limitadas a equipamentos da marca

### **Lacunas Identificadas:**

1. **Falta de Explicabilidade**: A maioria dos sistemas oferece apenas resultados numéricos sem explicação visual
2. **Interfaces Complexas**: Sistemas existentes priorizam funcionalidade sobre usabilidade
3. **Integração Limitada**: Dificuldade de integração com diferentes workflows clínicos
4. **Custo Elevado**: Soluções comerciais são inacessíveis para clínicas menores

### **Oportunidades para Nosso Sistema:**

- **Interface Intuitiva**: Foco na simplicidade e rapidez de uso
- **Explicabilidade Visual**: Apresentação clara das áreas de interesse na radiografia
- **Acessibilidade**: Solução web que funciona em qualquer dispositivo
- **Flexibilidade**: Adaptável a diferentes contextos clínicos

---

## 👥 Personas _(a serem desenvolvidas)_

---

## 🧠 Mapa de Empatia _(a ser desenvolvido)_

---
