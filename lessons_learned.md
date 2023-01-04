1. To find out which process owns the file use process explorer (Download from microsoft page) find -> "Find handle or DLL"
2. Resharper disappeared: https://resharper-support.jetbrains.com/hc/en-us/articles/207241845-ReSharper-is-not-available-in-Visual-Studio-after-installation
3. C:\Users\paja\AppData\Roaming\Mozilla\Firefox\Profiles\vqalmf1p.default\chrome\userChrome.css -> to change all layout stuff for Firefox
4. https://git-scm.com/docs/git-reset#git-reset-Resetasinglefileintheindex -> reset single file to some point in repository
5.  windows credential store -> when you cant conntect to bitbucket´
6. https://www.jetbrains.com/help/resharper/Reference__Keyboard_Shortcuts.html
8. https://www.chiark.greenend.org.uk/~sgtatham/bugs.html
10. templates in VS - http://www.rhyous.com/2010/02/17/how-to-modify-the-default-new-class-template-in-visual-studio-2008/
11. git lfs:
https://github.com/git-lfs/git-lfs/blob/master/docs/man/git-lfs-fetch.1.ronn
git config lfs.fetchinclude oder lfs.fetchexclude
	1. git init 
	2. git remote add origin https://paja@bitbucket.zuehlke.com/scm/cates/tpem-cc-artifacts.git 
	3. git config lfs.fetchinclude "tpem-cc-tpem-cc-deliverables/influxdb" (als beispiel) 
	4. git pull 
12. http://10.48.15.100:5601/app/kibana#/visualize/edit/62ecdbe0-2877-11e9-a5d6-6d80b830579b
13. git branch --merged | grep -v '^* master$' | grep -v '^  master$' | xargs git branch -d
14. gem install name
15. https://github.com/nunit/docs/wiki/Console-Command-Line --explore
16. curl -vX PUT http://localhost:1443/parameters/import -H "Content-Type: application/json" -d @ex2.json
17. docker run --rm -v $(pwd):/opt swagger2markup/swagger2markup convert -i /opt/tpem_basic_configuration_api.yaml -f /opt/swagger -c /opt/config.properties $(pwd):/opt - rzutowanie z katalogu aktualnego na katalog w dockerze a dalej parametry swagger2markup
18. organize using not visible -> do that: https://resharper-support.jetbrains.com/hc/en-us/articles/206546519-There-are-no-Visual-Studio-items-in-context-menu
21. git cherry-pick https://stackoverflow.com/questions/1670970/how-to-cherry-pick-multiple-commits/3933416#3933416
22. splitting commits -  https://git-scm.com/docs/git-rebase#_splitting_commits
fleetmanagement.dentsplysirona
23. windows installer logs -> https://support.microsoft.com/en-us/help/223300/how-to-enable-windows-installer-logging
24. Remote desktop with ubuntu
	https://askubuntu.com/questions/592537/can-i-access-ubuntu-from-windows-remotely
	when you got blackscreen:
	https://github.com/neutrinolabs/xrdp/issues/598#issuecomment-303203274
	https://github.com/neutrinolabs/xrdp/issues/764#issuecomment-304576785
	https://github.com/neutrinolabs/xrdp/issues/598#issuecomment-320138326
	https://github.com/neutrinolabs/xrdp/issues/893
25. When you have problems with Microsoft.Graph in Azure Portal for KeyVault:
	https://blog.alanta.nl/2020/01/grant-yourself-access-to-azure-key-vault.html
26. KeyVault in Azure Functions:
	- https://blog.wille-zone.de/post/dependency-injection-for-azure-functions/
	- https://blog.wille-zone.de/post/azure-keyvault-for-azure-functions/
	- https://medium.com/statuscode/getting-key-vault-secrets-in-azure-functions-37620fd20a0b
27. Cache of matlab -> C:\Users\paja\AppData\Local\Temp\paja\mcrCache8.3
28. Spark links:
https://spark.apache.org/docs/latest/api/java/index.html?org/apache/spark/sql/Dataset.html
https://medium.com/@aristo_alex/how-apache-sparks-transformations-and-action-works-ceb0d03b00d0
https://stackoverflow.com/questions/53594029/is-it-a-good-practice-to-incur-spark-show-method-in-production-spark-job
https://livebook.manning.com/book/spark-in-action-second-edition/16-cache-and-checkpoint-enhancing-spark-s-performances/v-14/1
https://stackoverflow.com/questions/35127720/what-is-the-difference-between-spark-checkpoint-and-persist-to-a-disk
