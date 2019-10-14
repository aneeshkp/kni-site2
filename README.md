# kni-site2

1. ./knictl fetch_requirements github.com/aneeshkp/kni-site2.git ( don't use if you are re-installing, this nuke the site info)
(Behind the scene running prep_bm_host)

2. ./knictl prepare_manifests kni-site2  (kni-site match the repo name)
(pulls in the blue prints from Akrino and combines them with site yamls via Kostomize)


3./knictl deploy_masters kni-site2  (watch console)
Now finaly manifest is created, it will be copied into automation.
(takes few minutes )

4../knictl deploy_workers kni-site2 (runs terra form) (watch console)
