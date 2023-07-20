# # AIFFEL Campus Online 5th Code Peer Review Templete
- 코더 : 양주영
- 리뷰어 : 어윤석

# PRT(PeerReviewTemplate) 
각 항목을 스스로 확인하고 토의하여 작성한 코드에 적용합니다.

- [X] 코드가 정상적으로 동작하고 주어진 문제를 해결했나요?
  > 정상적으로 동작하고 한국어 질문에 답을 출력하는 챗봇을 구현하였습니다.
- [X] 주석을 보고 작성자의 코드가 이해되었나요?
  > 필요한 부분에 주석으로 설명되어있어 코드를 이해하는데 도움이 되었습니다.
- [X] 코드가 에러를 유발할 가능성이 없나요?
  > 에러가 발생할 것 같은 부분을 발견하지 못했습니다.
- [X] 코드 작성자가 코드를 제대로 이해하고 작성했나요?
  > 정규표현식에 변화를 주며 테스트하였고, 코드를 잘 이해하고 작성하였습니다.
- [X] 코드가 간결한가요?
  > 동작을 위해 필요한 코드로 간결하게 작성되었습니다.

# 예시
1. 코드의 작동 방식을 주석으로 기록합니다.
2. 코드의 작동 방식에 대한 개선 방법을 주석으로 기록합니다.
3. 참고한 링크 및 ChatGPT 프롬프트 명령어가 있다면 주석으로 남겨주세요.
#### 학습 문장의 길이를 분석하여 MAX_LENGTH를 결정하는 부분을 참고 할 수 있었습니다.
```python
def visualize_sentence_lengths(sentences):
    # 각 문장의 단어 수를 세어줍니다
    word_counts = [len(sentence.split()) for sentence in sentences]

    # 최대 단어 수를 계산하여 히스토그램의 구간 수를 설정합니다
    max_word_count = max(word_counts)

    # 단어 수에 대한 히스토그램을 생성합니다
    # align='left': 이 매개변수는 히스토그램의 막대 정렬을 제어
    # rwidth=0.8: 이 매개변수는 히스토그램에서 막대의 상대적 너비를 제어
    plt.hist(word_counts, bins=range(1, max_word_count + 2), align='left', rwidth=0.8)
    plt.xlabel('words')
    plt.ylabel('sentence')
    plt.xticks(range(1, max_word_count + 1))
    plt.show()

visualize_sentence_lengths(questions)
visualize_sentence_lengths(answers)
```

# 참고 링크 및 코드 개선
개인적으로 내용에 대한 이해가 아직 많이 부족해서 개선할 부분이나 참고할 만한 내용을 찾지 못했습니다.
```python
# 코드 리뷰 시 참고한 링크가 있다면 링크와 간략한 설명을 첨부합니다.
# 코드 리뷰를 통해 개선한 코드가 있다면 코드와 간략한 설명을 첨부합니다.
```
