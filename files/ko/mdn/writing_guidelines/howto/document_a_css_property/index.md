---
title: CSS 속성을 문서화하는 방법
slug: MDN/Writing_guidelines/Howto/Document_a_CSS_property
l10n:
  sourceCommit: aa66311219951396e7305df61eb31831360d2c79
---

{{MDNSidebar}}

[CSS](/ko/docs/Web/CSS) 표준이 발전함에 따라 새로운 속성이 항상 추가되고 있습니다. MDN 웹 문서의 [CSS 참고서](/ko/docs/Web/CSS/Reference)는 이런 개발과 함께 최신 상태로 유지되어야 합니다. 이 문서에는 CSS 속성 참고서 페이지를 만들기 위한 단계별 지침을 제공합니다.

각 CSS 속성 참고서 페이지는 동일한 구조를 따릅니다. 특히, 이는 독자들에게 표준 참조 페이지 형식에 익숙해진 후에 정보를 더 쉽게 찾을 수 있도록 도와줍니다.

## 1단계 - 문서화할 속성을 결정하기

먼저 문서화하려는 CSS 속성을 찾아야 합니다. 여러분은 페이지가 누락되었거나 [이슈 목록](https://github.com/mdn/content/issues)에서 보고된 누락된 콘텐츠를 보았을 수 있습니다. CSS 속성에 대한 자세한 내용은 관련 사양(예: [W3C 명세서](https://www.w3.org/Style/CSS/) 또는 Gecko나 Blink와 같은 렌더링 엔진에 사용되는 비표준 속성에 대한 버그 보고서)을 찾아야 합니다.

> [!NOTE]
> W3C 명세서를 사용하는 경우, 게시된 버전(예: Working Draft)이 아닌 항상 **Editor's Draft**(왼쪽의 빨간색 배너 참고)를 사용하십시오. Editor's Draft는 항상 최종 버전에 더 가깝습니다!

구현과 사양이 다른 경우, 구현 버그에서 자유롭게 알려주십시오. 다음 상황 중 하나가 가능합니다.

- 구현 버그일 수 있습니다(그리고 후속 버그가 제출될 것입니다).
- 새로운 명세서 게시가 지연될 수 있습니다.
- 명세서에 오류가 있을 수 있습니다(이 경우, 명세서 버그를 제출하는 것이 좋습니다).

## 2단계 - CSS 속성 데이터베이스 확인하기

구문 또는 애니메이션 가능 여부와 같은 CSS 속성의 여러 특성은 여러 페이지에서 언급되므로 즉석 데이터베이스에 저장됩니다. 페이지에서 사용할 매크로는 데이터베이스에 저장된 속성 정보가 필요하므로 [이 정보가 있는지 확인하는 것부터 시작하십시오](https://github.com/mdn/data/blob/main/docs/updating_css_json.md).

## 3단계 - CSS 속성 페이지 만들기

준비는 끝났습니다! 이제 실제 CSS 속성 페이지를 추가할 수 있습니다. 새 CSS 속성 페이지를 만드는 가장 쉬운 방법은 기존 CSS 속성 페이지의 콘텐츠를 복사하고 새 속성에 맞게 편집하는 것입니다. 새 페이지를 만들려면 [페이지를 만드는 방법](/ko/docs/MDN/Writing_guidelines/Howto/Creating_moving_deleting) 가이드의 지침을 참조하십시오.

참고서 페이지를 만들 때 여러분은 예제를 추가하고 싶을 것입니다. 예제를 추가하려면 [라이브 샘플에 자습서](/ko/docs/MDN/Writing_guidelines/Page_structures/Live_samples)를 따르십시오. 만들고 있는 속성 페이지는 한 가지 속성에 대한 것이므로 추가하는 예제도 전체 사양이 사용되는 방식이 아니라 한 속성이 개별적으로 동작하는 방식을 보여주어야 합니다. 따라서 `list-style-type` 속성 예제는 좋은 효과를 생성하기 위해 다른 속성, 의사 클래스 또는 의사 요소와 결합하는 방법이 아니라 속성에 여러가지 값을 사용한 결과를 보여주어야 합니다. 튜토리얼과 안내서를 작성하여 더 많은 것을 보여줄 수 있습니다.

## 4단계 - 콘텐츠 검토 받기

속성 페이지를 만든 후 풀 리퀘스트로 제출합니다. 여러분의 페이지를 검토할 검토 팀 구성원이 자동으로 할당됩니다.
