# Datadog Azure Integration Update

## 1. Azure Integration 기간 연장 방법

1. Azure Portal 접속

2. Microsoft Entra ID

3. Manage > App registrations

4. All applications 〉 Monitoring Reader

5. Manage 〉 Certificates & secrets

6. 기존 만료된 ```Client Secret``` 경신은 불가능하므로 새로 생성

6. ```+ Mew client secret``` 클릭 후 신규 생성

> 생성 예제
> - Description: DatadogClientSecret
> - Expires: 730 days (24 months)
> - Add
> 
> | Description | Expires | Value | Secret ID |
> | --- | --- | --- | --- |
> | DatadogClientSecret | 11/14/2024 ⓘ | o6e************ | 88575ab3-********** |
> | DatadogClientSecret | 1/8/2027 | 323************ | a907151c-********** |

7. Value 값 복사

8. Datadog 접속

9. lntegations 〉 Azure

10. GeneraI 〉 CIient Secret Value 에 붙여넣기 후 저장
