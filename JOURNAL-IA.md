Il verifie surtout que la requete peut etre executee et que la fonction retourne un `Flow<Double?>`, mais il ne verifie pas vraiment si le resultat est correct.

Si on ne met pas de produits avec des valeurs connues dans la base, le test suppose des donnees qui peuvent ne pas exister.

Pour que le test soit utile, il faut ajouter des produits avec des `stockKg` connus, recuperer le resultat du `Flow` et verifier que la somme obtenue est bien celle attendue.