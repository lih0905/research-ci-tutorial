# Github CI tutorial

인프런 [머신러닝 엔지니어 실무]() 강의 중 '리서치 코드 품질 관리' 섹션 강의 내용을 이용하여 CI 설정한 레포.

1. `.github/workflows/lint.yml` 설정을 통해 `black` 테스트를 통과하는지 체크

1. `.github/workflows/coverage.yml` 설정을 통해 `*_test.py` 에서 정의된 유닛테스트 통과하는지 체크

1. [Code Climate](https://codeclimate.com/)과 연동하여 코드에 대한 자동 리뷰 생성 및 아래 뱃지 추가

<a href="https://codeclimate.com/github/lih0905/research-ci-tutorial/maintainability"><img src="https://api.codeclimate.com/v1/badges/b76879ccdbf3a6f7b18a/maintainability" /></a>

<a href="https://codeclimate.com/github/lih0905/research-ci-tutorial/test_coverage"><img src="https://api.codeclimate.com/v1/badges/b76879ccdbf3a6f7b18a/test_coverage" /></a>

* Code Climate 에서 레포 연동 후 `Repo Settings > Test Coverage` 에서 토큰 복사하여 `coverage.yml` 파일에 붙여넣어야 함
* `Repo Settings > Github` 에서 연동 설정해야 함

## Requirements

```
black==19.10b0
coverage==4.3
codeclimate-test-reporter==0.2.3
```