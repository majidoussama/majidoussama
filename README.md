GitHub Pro — Plan de professionnalisation
Oct 5, 2026 · @oussama
Quick wins — à faire en premier
1. Créer le README de profil (repo spécial majidoussama/majidoussama) — c'est l'élément manquant le plus visible : sans lui, un recruteur qui clique sur ton profil ne voit qu'une bio d'une ligne et trois repos, sans contexte. Le fichier prêt à l'emploi est livré séparément, prêt à pousser.
2. Ajouter une description (champ "About") au repo aws-cloud-security-lab — c'est le seul des trois à ne pas en avoir, alors que c'est ton projet le plus avancé techniquement.
3. Ajouter des Topics (tags) sur les trois repos — aucun n'en a actuellement. Les Topics sont le principal levier de visibilité dans la recherche GitHub et dans les filtres utilisés par les recruteurs tech ; 5 minutes par repo, impact disproportionné.
4. Corriger le fuseau horaire affiché sur le profil — GitHub montre actuellement UTC-12 (06:29 alors qu'il est après-midi/soir au Maroc), ce qui vient de l'heure système au moment des commits. Un fuseau aussi visiblement faux se voit au premier coup d'œil et donne une impression de configuration bâclée.
5. Harmoniser le lien LinkedIn — le profil pointe vers in/oussama-majid, mais l'URL réelle observée est in/oussama-majid-55b02b267 : vérifie quel est le bon slug et utilise-le partout (GitHub, CV, LinkedIn lui-même).
Niveau profil
Bio — la bio actuelle ("Cybersecurity Engineering student with experience in DS, AI, currently focused on expanding my cybersecurity expertise") est correcte mais générique et un peu longue à lire. Remplace-la par une version plus dense en mots-clés techniques :
🎓 Cybersecurity Engineering student (ENSIASD) · Cloud Security (AWS) · SIEM/SOC (Wazuh) · Network Security (FortiGate, pfSense) — open to internships
README de profil — absent actuellement. C'est le seul endroit où tu peux raconter une histoire (pas juste lister des repos) : qui tu es, tes 3 projets phares avec un résumé d'une ligne chacun, ta stack, tes certifications. Fichier complet livré séparément, prêt à pousser dans un nouveau repo nommé exactement majidoussama/majidoussama.
Pins — les trois repos apparaissent comme "popular" par défaut (choisis par l'algorithme de GitHub), pas explicitement épinglés par toi. Va dans "Customize your pins" et épingle-les toi-même, dans cet ordre : 1) aws-cloud-security-lab (cloud = compétence la plus recherchée actuellement, projet le plus récent), 2) soc-pentest-siem-lab (scope le plus large, SOC + pentest), 3) secure-network-fortigate-lab. Épingler explicitement montre une intention, pas un classement automatique.
Localisation — "ESSAOUIRA" en majuscules → "Essaouira, Morocco" pour plus de lisibilité à l'international.
Liens sociaux — garde LinkedIn (une fois l'URL corrigée) ; Instagram (majid__oussama) est un compte personnel (confirmé) — à retirer du profil GitHub : un recruteur qui clique dessus et tombe sur un compte perso peut nuire à l'image pro. Tu peux ajouter ton email et, si tu en crées un, un lien vers un portfolio.
Repo n°4 fantôme — l'onglet "Repositories" affiche 4, mais seuls 3 repos publics sont visibles/épinglables. Vérifie ce qu'est ce 4ème repo (privé ? fork ? brouillon ?) : s'il est présentable, rends-le public et documente-le comme les autres ; sinon laisse-le privé pour ne pas polluer le profil avec un repo à moitié fini.
Followers / activité — 0 followers est normal pour un étudiant, pas un problème en soi. Suivre quelques comptes pertinents (écoles partenaires, entreprises ciblées, figures de la cybersécurité, organisations comme OWASP) donne un profil plus "vivant" sans effort.
Graphe de contributions — l'activité est concentrée en rafales (juin à septembre), puis plus rien depuis. Pour les projets à venir, committe progressivement au fil du travail plutôt qu'en un seul bloc final : un historique de commits régulier (même petit) raconte un vrai processus de travail, ce qu'un recruteur technique regarde parfois directement.
Repo : aws-cloud-security-lab
C'est ton projet le plus technique et le plus récent (AWS réel, SIEM, WAF, pentest) — mais aussi celui avec le moins d'habillage GitHub.
Description manquante — ajoute ce one-liner dans "About" :
Secured a real AWS VPC with a custom Linux firewall (iptables/nftables), inline Suricata IDS/IPS and a Wazuh SIEM — CIS-hardened, pentested with Nmap/Burp Suite, remediated with a ModSecurity WAF. ~$2.79 total AWS cost.
Topics à ajouter : aws cloud-security wazuh siem suricata ids-ips iptables nftables cis-benchmark penetration-testing network-security devsecops cybersecurity
Image de preview sociale — dans Settings > General > Social preview, upload une capture du schéma d'architecture (tu en as déjà dans assets/) : c'est l'image affichée quand le lien est partagé sur LinkedIn ou dans un message ; actuellement c'est l'image par défaut GitHub.
Un seul commit sur main — pas rédhibitoire en soi, mais ça se voit. Pas besoin de réécrire l'historique (ne force-push jamais pour "simuler" un historique) : pour la suite, ajoute 2-3 commits naturels (ex. "docs: add architecture diagram", "chore: add GitHub topics") en faisant les changements ci-dessus — ça suffit à montrer un repo vivant.
Ce qui est déjà bon, à garder tel quel : structure propre (assets/, configs/, docs/, .gitignore, LICENSE MIT, ROADMAP.md), confirmation explicite dans le README qu'aucun secret n'est committé, et un ROADMAP.md qui assume honnêtement ce qu'il reste à faire (jours 4-5 de la semaine 4) — cette honnêteté est un vrai plus en entretien, ne la masque pas.
Repo : secure-network-fortigate-lab
C'est déjà le repo le mieux habillé des trois — description claire, README en 10 sections (architecture, modèle de sécurité, tests de validation, limites honnêtes, roadmap), et des badges déjà en place (FortiGate NGFW, Active Directory, VMware, Ubuntu 22.04, k6, MIT). Rien à changer sur le fond.
Le seul vrai manque : les Topics, absents malgré un contenu solide. Ajoute : fortigate ngfw active-directory network-segmentation dmz defense-in-depth glpi network-security cybersecurity
Langage affiché : PowerShell — à vérifier que ça reflète bien le contenu dominant (scripts de config) et pas juste un fichier qui fait du bruit statistique ; si la majorité du repo est de la documentation/config plutôt que du PowerShell, ce n'est pas grave en soi, mais c'est ce langage qui s'affiche en badge sur ton profil.
Image de preview sociale — même remarque que pour le repo AWS : tu as déjà un dossier diagrams/, utilise une des vues d'architecture comme image sociale.
Repo : soc-pentest-siem-lab
Ton projet avec le plus grand scope (4 zones, pfSense, Wazuh, AD, 23 attaques planifiées) et un README déjà très complet (11 chapitres). Comme pour le repo FortiGate, le contenu est bon — c'est l'habillage GitHub qui manque.
Topics à ajouter : pfsense wazuh siem active-directory soc blue-team red-team penetration-testing mitre-attack modsecurity owasp-crs cybersecurity
SECURITY.md déjà présent — c'est un vrai bon réflexe (peu de projets étudiants en ont un) : mets-le en avant dans le README de profil comme preuve de maturité pro, pas seulement dans ce repo.
Statut honnête "18/23 attaques exécutées" — garde cette formulation telle quelle plutôt que de la gonfler à "terminé". En entretien technique, un statut honnête avec un chiffre précis passe mieux qu'une affirmation vague de complétude, parce qu'il invite une question de suivi à laquelle tu as déjà la réponse.
Hygiène générale
• Topics partout : le changement le plus rentable de cette liste — gratuit, 5 minutes par repo, et c'est littéralement ce que les filtres de recherche GitHub et certains outils de sourcing recruteur utilisent en premier.
• Cohérence avec le README de profil : une fois le README de profil en place, vérifie que les trois one-liners qu'il donne pour chaque projet correspondent exactement aux descriptions "About" mises à jour sur chaque repo — évite d'avoir deux formulations différentes du même projet à deux endroits.
• Vérification "pas de secret committé" : déjà documentée explicitement sur aws-cloud-security-lab — fais la même vérification (et mentionne-la si vrai) sur les deux autres repos, c'est un signal de rigueur particulièrement apprécié des recruteurs techniques.
• Images de preview sociale sur les trois repos (actuellement l'image par défaut GitHub partout).
• Commits à l'avenir : pour le prochain projet, committe au fil de l'eau plutôt qu'en un seul bloc — pas besoin de réécrire l'historique existant, juste une habitude à prendre à partir de maintenant.
• Repo n°4 fantôme (voir section « Niveau profil ») — à clarifier avant toute communication publique du profil.
Checklist récapitulative
[ ] Créer le repo majidoussama/majidoussama et y pousser le README de profil fourni
[ ] Mettre à jour la bio du profil
[ ] Corriger le fuseau horaire (vérifier l'heure système / la config git avant le prochain commit)
[ ] Harmoniser l'URL LinkedIn
[ ] Épingler manuellement les 3 repos dans l'ordre recommandé
[ ] Retirer ou garder Instagram selon la nature du compte
[ ] Vérifier le 4ème repo listé mais non visible
[ ] Ajouter la description "About" sur aws-cloud-security-lab
[ ] Ajouter les Topics sur les 3 repos
[ ] Ajouter une image de preview sociale sur les 3 repos
[ ] Suivre quelques comptes pertinents sur GitHub
