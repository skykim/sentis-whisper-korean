# sentis-whisper-korean
Unity Sentis에서 Whisper를 사용하여 한국어를 인식하는 Speech-to-Text 예제입니다.

## 환경
- Unity 2023.2.20f1
- Sentis 1.6.0-pre.1

## 설정방법
- 본 저장소 Clone 후, [StreamingAssets.zip](https://drive.google.com/file/d/1C35rfXr6UxxpRrtU9h8-H8RJ0S0010zR/view?usp=drive_link)을 다운받아서 Assets/StreamingAssets에 압축해제합니다.

## 실행방법
- Scenes/STTScene을 오픈합니다.
- LeftCtrl 키를 누른 채로 한국말로 말하고, 이후 LeftCtrl 키를 떼면 녹음을 종료하고 바로 Speech-to-Text 작업을 시작합니다.
- 단, 첫 추론과정에서는 많은 시간이 소요될 수 있는 점 참고 바랍니다.
- 그 이외에 영어와 일본어를 비롯한, Whisper에서 지원하는 언어의 경우에도 사용할 수 있습니다.

## Whisper 모델변경
- [Whisper](https://github.com/openai/whisper)는 tiny, base, small, medium, large를 지원합니다.
- 현재 프로젝트에서는 small 모델을 사용중이며, 그 이외의 모델을 사용하고자 하는 경우에는 [torch-to-onnx-zoo](https://github.com/skykim/torch-to-onnx-zoo)를 참고하여 모델을 직접 변환하여 사용할 수 있습니다.
