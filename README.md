# HVSO_TutorialManager_Sample
HVSO 튜토리얼 처리 방식에 대한 코드 일부

# 흐름 설명
튜토리얼인 경우, ScenarioGameManagment 가 해당되는 튜터리얼 정보(ScriptData)를 ScenarioExecuteHandler에 전달한다.<br>
ScenarioExecuteHandler는 내부에 정의되어 있는 튜토리얼 관련 함수들을 Queue 에 쌓아<br>
하나씩 Dequeue 하여 진행시킨다.<br>
여기서 중요한 점은 이 함수들은 클래스명과 동일하고,
그 클래스들은 ScenarioExecute 클래스를 상속받는다는 공통점이 있다.
