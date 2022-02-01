# Untracked
### 추적되지 않고 있는 상태
* 파일을 새로 생성하고 그 파일을 한번도 git add해주지 않았을때의 상태

# Tracked
### 파일이 git에 의해 그 변동사항이 추적되고 있는 상태
* 아래의 3가지로 나뉜다
## Staged
* 파일의 내용이 수정되고 나서 staging area에 올라와있는 상태
<br>
<font color = "yellow">
새로 생성한 파일에 내용을 쓰고 git add 해주거나
<br>
한번이라도 커밋에 포함됐었던 파일이라도 내용을 수정하고 git add를 해준 상태
</font> 
## Unmodified
* 현재 파일의 내용이 최신 커밋의 모습과 비교했을때 전혀 바뀐게 없는 상태
<font color = "yellow">
<br>
커밋을 하고 난 직후에는 working direcotry안의 모든 파일들이 이 상태가 된다.
</font>
## Modified
* 최신 커밋의 모습과 비교했을 때 조금이라도 바뀐 내용이 있는 상태

# 상태전환
## Add the file
* Untracked상태의 파일을 처음으로 git add 해주면 Staged상태가 된다.
## Edit the file
* 최신 커밋과 비교했을 때 차이가 없는 Unmodified상태의 파일의 내용을 수정하면 Modified상태가 된다.
## Stage the file
* Modified 상태의 파일을 git add해주면 Staged상태가 된다.
## Remove the file
* 파일을 삭제하면 git에서 더이상 인식하지 않는다.
## Commit
* 커밋을 하면 staging area에 있던 파일들이 커밋에 반영되고, 모든 파일들은 최신 커밋과 차이가 없게 되니까 Unmodifed상태가 된다.