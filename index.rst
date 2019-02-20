CARBONTRAIL_RCAI : 0xa41C700556D9167257F69DDf66260a3d604D94f5
https://etherscan.io/address/0xa41c700556d9167257f69ddf66260a3d604d94f5

//------VARIABLES---------

//info_concealed (String ASCII convertie en Hex) = 3 premieres lettres du nom du client - premiere lettre du nom du client - 4 dernières lettres du nom du client - 2 premiers chiffres du code postal du client - 4ème chiffre du code postal du client - 2 premières lettres de la ville du client
//client_full (String ASCII convertie en Hex) =  Identité du client au format PNCEE (NOM;PRENOM pour un particulier RAISON SOCIALE;SIRET pour un professionnel) encodée avec l'alogorithme MD5
//address_full (String ASCII convertie en Hex) = Adresse du client au format PNCEE (NUMERO DE VOIE NOM DE VOIE;CODE POSTAL; VILLE) encodée avec l'alogorithme MD5
//declared_for (String ASCII convertie en Hex) = Adresse de l'obligé dans la blockchain (e.g. MGNS. primary address = 0x62073c7c87c988f2Be0EAF41b5c0481df98e886E)

//status = Code parmi la liste suivante
//BACCARA : Test
//1: Client Non Conforme
//2: Droit Suppression GPDR Client 
//3: Erreur Saisie
//4: -
//5: Entrée en relation sans RCAI
//6: Mise à jour fiche
//7: RCAI Antérieur 
//8: Entrée en Relation Arbitrage sans RCAI
//9: RCAI Bloc Actuel 

//Exemple Entrée en relation de MGNS. avec lettre d'engagement envoyée par mail à M. Lucien Renard, 88 impasse du Colonel De Gaulle, 13001 MARSEILLE
//info_concealed : REN-L-ULLE-13-0-MA -> 0x52454E2D4C2D554C4C452D31332D302D4D410A
//client_full : MD5 ("RENARD;LUCIEN") = 7782b8d28bbc0afd1bfc6f84bcd1bceb -> 0x7782b8d28bbc0afd1bfc6f84bcd1bceb
//adress_full : MD5 ("88 IMPASSE DU COLONEL DE GAULLE;13001;MARSEILLE") = 40d3001c5cb5946d1d62b8b1363ec967 -> 0x40d3001c5cb5946d1d62b8b1363ec967
//declared_for :  0x62073c7c87c988f2Be0EAF41b5c0481df98e886E
//status : 9


CARBONTRAIL_OPESTA : 0x5623796B934164857D8a320eAD6E3B13f01c712e
https://etherscan.io/address/0x5623796b934164857d8a320ead6e3b13f01c712e

//------VARIABLES---------

//reference_interne (String ASCII convertie en Hex) = Référence dossier
//fiche (String ASCII convertie en Hex) = Référence fiche_opération_standardisée
//volumekWh(Integer) = Volume de CEE  en kWh CUMAC
//date_engagement(Integer) = Nombre de secondes entre le 1er Janvier 1970 et la date d'engagement de l'opération
//date_facture(Integer) = Nombre de secondes entre le 1er Janvier 1970 et la date de facture
//pro = (String ASCII convertie en Hex) =  Identité du pro au format PNCEE (RAISON SOCIALE;SIREN;ou RAISON SOCIALE;SIREN SOUS TRAITANT;RAISON SOCIALE;SIREN SOUS TRAITANT) encodée avec l'alogorithme MD5
//client_full (String ASCII convertie en Hex) =  Identité du client au format PNCEE (NOM;PRENOM pour un particulier RAISON SOCIALE;SIREN pour un professionnel) encodée avec l'alogorithme MD5
//address_full (String ASCII convertie en Hex) = Adresse de réalisation de l'opération au format PNCEE (NUMERO DE VOIE NOM DE VOIE;CODE POSTAL; VILLE) encodée avec l'alogorithme MD5
//declared_for (String ASCII convertie en Hex) = Adresse de l'obligé dans la blockchain (e.g. MGNS. primary address = 0x62073c7c87c988f2Be0EAF41b5c0481df98e886E)

//nature_bon = Code parmi la liste suivante
//BACCARA : Arbitrage
//1 : Contribution financière (monnaie fiducaire ou cryptomonnaie) 
//2 : Bon d'achat pour des produits de consommation courante
//3 : Prêt bonifié
//4 : Audit ou conseil
//5 : Produit ou service offert
//6 : Opération réalisée sur patrimoine propre


//status = Code parmi la liste suivante
//BACCARA : Test
//1: Annulation Non Conformité
//2: Annulation Droit Suppression GPDR Client 
//3: Annulation Erreur Saisie
//4: -
//5: Documents reçus 
//6: Validé interne
//7: Déposé PNCEE
//8: Arbitrage
//9: Validé PNCEE

//Exemple MGNS. s'engage le 16/01/2019 a poser gratuitement des mousseurs sur les 750 robinets de l'ECOLE DE CIRQUE PITRERIES 2 RUE DE STRASBOURG 83210 SOLLIES PONT SIRET 42493526000036. Posé et facturé par FRANCE MERGUEZ DISTRIBUTION SIRET 34493368400021 le 17/01/2019. ASH numéro MPE400099. Enregistrement dans la blockchain lors du dépot au PNCEE.
//client_full : MD5 ("ECOLE DE CIRQUE PITRERIES;42493526") = 95be74bce973b492a060a4a5e38fb916 -> 0x95be74bce973b492a060a4a5e38fb916
//adress_full : MD5 ("2 RUE DE STRASBOURG;83210;SOLLIES PONT") = c86f2d95804c4af2a1cbf85d64df29e0 -> 0xc86f2d95804c4af2a1cbf85d64df29e0
//pro : MD5 ("FRANCE MERGUEZ DISTRIBUTION;344933684") = 4cf60fe171f7487aedb1c0892f2614eb -> 0x4cf60fe171f7487aedb1c0892f2614eb
//declared_for :  0x62073c7c87c988f2Be0EAF41b5c0481df98e886E
//nature_bon : 5
//status : 7
//reference_interne : MPE400099 -> 0x4D50453430303039390A
//fiche : BAT-EQ-133 -> 0x4241542D45512D3133330A
//volumekWh : 2031750
//date_engagement : 1547659037
//date_facture : 1547745437
