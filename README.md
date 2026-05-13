# LangGraph Multi-Agent Practice

LangGraph 기반 Multi-Agent 구조를 학습하고 구현하기 위한 프로젝트이다.  
Ollama 로컬 LLM과 LangChain을 활용하여 Agent Workflow 구조를 실습 형태로 구현하였다.

<br>

## 프로젝트 개요

본 프로젝트는 LangGraph를 활용하여 Multi-Agent Workflow를 구성하고,  
각 Agent의 실행 흐름을 연결하는 과정을 실습하기 위해 진행하였다.

또한 코드 실행 결과(Output)를 통해  
챗봇 형태의 응답 생성 결과를 확인할 수 있도록 구성하였다.

---

## Multi-Agent 구조

LangGraph를 활용하여 Agent 간 흐름을 구성하였다.

사용자의 입력이 들어오면 각 Agent가 순차적으로 실행되며,  
최종적으로 LLM을 통해 응답을 생성하는 구조이다.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d6d93e54-6ed0-4311-ba4f-44091a525568" width="150"/>
</p>

---

## LangGraph Workflow

LangGraph를 활용하여 Agent 간 흐름을 그래프 구조 형태로 구성하였다.

```text
User Input
    ↓
Agent Workflow
    ↓
LLM Response
```

---

## 구현 내용

본 프로젝트에서는 다음 내용을 중심으로 실습하였다.

* LangGraph 기반 Workflow 구성
* Agent 실행 흐름 연결
* Ollama 기반 LLM 응답 생성
* 코드 실행 결과(Output) 확인

---

## 사용 기술

* Python
* LangChain
* LangGraph
* Ollama
* EXAONE 3.5

---

## 결과

코드 실행 결과를 통해  
LangGraph 기반 Multi-Agent Workflow 구성 및  
LLM 응답 생성 과정을 확인할 수 있었다.

<p align="center">
  <img src="https://github.com/user-attachments/assets/23cc4e3d-6510-428e-8841-6d193350c584" width="900"/>
</p>

---

## 결과 요약

* LangGraph 기반 Multi-Agent 구조 구현
* Agent Workflow 구성
* Ollama 로컬 LLM 활용
* 코드 실행 결과 기반 응답 확인
