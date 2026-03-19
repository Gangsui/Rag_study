# 01-Foundations

## 개요
이 파트는 LangChain 메시지 구조와 LangGraph의 상태 기반 워크플로우를 익히는 기초 실습입니다.

실습 노트북: [Message.ipynb](Message.ipynb)

## 간단 정리
- 환경 변수 로드 후 Gemini 모델을 초기화하고 기본 대화를 실행
- `SystemMessage`, `HumanMessage`, `AIMessage`, `ToolMessage`의 역할 확인
- 메시지 메타데이터(`name`, `id`) 사용 방식 실습
- 도구 호출 흐름(`tool_calls` -> `ToolMessage` -> 최종 응답) 실습
- `StateGraph`로 기본 그래프(START -> Node -> END) 구성
- `TypedDict` 기반 상태 스키마와 상태 업데이트 방식 확인
- `Annotated + add` 리듀서로 리스트 누적 병합 동작 확인
- `add_messages`를 사용한 메시지 상태 누적 처리 실습
- `add_conditional_edges`로 조건 분기(짝수/홀수) 라우팅 구현
- `Command`를 사용한 루프형 의사결정 노드 구현

## 핵심 키워드
- LangChain Messages
- StateGraph
- TypedDict State
- Reducer (add, add_messages)
- Conditional Edges
- Command Routing

## 다음 학습
- 동일 패턴을 작은 Agent 예제로 확장
- 메시지/상태 구조를 실제 RAG 파이프라인에 연결
