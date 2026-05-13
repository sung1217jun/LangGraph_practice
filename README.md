# LangGraph Multi-Agent Practice

LangGraph 기반 Multi-Agent 구조를 학습하고 구현하기 위한 프로젝트이다.
Ollama 로컬 LLM과 LangChain을 활용하여 문서 기반 질의응답(RAG) 흐름을 구성하였으며,
LangGraph를 이용한 Agent Workflow 구조를 실습 형태로 구현하였다.

<br>

## 프로젝트 개요

사용자의 질문이 입력되면 관련 문서를 검색하고,
검색된 문맥(Context)을 기반으로 LLM이 답변을 생성하는 RAG 구조를 구현하였다.

본 프로젝트는 실제 서비스 형태보다는
LangGraph 기반 Multi-Agent Workflow를 구성하고 활용하는 과정에 초점을 두고 진행하였다.

또한 챗봇 형태의 결과를 코드 실행 결과(Output)로 확인할 수 있도록 구성하였다.

---

## Multi-Agent 구조

LangGraph를 활용하여 다음과 같은 흐름으로 구성하였다.

* Retriever Agent
* Context 생성
* LLM Response 생성

질문이 입력되면 Retriever가 관련 문서를 검색하고,
검색된 문맥을 기반으로 LLM이 최종 답변을 생성하는 구조이다.

<img width="115" height="432" alt="image" src="https://github.com/user-attachments/assets/d6d93e54-6ed0-4311-ba4f-44091a525568" />


---

## RAG 구성

문서 기반 질의응답 시스템 구현을 위해 다음 과정을 수행하였다.

* TextLoader를 활용한 문서 로드
* RecursiveCharacterTextSplitter 기반 텍스트 청킹
* Ollama Embedding 생성
* ChromaDB Vector Store 저장
* Retriever 기반 문서 검색
* Context 기반 응답 생성

텍스트 청킹은 다음 설정으로 진행하였다.

* chunk_size = 100
* chunk_overlap = 20

---

## LangGraph Workflow

LangGraph를 활용하여 Agent 간 흐름을 그래프 구조 형태로 구성하였다.

```text id="3l7v2h"
User Question
    ↓
Retriever
    ↓
Vector DB Search
    ↓
Context 생성
    ↓
LLM 응답 생성
```

---

## 사용 기술

* Python
* LangChain
* LangGraph
* Ollama
* EXAONE 3.5
* ChromaDB

---

## 결과

코드 실행 결과를 통해 질문에 대한 문서 검색 및 응답 생성 과정을 확인할 수 있도록 구현하였다.

또한 LangGraph 기반 Multi-Agent Workflow 구성 및
RAG 파이프라인 구현이 가능함을 확인하였다.

<img width="2142" height="860" alt="image" src="https://github.com/user-attachments/assets/23cc4e3d-6510-428e-8841-6d193350c584" />

---

## 결과 요약

* LangGraph 기반 Multi-Agent 구조 구현
* RAG 기반 문서 검색 흐름 구성
* Ollama 로컬 LLM 활용
* ChromaDB Vector Store 적용
* Context 기반 질의응답 구현

---
