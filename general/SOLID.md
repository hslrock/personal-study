
## SOLID 원칙 공부 노트
각 ipynb 설명내용 참조: https://velog.io/@haero_kim/SOLID-%EC%9B%90%EC%B9%99-%EC%96%B4%EB%A0%B5%EC%A7%80-%EC%95%8A%EB%8B%A4
```mermaid
graph TB
    SOLID(SOLID 원칙) --> S(단일 책임 원칙)
    SOLID --> O(개방/폐쇄 원칙)
    SOLID --> L(리스코프 치환 원칙)
    SOLID --> I(인터페이스 분리 원칙)
    SOLID --> D(의존성 역전 원칙)

    S -->|변경의 이유는 하나만| ComponentA
    O -->|확장에는 열려 있고, 수정에는 닫혀 있어야 함| ComponentB
    L -->|서브 타입은 기반 타입으로 치환 가능해야 함| ComponentC
    I -->|특정 클라이언트에 맞춘 인터페이스 설계| ComponentD
    D -->|상위 모듈은 하위 모듈에 의존하지 않음| ComponentE

    subgraph 설명
        ComponentA["하나의 클래스는 하나의 책임만 가져야 한다."]
        ComponentB["소프트웨어는 확장에는 열려 있으나, 기존 코드 수정에는 닫혀 있어야 한다."]
        ComponentC["하위 클래스는 상위 클래스를 대체할 수 있어야 한다."]
        ComponentD["클라이언트는 사용하지 않는 메서드에 의존하지 않아야 한다."]
        ComponentE["상위 모듈은 하위 모듈에 의존하지 않고, 추상화에 의존해야 한다."]
    end

    classDef highlight fill:#f9f,stroke:#333,stroke-width:2px;
    class S,O,L,I,D highlight;



```

### 1. SRP
이미지 참조: https://www.evertop.pl/en/understanding-solid-principles-single-responsibility/
![alt text](image/srp.png)

### 2. OCP
이미지 참조:https://www.youtube.com/watch?v=H7oyqncSgEE
![alt text](image/orp.png)

### 3. LSP
이미지 참조:https://www.linkedin.com/pulse/liskov-substitution-principle-mamata-raote-she-her-
![alt text](image/lsp.png)

### 4. ISP
이미지 참조:https://walbatrossw.github.io/oop/2018/07/27/07-solid-isp.html
![alt text](image/isp.png)

### 5. DIP
이미지 참조: https://medium.com/@kedren.villena/simplifying-dependency-inversion-principle-dip-59228122649a
![alt text](image/dip.png)