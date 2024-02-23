### ✏️ 브랜치

---

>`master 브랜치` : 저장소를 처음 만들면, Git은 master라는 브랜치를 자동생성함<br>
> 새로운 브랜치를 만들어 checkout하지 않는 한, 모든 작업은 master브랜치에서 일어남

#### 💭 브랜치 그래프로 보기

```
# 브랜치를 전체보여주고 시각적으로 한줄로 로그표시
git log --all --graph --oneline
```

![img_1.png](img/log_graph.png)

---

#### 💭 브랜치 생성

```
# 브랜치 종류 모두 보여줌
git branch

# 브랜치 추가
git branch 브랜치명
```

![img_2.png](img/branch생성.png)

---

#### 💭 브랜치 이동

```
# 해당 브랜치로 이동
git checkout 브랜치명
```

![img_3.png](img/branch_checkout.png)

#### 💭 각 브랜치마다 커밋 만들고 로그확인

![img_4.png](img/log_graph2.png)

---

#### 💭 브랜치 병합

![img.png](img/merge.png)

```
# 브랜치 병합(기준이 되는 브랜치로 이동해서 다음 명령어 실행)
git merge 병합하고 싶은 브랜치명
```

#### 💭 merge(충돌 x)

![img_1.png](img/merge_충돌x.png)

- 서로 다른 파일 병합할 경우
- 같은파일, 다른부분 병합할 경우

#### 💭 merge(충돌 났을 경우)

![img_3.png](img/merge_충돌o.png)

- 같은파일, 같은부분 병합할 경우

![img_4.png](img/conflict1.png)

- <<<<<과 >>>>>사이가 충돌난 부분이다.
- 이 부분을 사용자가 따로 충돌을 해결하고 커밋해야된다.

![img_5.png](img/conflict2.png)

![img_6.png](img/conflict3.png)

#### 💭 3-way-merge

![img_7.png](img/3_way_merge.png)

- here, there => 브랜치
- base => 브랜치들의 뿌리 커밋

#### 💭 merge 도구
- p4merge

```
# 설정
git config --global merge.tool p4merge
git config --global mergetool.p4merge.path 'C:\Program Files\Perforce\p4merge.exe'

# 실행
git mergetool
```

![img.png](img/p4merge.png)