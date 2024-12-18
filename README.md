Git Komutları
Patika.dev Git eğitimi sırasında aldığım notlar.

İnit
git init —> İlk projeyi oluşturma.
Add
git add * . -a —> Repoya dosya ekleme.
Commit
git commit -m "First Commit" —> Snapshot almak için.
Amend
git amend —> Son yapılan commiti geri alır.
git commit --amend —> Son yapılan commit üzerine ekler (yeni commit oluşturmaz).
git commit --amend -m "yeni mesaj" —> Son commitin mesajını değiştirir.
Status
git status —> Durumu görmek için.
Push, Pull ve Clone
git push —> Uzak bilgisayara göndermek için.
git pull —> Uzak bilgisayardan çekmek için.
git clone —> Projeyi kopyalayarak çeker.
Checkout
git checkout isim —> İsim adındaki brancha geçiş yapar.
git checkout -b isim2 —> isim2 adında bir branch oluşturup direkt geçiş yapar.
Rm
git rm —> Dosya ve klasör silmek için.
git rm --cached name —> Staged ortamına eklenmiş bir dosyanın takibinin bırakılması yani untracked (izlenmeyen) hale getirilmesi sağlar.
Diff ve Log
git diff —> Değişiklikleri gösterir.
git diff log1 .. log2 index.md —> index.md'nin log1 ve log2 arasındaki değişiklikleri gösterir.
git log —> Tüm snapshotları gösterir.
git log -n 1 —> Son snapshotı gösterir (2, 3 diye devam eder).
Revert
git revert lognumarasi —> lognumarasi logunu geri alır. Geri alma logunu geri alırsak eski haline döner.
Reset
git reset --hard donmekistediginlog —> Dönmek istediğin yere kadar olan logları siler.
Branch
git branch —> Branch'ları gösterir.
git branch isim —> "isim" adında bir branch oluşturur.
git branch -d isim2 —> isim2 adlı branch'i siler.
Touch
touch isim.md —> isim.md adında bir dosya oluşturur.
Stash
git stash —> Son commite kadar olan bölümü geçici olarak depolar ve son commite döner.
git stash list —> Stash'ları gösterir.
git stash clear —> Stash kaydını siler.
git stash pop —> En üstteki kaydı geri getirir ve kaydı listeden siler.
git stash apply stash@{1} —> 2. stash kaydına döner ama listeden silmez.
git stash drop stash@{0} —> 1. stash kaydını siler.
Merge
git merge branch_ismi —> Master ile branch_ismi'ni birleştirir.
git merge --squash branch_ismi —> Master ile branch_ismi'ni birleştirir fakat branch_ismi'nin commit geçmişini tek bir commit'de toplar. Geçmişin çok uzamasını engeller. Bunu yaptıktan sonra son bir commit daha yapmamızı bekler.
git merge --abort —> Yapmakta olduğumuz merge'ü iptal eder.
Rebase
git rebase branch_ismi —> Değişiklikleri sanki ana branch'da yapmış gibi gösterir ve commit tarihçesine bir şey eklemez.
