# Optimizing Retrieval with MongoDB & Voyage 4

Este repositório contém os materiais práticos e exemplos de código apresentados no webinar sobre otimização de sistemas de recuperação (Retrieval) para aplicações de IA. 

O foco principal é demonstrar como utilizar a nova série de modelos Voyage 4 em conjunto com o MongoDB Atlas para criar sistemas de RAG (Retrieval-Augmented Generation) eficientes, escaláveis e de baixo custo.

🚀 Visão Geral

A nova geração de modelos da Voyage AI introduz o conceito de Shared Embedding Spaces, permitindo que diferentes modelos (Large, Lite, Nano) operem no mesmo espaço vetorial.

Isso elimina a necessidade de reindexar todo o seu banco de dados ao trocar de modelo para otimizar latência ou custo.

🛠️ Principais Técnicas Abordadas

Asymmetric Retrieval: Uso de modelos distintos para vetorizar consultas e documentos (ex: voyage-4-lite para queries e voyage-4-large para documentos), 
otimizando a performance sem perder precisão.

Vector Quantization: Compressão de vetores de alta precisão (float32) para formatos binários, reduzindo drasticamente o consumo de memória e custos de infraestrutura no MongoDB.

Dimensionality Reduction: Estratégias para manter a relevância semântica utilizando vetores menores.

MongoDB Integration: Implementação prática utilizando o driver pymongo para gerenciar coleções de vetores e realizar buscas semânticas.

