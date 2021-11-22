---
layout: post
title:  "Chapter 1-1 - a Reliable, Scalable, and Maintainable Applications"
---

# Designing data intensive applications 첫 번째 챕터 요약본 입니다.

### Terminologies
DDIA책에서는 대부분의 소프트웨어 시스템에서 중요시 되는 아래 3가지 내용 들을 중점적으로 다룬다.

**Reliability** <br /> 시스템은 correctly 동작해야 한다. 하드웨어적 / 소프트웨어적 혹은 human error가 발생한 상황에서도 설계시 의도했던 function을 수행 할 수 있어야 한다.<br />
**Scalability** <br /> 데이터, 트래픽의 볼륨 및 시스템의 복잡도가 증가함에 따라 우리는 해당 적절히 다룰수 있어야 한다.<br />
**Maintainability** <br /> 시스템은 유지 보수 및 새로운 use case에 적용 할 시 productive하게 동작할 수 있도록 설계되어야 한다.

- Reliability
  - 모두가 "reliable"이 무슨 뜻인지에 대해 직관적 개념은 있지만, 소프트웨어적 측면으로는 전형적으로 아래 사항들을 만족을 할때 Reliable하다고 표현한다.
    - 어플리케이션이 유저가 예상한대로 동작을 한다
    - 유저의 실수 혹은 잘못된 사용방법에도 "tolerate" 할 수 있어야 한다
    - 주어진 Requirements즉, 예상되는 data / traffic 볼륨에도 충분히 수행할 수 있어야 한다.
    - malicious 한 인풋 (unauthorized access / abuse)를 막을 수 있어야 한다.
  - 즉 우리가 의미하는 reliability란 fault-tolerant or resilient 와도 같다. 여기서 주의할 점은 fault란 <span style="color:red">failure</span>와는 다른 개념이다. **fault** 는 시스템 내부 하나의 component가 약간 오작동(?) 하는것이라 하면 **failure**는 전체 시스템의 동작이 멈추는것과 동치한다. 
  - 실제 예제들이 어떻게 fault-tolerant한 시스템을 구성했는지는 아래의 링크를 참조하면 좋을것 같다
    - https://www.usenix.org/system/files/conference/osdi14/osdi14-paper-yuan.pdf
    - https://medium.com/netflix-techblog/the-netflix-simian-army-16e57fbab116
  - Security가 중요시 여겨지는 앱에서는 fault-preventing이 더 중요시 여겨지지만 해당 책에서는 전자의 경우를 중점적으로 다룬다
- Hardware Faults
- Software Erros
- Human Errors
- Scalability
- Describing Load
- Describing Performance
- Approaches for Coping with Load
- Maintainability
- Operability: Making life easy for operations
- Simplicity: Managing Complexity
- Evolvability: Making Change Easy
