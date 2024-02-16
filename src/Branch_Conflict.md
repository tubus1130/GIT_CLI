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

#### 각 브랜치마다 커밋 만들고 로그확인

![img_4.png](img/log_graph2.png)