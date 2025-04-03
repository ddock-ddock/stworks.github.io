---
# the default layout is 'page'
icon: fas fa-info-circle
order: 1
mermaid: true
---

STworks.kr은 똑똑[^dkdk] 주식회사에서 만든 스타트업 영업보고(투자자보고) 시스템입니다.

## 스타트업 업무의 일반 흐름
원하는 메뉴를 클릭하시면 해당 매뉴얼로 이동합니다.

```mermaid
flowchart TD

subgraph s1["설정"]
    n1["STworks 가입 요청 (VC)"]
    n2["STworks 회사(회원)가입<br>scm002"]
    n3["STworks 로그인<br>scm001"]
    n4["STworks 사용자 관리<br>scm006"]
    n5["STworks 역할/권한 관리<br>scm007"]
end

subgraph s2["투자자 관리"]
    n6["영업보고 목록<br>sbr001~003"]
    n7["영업보고 상세(보고서 작성)<br>sbr004"]
    n9["의결"]
    n10["주주총회<br>ssa001~7"]
    n11["동의 및 협의"]
end

subgraph s3["증권관리"]
    n8["주주명부<br>sct001"]
end
  
subgraph s4["이메일 회신"]
    n12["주주총회 메일 회신"]
    n13["주주총회 결과 메일 회신"]
end

    n1 --> n2
    n2 --> n3
    n3 --> n4
    n4 --> n5
    n5 --> s2 & s3
    n6 --> n7
    n9 --> n10 & n11
    n10 --> s4
    n12 --> n13

    style n1 fill:#e6ffe6,stroke:#66cc66,stroke-width:2px,rx:10,ry:10,color:#333333,fontColor:#333333

    click n2 "{% post_url 2024-09-01-scm002 %}"
    click n3 "{% post_url 2024-09-02-scm001 %}"
    click n4 "{% post_url 2024-09-03-scm006 %}"
    click n5 "{% post_url 2024-09-04-scm007 %}"
    click n6 "{% post_url 2024-09-05-sbr001 %}"
    click n7 "{% post_url 2024-09-06-sbr004 %}"
    click n8 "{% post_url 2024-09-07-sct001 %}"
    click n10 "{% post_url 2024-09-08-ssa002 %}"
    click n12 "{% post_url 2024-09-09-sie002 %}"
    click n13 "{% post_url 2024-09-10-sie003 %}"
```



버그 및 문의 사항은 다음 이메일로 보내주세요: **[we@ddock.kr](mailto:we@ddock.kr)**


---

[^dkdk]:똑똑(ddock.kr)은 대한민국 벤처투자전문회사인 DSC인베스트먼트가 VC업계의 업무 방식을 혁신하고자 만든 IT자회사입니다. 
