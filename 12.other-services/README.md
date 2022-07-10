# DB와 API Gateway 구성하기
[DynamoDB](https://aws.amazon.com/ko/dynamodb/?nc1=h_ls) 는 AWS의 noSQL 데이터서비스입니다. 기존에 흔히 사용하시는 Oracle이나 Mysql의 경우, 데이터를 보관하는 형태인 스키마를 정의하고, 이 스키마를 이용해서 데이터를 저장하게 됩니다. 하지만 이 DynamoDB 와 같은 noSQL 데이터베이스를 이용하시면 이런 스키마 없이 데이터를 원하는 형태로 자유롭게 저장할 수 있습니다. 또한, AWS의 완전관리형 서비스인만큼 서버 관리도 신경쓰지 않으셔도 됩니다.

[API Gateway](https://aws.amazon.com/ko/api-gateway/) 는 AWS의 api 관리 서비스입니다. API 란 외부에서 기업의 서비스를 이용하려고 할때 규격을 정해주는 것을 의미합니다. 일종의 형식을 정해놓고, 이 형식대로 기업의 서비스를 호출하면 기업은 서비스를 제공해 주는 약속이라고 생각하시면 됩니다. API Gateway는 이런 API 를 관리해주고 API 를 통해 외부에서의 호출이 왔을때 대문 역할을 하는 AWS 서비스입니다.

이번 세션에서는 이 두가지 서비스를 생성하고 lambda 와 연결해서 좀 더 완성도 높은 서비스를 만들어 보겠습니다. DynamoDB 를 연결해서 데이터도 저장해보고, 아까는 Lambda functions URL 을 통해서 접근했다면 이번에는 API Gateway를 이용해서 접근해 보겠습니다.
