# Git-branching


## Bianny Holguin 2021-1274

### Resumen Comandos 

**Principal**
- **Nivel 1.1**
git commit;
git commit;

- **Nivel 1.2**
git branch bugFix;
git checkout bugFix;

- **Nivel 1.3**
git checkout -b bugFix;
git commit;
git checkout master;
git commit;
git merge bugFix;

- **Nivel 1.4**
git checkout -b bugFix;
git commit;
git checkout master;
git commit;
git checkout bugFix;
git rebase master;

- **Nivel 2.1 ** 
git checkout C4;

- **Nivel 2.2**
git checkout C4^;

- **Nivel 2.3**
git branch -f master C6;
git branch -f bugFix C0;
git checkout C1;

- **Nivel 2.4**
git reset local~1;
git checkout pushed;
git revert pushed;

- **Nivel 3.1**
git cherry-pick C3 C4 C7;

- **Nivel 3.2**
git rebase -i master~4 --aboveAll;

- **Nivel 4.1**
git checkout master;
git cherry-pick C4;

- **Nivel 4.2**
git rebase -i caption~2 --aboveAll;
git commit --amend;
git rebase -i caption~2 --aboveAll;
git branch -f master caption;

- **Nivel 4.3**
git checkout master;
git cherry-pick C2;
git commit --amend;
git cherry-pick C3;

- **Nivel 4.4**
git tag v0 C1;
git tag v1 C2;
git checkout C2;

- **Nivel 4.5**
git commit;

- **Nivel 5.1**
git rebase master bugFix;
git rebase bugFix side;
git rebase side another;
git rebase another master;

- **Nivel 5.2**
git branch bugWork master~^2~;

- **Nivel 5.3**
git checkout one;
git cherry-pick C4 C3 C2;
git checkout two;
git cherry-pick C5 C4 C3 C2;
git branch -f three C2;

**Remoto**

- **Nivel 1.1**
git clone;

- **Nivel 1.2**
git commit;
git checkout o/master;
git commit;

- **Nivel 1.3**
git fetch;

- **Nivel 1.4**
git pull;

- **Nivel 1.5**
git clone;
git fakeTeamwork master 2;
git commit;
git pull;

- **Nivel 1.6**
git clone;
git commit;
git commit;
git push;

- **Nivel 1.7**
git clone;
git fakeTeamwork;
git commit;
git pull --rebase;
git push;

- **Nivel 2.1**
git fetch;
git rebase o/master side1;
git rebase side1 side2;
git rebase side2 side3;
git rebase side3 master;
git push;

- **Nivel 2.2**
git checkout master;
git pull;
git merge side1;
git merge side2;
git merge side3;
git push;

- **Nivel 2.3**
git checkout -b side o/master;
git commit;
git pull --rebase;
git push;

- **Nivel 2.4**
git push origin master;
git push origin foo;

- **Nivel 2.5**
git push origin master~1:foo;
git push origin foo:master;

- **Nivel 2.6**
git fetch origin master~1:foo;
git fetch origin foo:master;
git checkout foo;
git merge master;

- **Nivel 2.7**
git push origin :foo;
git fetch origin :bar;

- **Nivel 2.8**
git pull origin bar:foo;
git pull origin master:side;
