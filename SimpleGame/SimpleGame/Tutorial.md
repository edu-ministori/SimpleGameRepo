# Youtube Reference
https://www.youtube.com/watch?v=KRGPNi9mEMo&list=PL6xSOsbVA1eb_QqMTTcql_3PdOiE928up&index=2

# SFML ���̺귯�� ��ġ

## ������Ʈ
https://www.sfml-dev.org/download/sfml/2.6.0/

## �ٿ�ε�
- C++ 17 : 2022 / 32��Ʈ
 
## ���� ����

```
- SimpleGame - External - include
                        - lib
             - SimpleGame
             - SimpleGame.sln
```

- SFML > include ��ü ����/���� => SimpleGame > External > include
- SFML > lib ��ü ����/���� => SimpleGame > External > lib
- SFML > bin ��ü ���� => SimpleGame > SimpleGame

# VS 2022 ȯ�� ����

- VS 2022 ������ ��� ���� > Solution Platform > x86���� ����
- Solution Explorer > SimpleGame �̸��� ��Ŭ�� > Drop Down Menu > Properies
- ��� ���� ����
    - Configuration > All Configuration
    - Platform > win32
- C/C++ > General > Aditional include Directories
    - SFML���� �����ؿ� ����/������ �ִ� ��ġ(����)�� ����
    - $(SolutionDir) : ���� ������Ʈ ���� ǥ�� �Է�
    - ���� �Է� ���� : $(SolutionDir)\External\include

- LInker > Genaral > Additional Library Directories
    - SFML���� �����ؿ� ����/������ �ִ� ��ġ(����)�� ����
    - ���� �Է� ���� : $(SolutionDir)\External\lib

- Linker > Input > additional Dependancies
    - Configuration > Release ī�װ��� ����

```
  sfml-system.lib
  sfml-graphics.lib
  sfml-window.lib
  sfml-audio.lib
  sfml-network.lib
```

- Linker > Input > additional Dependancies
   - Configuration > Debug

```
  sfml-system-d.lib
  sfml-graphics-d.lib
  sfml-window-d.lib
  sfml-audio-d.lib
  sfml-network-d.lib
```
 
# Event

## Event ����
- ���, ��Ȳ�� ��ȭ
- Interface�� �����ؼ� ����� ��Ȳ�� ��ȭ
- Ű����, ���콺�� ����� ��Ȳ�� ��ȭ
    - Ű���� �̺�Ʈ : Ű �Է�
    - ���콺 �̺�Ʈ : ���콺 Ŭ��( Press / Release ), �� ��ũ��, ���� Ŭ��, ������
- ��ġ ��ũ�� : ��ġ, ��������, ��ġ
- �ε�

## Event Handling

- Event Delegate : �������� �̺�Ʈ�� ����
- Event Listening : �̺�Ʈ ����
- Event Handle : ������ �̺�Ʈ�� ���ؼ� ������ ����


# Game Loop

# SimpleGame ������Ʈ�� ������ Game Ŭ����

- ������ ���������� Control�ϴ� Ŭ����
- Enemy ����
- Player ����

