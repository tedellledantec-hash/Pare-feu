# Pare-feu
1. Définition d’un pare-feu : 
   
Un pare-feu (firewall) est un logiciel ou matériel qui contrôle et filtre les communications entre réseaux selon une politique de sécurité.
Il agit comme un sas de sécurité : tout trafic entrant/sortant doit être autorisé.

2. Zones de sécurité


Extranet : Réseau externe, peu contrôlé et ouvert.
Exemple : Internet.


Intranet : Réseau interne, très protégé avec un accès restreint.
Exemple : Réseau local d’une entreprise.


DMZ : Zone intermédiaire, moins protégée, qui héberge les services publics.
Exemple : Serveurs web, FTP, DNS.


3. Types de pare-feu


Stateless (filtrage simple) :
Filtre les paquets selon l’IP, le port et le protocole, sans mémoire des connexions.
Avantages/Inconvénients : Simple, mais peu souple (ex. problèmes avec FTP).


Stateful (avec état) :
Conserve l’état des connexions pour un filtrage dynamique.
Avantages/Inconvénients : Plus sécurisé, gère les protocoles complexes.


Proxy applicatif :
Filtre au niveau applicatif (ex. proxy HTTP).
Avantages/Inconvénients : Très sécurisé, mais moins performant.


4. Politiques de sécurité


Tout ce qui n’est pas interdit est autorisé :
Approche permissive (moins sécurisée).


Tout ce qui n’est pas autorisé est interdit :
Approche restrictive (recommandée).


5. Fonctionnalités clés


Filtrage :
Autorise ou refuse les communications selon des règles (IP, port, protocole, utilisateur).


NAT/PAT :

NAT : Traduction d’adresse réseau, permet de partager une IP publique entre plusieurs appareils.
PAT : Utilise des ports pour partager une IP publique (ex. pour les connexions FAI).


Isolation des zones :
Sépare les réseaux en zones de sécurité (ex. DMZ).


Journalisation :
Enregistre les tentatives de connexion pour audit.


6. Exemples de pare-feux


Logiciels :
pfSense, OPNSense, Windows Firewall, Zone Alarm, Comodo Firewall Pro.


Matériels :
FireBox (WatchGuard), Netgear, Sophos XG Firewall, Cisco ASA 5500-x.



7. Vocabulaire à retenir

ACL : Liste de contrôle d’accès (règles de filtrage).
Stateful Inspection : Filtrage dynamique avec mémoire des connexions.

Proxy : Intermédiaire qui filtre les requêtes applicatives.
DoS : Attaque par déni de service (le stateful aide à s’en protéger).
