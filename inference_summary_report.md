# Inference Summary Report

Single report covering all manuscripts in the inference set, partitioned into four non-overlapping categories. Each manuscript appears in exactly one section.

## Category overview

| Section | Category | Count | Notes |
|---|---|---:|---|
| 1 | Catalog agreement | 171 | Model prediction matches filename's claimed author |
| 2 | Catalog disagreement | 719 | Model predicts a different trained scribe than filename claims |
| 3 | Anonymous attribution | 552 | Filename is anonymous/uncertain; model proposed an attribution |
| 4 | Untrained-author filename | 1472 | Filename's author is not one of the 100 trained classes |
| | **Total** | **2914** | |

## Reading the tables

- **Tier**: confidence tier assigned by per-manuscript voting. `high` = >=80% pages agree AND mean margin >= 10. `medium` = >=50% agreement AND margin >= 3. `low` = neither.
- **Manuscript**: folder name in the inference dataset.
- **Cataloged**: filename's claimed author, resolved to the training class name via the alias map (sections 1 and 2 only).
- **Model says**: model's top-1 prediction across all pages.
- **Pages**: total page count.
- **Agreement**: pages that voted for the top-1 prediction over total pages.
- **Margin**: mean confidence gap between top-1 and runner-up across pages. Higher = more decisive per-page voting.
- **Top-5**: top 5 authors by vote count, with page count in parentheses.

Rows within each section are sorted by tier (high -> medium -> low), then by margin (highest first) within tier.

## 1. Catalog agreement

Manuscripts where the model's prediction matches the filename's catalog attribution (after alias normalization). These represent cases where the model's scribal-hand identification independently confirms the catalog's claim.

**171 manuscripts** (high: 77, medium: 68, low: 26)

| Tier | Manuscript | Cataloged | Model says | Pages | Agreement | Margin | Top-5 |
|---|---|---|---|---:|---:|---:|---|
| high | `LEONORCUEVA_Testamento_Autografo` | LEONORCUEVA | LEONORCUEVA | 16 | 16/16 (100%) | 100.70 | LEONORCUEVA (16) |
| high | `PACHECO_Comedias_Autografo` | PACHECO | PACHECO | 254 | 240/254 (94%) | 98.76 | PACHECO (240), LANINI (3), MULSA (2), AVELLANEDADELACUEVA (2), GONZALEZDETORRES (1) |
| high | `SANTATERESA_Fundaciones` | SANTATERESA | SANTATERESA | 278 | 262/278 (94%) | 76.52 | SANTATERESA (262), LEONORCUEVA (2), CERVANTES (1), GONZALEZDETORRES (1), VIDALYSALVADOR (1) |
| high | `SANTATERESA_Vida` | SANTATERESA | SANTATERESA | 455 | 414/455 (91%) | 65.57 | SANTATERESA (414), CERVANTES (2), AVELLANEDA (1), LEONORCUEVA (1), CECILIANACIMIENTO (1) |
| high | `ROJAS_AscensionCristo_Autografo` | LICENCIADOROJAS | LICENCIADOROJAS | 19 | 19/19 (100%) | 64.69 | LICENCIADOROJAS (19) |
| high | `LORENZANA_OrigenAparecimientoSenoraHoyo` | LORENZANA | LORENZANA | 42 | 42/42 (100%) | 64.24 | LORENZANA (42) |
| high | `ROJAS_HuidaAEgipto_Autografo` | LICENCIADOROJAS | LICENCIADOROJAS | 33 | 31/33 (94%) | 61.44 | LICENCIADOROJAS (31), LORENZANA (1) |
| high | `SANTATERESA_Caravaca` | SANTATERESA | SANTATERESA | 1 | 1/1 (100%) | 59.07 | SANTATERESA (1) |
| high | `ROJAS_PurificacionNuestraSenora_Autografo` | LICENCIADOROJAS | LICENCIADOROJAS | 24 | 24/24 (100%) | 57.00 | LICENCIADOROJAS (24) |
| high | `Belmonte_Casarsesinhablarse` | BELMONTE | BELMONTE | 58 | 48/58 (83%) | 55.41 | BELMONTE (48), GONZALEZDEBARCIA (1), HURTADODEMENDOZA (1) |
| high | `LopezJacinto_EnganoenlaverdadEl` | LOPEZJACINTO | LOPEZJACINTO | 69 | 60/69 (87%) | 55.05 | LOPEZJACINTO (60), GONZALEZDEBARCIA (1) |
| high | `CARVAJAL_BandoleraDeFlandes` | CARVAJAL | CARVAJAL | 63 | 62/63 (98%) | 50.76 | CARVAJAL (62), CERVANTES (1) |
| high | `LEONORCUEVA_Poesias_Autografo` | LEONORCUEVA | LEONORCUEVA | 42 | 42/42 (100%) | 45.32 | LEONORCUEVA (42) |
| high | `DELAHOZ_DescubrimientodelasBatuecas_Autografo` | HOZYMOTA | HOZYMOTA | 70 | 61/70 (87%) | 43.60 | HOZYMOTA (61), CARVAJAL (1), LICENCIADOROJAS (1), CONTRERAS (1), GONZALEZDEBARCIA (1) |
| high | `GILENRIQUEZ_ElPozo_Autografo` | GILENRIQUEZ | GILENRIQUEZ | 6 | 6/6 (100%) | 42.60 | GILENRIQUEZ (6) |
| high | `CAJESI_TrabajosdeJose` | CAXESI | CAXESI | 22 | 21/22 (96%) | 37.55 | CAXESI (21), HURTADODEMENDOZA (1) |
| high | `REMON_GrandezasDeMadrid_Autografo` | REMON | REMON | 98 | 80/98 (82%) | 36.28 | REMON (80), LICENCIADOROJAS (2), VALDIVIELSO (1), VIDALYSALVADOR (1), LOPE (1) |
| high | `GarciaMarcos_Enganarseensufavor` | GARCIAMARCOS | GARCIAMARCOS | 86 | 74/86 (86%) | 35.35 | GARCIAMARCOS (74), FAJARDOYACEVEDO (1) |
| high | `CANIZARES_ConMusica_acto2_Autografo` | CANIZARES | CANIZARES | 29 | 28/29 (97%) | 33.84 | CANIZARES (28), BOLEAYALVARADO (1) |
| high | `MORETO_AmorYObligacion_Autografo` | MORETO | MORETO | 67 | 58/67 (87%) | 33.21 | MORETO (58), DAVILAYPALOMARES (1), GONZALEZDEBARCIA (1) |
| high | `LANINI_DeseadoPrincipe_acto1y2_Autografo_-2` | LANINI | LANINI | 37 | 37/37 (100%) | 32.75 | LANINI (37) |
| high | `VELEZ_CatalanSerrallonga_acto3_Autografo` | VELEZ | VELEZ | 37 | 36/37 (97%) | 31.94 | VELEZ (36) |
| high | `LOPE_GalanMembrilla_Autografo` | LOPE | LOPE | 58 | 52/58 (90%) | 31.89 | LOPE (52), CERVANTES (3), REMON (1), CORDERO (1), HURTADODEMENDOZA (1) |
| high | `LOPE_SantiagoVerde_Autografo` | LOPE | LOPE | 39 | 35/39 (90%) | 31.83 | LOPE (35), CERVANTES (2), REMON (2) |
| high | `TIRSO_SantaJuanaPrimera_Autografo` | TIRSO | TIRSO | 90 | 84/90 (93%) | 31.55 | TIRSO (84), BATRES (1), ENRIQUEZ (1) |
| high | `LopezJacinto_MujerjuezdesumaridoLa` | LOPEZJACINTO | LOPEZJACINTO | 133 | 115/133 (86%) | 31.34 | LOPEZJACINTO (115), PAREDES (2), CASTILLOSOLORZANO (1) |
| high | `ZABALETA_HidalgaHermosura_acto1_Autografo` | ZABALETA | ZABALETA | 31 | 31/31 (100%) | 30.45 | ZABALETA (31) |
| high | `CONTRERAS_Poesia_Autografo` | CONTRERAS | CONTRERAS | 112 | 105/112 (94%) | 30.28 | CONTRERAS (105), LICENCIADOROJAS (1), MULSA (1), AMESCUA (1) |
| high | `BELMONTE_PrincipePerseguido_acto1_Autografo` | BELMONTE | BELMONTE | 36 | 36/36 (100%) | 29.93 | BELMONTE (36) |
| high | `LEONORCUEVA_Firmezaenelausencia_Autografo` | LEONORCUEVA | LEONORCUEVA | 105 | 104/105 (99%) | 29.66 | LEONORCUEVA (104), VARGASMACHUCA (1) |
| high | `CALDERON_ElAnoSantoRoma_Autografo` | CALDERON | CALDERON | 30 | 29/30 (97%) | 29.39 | CALDERON (29), FAJARDOYACEVEDO (1) |
| high | `MONTALBAN_PolifemoCirce_acto2_Autografo` | MONTALBAN | MONTALBAN | 34 | 33/34 (97%) | 29.32 | MONTALBAN (33) |
| high | `HOZ_DeseadoPrincipe_acto3_Autografo_-2` | HOZYMOTA | HOZYMOTA | 20 | 19/20 (95%) | 28.98 | HOZYMOTA (19), LANINI (1) |
| high | `LopezJacinto_NohayfuerzacontraelamorVictori` | LOPEZJACINTO | LOPEZJACINTO | 127 | 103/127 (81%) | 28.54 | LOPEZJACINTO (103), CONTRERAS (3), LOPEZDELCAMPO (2), LICENCIADOROJAS (1), VIDALYSALVADOR (1) |
| high | `CALDERON_ViaticoCordero_Autografo` | CALDERON | CALDERON | 27 | 23/27 (85%) | 28.42 | CALDERON (23), GILENRIQUEZ (4) |
| high | `VELEZ_CondePeroVelez_Autografo` | VELEZ | VELEZ | 116 | 107/116 (92%) | 28.03 | VELEZ (107), LOPE (3), VIDALYSALVADOR (1) |
| high | `CALDERON_ADios_Autografo` | CALDERON | CALDERON | 27 | 26/27 (96%) | 27.92 | CALDERON (26), SARAVIAYMENDOZA (1) |
| high | `LANINI_AllaVanLeyesDoQuierenReyes_Autografo` | LANINI | LANINI | 70 | 58/70 (83%) | 27.87 | LANINI (58), HURTADODEMENDOZA (1), SANDOVAL (1) |
| high | `DIAMANTE_VaqueroEmperador_acto2_Autografo` | DIAMANTE | DIAMANTE | 28 | 27/28 (96%) | 26.95 | DIAMANTE (27), QUINONES (1) |
| high | `BELMONTE_AmorDesafiado_Autografo` | BELMONTE | BELMONTE | 108 | 87/108 (81%) | 26.85 | BELMONTE (87), VIDALYSALVADOR (2), LOPEZDELCAMPO (1), PAREDES (1), GARCIAMARCOS (1) |
| high | `CALDERON_AguaMansa_Autografo` | CALDERON | CALDERON | 108 | 100/108 (93%) | 25.79 | CALDERON (100), GILENRIQUEZ (2), VIDALYSALVADOR (2), GARCIADEPRADO (1), AVELLANEDADELACUEVA (1) |
| high | `CALDERON_YerrosNaturaleza_acto2_Autografo` | CALDERON | CALDERON | 47 | 45/47 (96%) | 24.35 | CALDERON (45), MONTALBAN (1), QUINONES (1) |
| high | `BELMONTE_MejorAmigoMuerto_acto1_Autografo` | BELMONTE | BELMONTE | 30 | 30/30 (100%) | 24.27 | BELMONTE (30) |
| high | `VIDALYSALVADOR_AmorFirmezaYCorona_Autografo` | VIDALYSALVADOR | VIDALYSALVADOR | 156 | 149/156 (96%) | 24.06 | VIDALYSALVADOR (149) |
| high | `LOPE_DoncellaTeodor_Autografo` | LOPE | LOPE | 124 | 100/124 (81%) | 24.06 | LOPE (100), VIDALYSALVADOR (2), PAREDES (1), CONTRERAS (1), LEONORCUEVA (1) |
| high | `LOPE_HermosaEster_Autografo` | LOPE | LOPE | 55 | 50/55 (91%) | 23.99 | LOPE (50), CERVANTES (4), QUEVEDO (1) |
| high | `VARGAS_AUnTiempoReyYVasallo_acto1_Autografo` | VARGAS | VARGAS | 41 | 41/41 (100%) | 23.87 | VARGAS (41) |
| high | `MIRAAMESCUA_AdversaFortuna_Autografo` | AMESCUA | AMESCUA | 115 | 109/115 (95%) | 23.39 | AMESCUA (109), VARGASMACHUCA (1) |
| high | `CALDERON_MejorAmigoMuerto_acto3_Autografo` | CALDERON | CALDERON | 28 | 28/28 (100%) | 21.71 | CALDERON (28) |
| high | `GONZALEZDEBARCIA_SacodelagrancasadeMecaEl_Autografo` | GONZALEZDEBARCIA | GONZALEZDEBARCIA | 80 | 73/80 (91%) | 21.52 | GONZALEZDEBARCIA (73), VIDALYSALVADOR (3), CERVANTES (1), HURTADODEMENDOZA (1), CECILIANACIMIENTO (1) |
| high | `HozyMota_DisparatesJuanEncina_Autografo` | HOZYMOTA | HOZYMOTA | 119 | 105/119 (88%) | 21.35 | HOZYMOTA (105), VIDALYSALVADOR (2), VALDIVIELSO (1), VARGASMACHUCA (1), AMESCUA (1) |
| high | `LOPE_CarlosV_Autografo` | LOPE | LOPE | 119 | 102/119 (86%) | 21.26 | LOPE (102), VARGASMACHUCA (2), HURTADODEMENDOZA (1), VELEZ (1) |
| high | `HOZ_VivaImagen_acto2_Autografo` | HOZYMOTA | HOZYMOTA | 33 | 32/33 (97%) | 21.02 | HOZYMOTA (32), CANIZARES (1) |
| high | `CALDERON_CuraEnfermedad_Autografo` | CALDERON | CALDERON | 30 | 24/30 (80%) | 20.20 | CALDERON (24), BOLEAYALVARADO (2), GILENRIQUEZ (2), SARAVIAYMENDOZA (1), BELMONTE (1) |
| high | `LOPE_Encomienda_Autografo` | LOPE | LOPE | 125 | 100/125 (80%) | 18.11 | LOPE (100), CERVANTES (2), HURTADODEMENDOZA (2), CECILIANACIMIENTO (1), ENRIQUEZ (1) |
| high | `CALDERON_HidalgaHermosura_acto3_Autografo` | CALDERON | CALDERON | 37 | 35/37 (95%) | 18.11 | CALDERON (35), ZABALETA (1), LEONORCUEVA (1) |
| high | `CALDERON_MagicoProdigioso_Autografo` | CALDERON | CALDERON | 157 | 137/157 (87%) | 17.37 | CALDERON (137), QUINONES (2), MONTALBAN (1), CONTRERAS (1), BELMONTE (1) |
| high | `Calderon_MagicoprodigiosoEl` | CALDERON | CALDERON | 169 | 137/169 (81%) | 16.79 | CALDERON (137), VIDALYSALVADOR (3), QUINONES (2), AMESCUA (1), PAREDES (1) |
| high | `CALDERON_VacanteGeneral_Autografo` | CALDERON | CALDERON | 7 | 6/7 (86%) | 16.23 | CALDERON (6), MARCHANTE (1) |
| high | `MENESES_PrincipePerseguido_acto3_Autografo` | MENESES | MENESES | 36 | 33/36 (92%) | 15.96 | MENESES (33), LANINI (1), AVELLANEDA (1), COELLO (1) |
| high | `LOPE_DamaBoba_Autografo` | LOPE | LOPE | 119 | 108/119 (91%) | 15.77 | LOPE (108), CASTILLOSOLORZANO (1), CERVANTES (1), MULSA (1) |
| high | `Alarcon_MejorAmigoMuerto_acto2_Autografo` | ALARCON | ALARCON | 30 | 29/30 (97%) | 15.64 | ALARCON (29), CALDERON (1) |
| high | `LOPE_Barlaan_Autografo` | LOPE | LOPE | 53 | 47/53 (89%) | 15.41 | LOPE (47), VELEZ (2), QUEVEDO (1), SANDOVAL (1) |
| high | `GONZALEZDEBARCIA_DonQuijote_Autografo` | GONZALEZDEBARCIA | GONZALEZDEBARCIA | 22 | 22/22 (100%) | 15.14 | GONZALEZDEBARCIA (22) |
| high | `HERNANDEZPADILLA_cartapacio` | HERNANDEZPADILLA | HERNANDEZPADILLA | 278 | 259/278 (93%) | 15.13 | HERNANDEZPADILLA (259), SANTATERESA (5), AMESCUA (2), LEONORCUEVA (2), AGUADOELVIEJO (2) |
| high | `MIRAAMESCUA_MartirdeMadrid_acto1y3_Autografo` | AMESCUA | AMESCUA | 85 | 73/85 (86%) | 15.04 | AMESCUA (73), CASTILLOSOLORZANO (5), PAREDES (1), AVELLANEDA (1), CUEVAYSILVA (1) |
| high | `DIAMANTE_CruzDeCaravaca_Autografo` | DIAMANTE | DIAMANTE | 96 | 88/96 (92%) | 14.83 | DIAMANTE (88), VIDALYSALVADOR (3), BELMONTE (1), GARCIADEPRADO (1), HURTADODEMENDOZA (1) |
| high | `LOPE_MelindresBelisa_acto1` | LOPE | LOPE | 34 | 33/34 (97%) | 14.55 | LOPE (33), REMON (1) |
| high | `LOPE_SembrarEnBuena_Autografo` | LOPE | LOPE | 56 | 53/56 (95%) | 14.50 | LOPE (53), REMON (2) |
| high | `CALDERON_DevocionMisa_Autografo` | CALDERON | CALDERON | 27 | 22/27 (82%) | 14.34 | CALDERON (22), GILENRIQUEZ (3), MARCHANTE (1), BOLEAYALVARADO (1) |
| high | `LANINI_AfricanoNeron_acto2y3_Autografo` | LANINI | LANINI | 54 | 50/54 (93%) | 14.01 | LANINI (50), AVELLANEDA (3), VIDALYSALVADOR (1) |
| high | `COELLO_YerrosNaturaleza_acto3_Autografo` | COELLO | COELLO | 25 | 24/25 (96%) | 13.21 | COELLO (24), CALDERON (1) |
| high | `CALDERON_LirioAzucena_Autografo` | CALDERON | CALDERON | 29 | 25/29 (86%) | 13.18 | CALDERON (25), GILENRIQUEZ (3), VILLEGASJUANBAUTISTA (1) |
| high | `GONGORA_Soneto_Autografo` | GONGORA | GONGORA | 2 | 2/2 (100%) | 12.90 | GONGORA (2) |
| high | `CALDERON_PrimerRefugio_Autografo` | CALDERON | CALDERON | 54 | 46/54 (85%) | 12.60 | CALDERON (46), GILENRIQUEZ (2), BANCESCANDAMO (1), VILLEGASJUANBAUTISTA (1), SARAVIAYMENDOZA (1) |
| high | `CALDERON_GranPrincipeFez_Autografo` | CALDERON | CALDERON | 186 | 166/186 (89%) | 10.74 | CALDERON (166), MONTALBAN (10), QUINONES (3), VIDALYSALVADOR (2), VARGASMACHUCA (1) |
| high | `LOPE_AmorPleitoYDesafio_Autografo` | LOPE | LOPE | 124 | 100/124 (81%) | 10.51 | LOPE (100), VIDALYSALVADOR (2), VELEZ (2), CONTRERAS (1), HURTADODEMENDOZA (1) |
| medium | `TorresLorenzode_ConversiondelaMagdalenaLa` | TORRESLORENZODE | TORRESLORENZODE | 28 | 19/28 (68%) | 55.18 | TORRESLORENZODE (19), PAREDES (1) |
| medium | `SANDOVAL_AlcaldeCasado_Autografo` | SANDOVAL | SANDOVAL | 12 | 8/12 (67%) | 48.89 | SANDOVAL (8), GONZALEZDEBARCIA (1) |
| medium | `VALDIVIESO_ProbanzasEHidalguiaDelHombre_Autografo` | VALDIVIELSO | VALDIVIELSO | 36 | 23/36 (64%) | 47.68 | VALDIVIELSO (23), CONTRERAS (1) |
| medium | `SANTATERESA_ModoVisitar` | SANTATERESA | SANTATERESA | 79 | 45/79 (57%) | 30.91 | SANTATERESA (45), LORENZANA (2), LANINI (1), CUENCAYARGUELLO (1), CASTILLOSOLORZANO (1) |
| medium | `LOPEZDECARDENA_LoaParaAumentarLaDevocion_Autografo` | LOPEZDECARDENA | LOPEZDECARDENA | 16 | 8/16 (50%) | 29.93 | LOPEZDECARDENA (8), VIDALYSALVADOR (3), PAREDES (1), DIAMANTE (1) |
| medium | `VELEZ_AguilaDelAguaYBatallaNaval_Autografo` | VELEZ | VELEZ | 139 | 107/139 (77%) | 29.16 | VELEZ (107), DIAMANTE (2), CASTILLOSOLORZANO (1), CARVAJAL (1), VIDALYSALVADOR (1) |
| medium | `CALDERON_DivinoCazador_Autografo` | CALDERON | CALDERON | 63 | 42/63 (67%) | 26.70 | CALDERON (42) |
| medium | `CALDERON_SecretoAVoces_Autografo` | CALDERON | CALDERON | 145 | 104/145 (72%) | 24.67 | CALDERON (104), CONTRERAS (7), VIDALYSALVADOR (3), GARCIADEPRADO (3), CASTILLOSOLORZANO (2) |
| medium | `TIRSO_SantaJuanaTercera_Autografo` | TIRSO | TIRSO | 129 | 96/129 (74%) | 23.12 | TIRSO (96), VIDALYSALVADOR (4), MARCHANTE (2), MESA (2), AMESCUA (2) |
| medium | `LOPE_PruebaAmigos_Autografo` | LOPE | LOPE | 145 | 107/145 (74%) | 22.91 | LOPE (107), VIDALYSALVADOR (3), BELMONTE (1), GARCIADEPRADO (1), BATRES (1) |
| medium | `CALDERON_VidaVerdadMentira_Autografo` | CALDERON | CALDERON | 161 | 127/161 (79%) | 22.40 | CALDERON (127), VILLEGASJUANBAUTISTA (2), CERVANTES (1), LOPE (1), HURTADODEMENDOZA (1) |
| medium | `LOPE_BatallaHonor_Autografo` | LOPE | LOPE | 129 | 97/129 (75%) | 22.14 | LOPE (97), LICENCIADOROJAS (2), HURTADODEMENDOZA (2), SANTATERESA (1), VIDALYSALVADOR (1) |
| medium | `BELMONTE_SastredelCampillo_Autografo` | BELMONTE | BELMONTE | 171 | 136/171 (80%) | 21.33 | BELMONTE (136), GARCIADEPRADO (2), VARGASMACHUCA (2), CASTILLOSOLORZANO (1), BENAVIDES (1) |
| medium | `LOPE_ObrasSonAmores_Autografo` | LOPE | LOPE | 47 | 35/47 (74%) | 21.26 | LOPE (35), QUEVEDO (1), LEIVARAMIREZ (1), ROJASZORRILLA (1), AMESCUA (1) |
| medium | `LOPE_CoronaMerecida_Autografo` | LOPE | LOPE | 131 | 99/131 (76%) | 20.93 | LOPE (99), QUINONES (2), HOZYMOTA (1), CALDERON (1), HURTADODEMENDOZA (1) |
| medium | `LOPE_Bastardo_Mudarra_Autografo` | LOPE | LOPE | 146 | 98/146 (67%) | 20.91 | LOPE (98), VIDALYSALVADOR (4), HURTADODEMENDOZA (3), REMON (2), DAVILAYPALOMARES (1) |
| medium | `LOPE_DiscordiaCasados_Autografo` | LOPE | LOPE | 141 | 102/141 (72%) | 19.74 | LOPE (102), VIDALYSALVADOR (7), ROJASZORRILLA (1), CASTILLOSOLORZANO (1), MONTALBAN (1) |
| medium | `QUEVEDO_carta_coronaArago` | QUEVEDO | QUEVEDO | 2 | 1/2 (50%) | 19.43 | QUEVEDO (1), ENRIQUEZ (1) |
| medium | `LOPE_PedroCarbonero_Autografo` | LOPE | LOPE | 141 | 101/141 (72%) | 19.03 | LOPE (101), HURTADODEMENDOZA (2), AMESCUA (2), QUINONES (1), CASTILLOSOLORZANO (1) |
| medium | `LOPE_Estefania_Autografo` | LOPE | LOPE | 148 | 102/148 (69%) | 18.95 | LOPE (102), VIDALYSALVADOR (4), VALDIVIELSO (2), VARGASMACHUCA (2), HURTADODEMENDOZA (2) |
| medium | `LOPE_DesdenVengado_Autografo` | LOPE | LOPE | 143 | 102/143 (71%) | 17.85 | LOPE (102), VIDALYSALVADOR (5), BELMONTE (2), MEDINA (1), CASTILLOSOLORZANO (1) |
| medium | `CALDERON_LlamadosyEscogidos_Autografo` | CALDERON | CALDERON | 73 | 50/73 (68%) | 17.07 | CALDERON (50), MONTALBAN (4), SARAVIAYMENDOZA (1), QUINONES (1), VIDALYSALVADOR (1) |
| medium | `MIRAAMESCUA_NoHayDicha_Autografo` | AMESCUA | AMESCUA | 141 | 82/141 (58%) | 16.55 | AMESCUA (82), GARCIADEPRADO (8), ALARCON (7), VIDALYSALVADOR (4), CASTILLOSOLORZANO (4) |
| medium | `LOPE_PrincipeDespenado_Autografo` | LOPE | LOPE | 142 | 96/142 (68%) | 16.45 | LOPE (96), VIDALYSALVADOR (3), QUEVEDO (2), TORRESLORENZODE (1), BARRIONUEVO (1) |
| medium | `MIRAAMESCUA_CasaTahur_Autografo` | AMESCUA | AMESCUA | 161 | 85/161 (53%) | 16.07 | AMESCUA (85), CASTILLOSOLORZANO (28), VIDALYSALVADOR (6), VELEZ (5), BELMONTE (3) |
| medium | `Montalban_Comopadreycomorey_Autografo` | MONTALBAN | MONTALBAN | 147 | 95/147 (65%) | 15.84 | MONTALBAN (95), QUINONES (3), CASTILLOSOLORZANO (2), CONTRERAS (2), GONZALEZDEBARCIA (2) |
| medium | `CALDERON_DesdichaVoz_Autografo` | CALDERON | CALDERON | 149 | 117/149 (78%) | 15.10 | CALDERON (117), QUINONES (5), VIDALYSALVADOR (3), CONTRERAS (3), VALDIVIELSO (1) |
| medium | `LANINI_AngelDeLasEscuelas_Autografo` | LANINI | LANINI | 142 | 107/142 (75%) | 14.40 | LANINI (107), AVELLANEDA (5), LICENCIADOROJAS (4), GONZALEZDEBARCIA (1), CERVANTES (1) |
| medium | `CALDERON_HumildadCoronada_Autografo` | CALDERON | CALDERON | 79 | 54/79 (68%) | 13.64 | CALDERON (54), GARCIADEPRADO (8), ENRIQUEZ (5), VALDIVIELSO (5), QUINONES (3) |
| medium | `CALDERON_PintorDeshonra_Autografo` | CALDERON | CALDERON | 27 | 21/27 (78%) | 13.23 | CALDERON (21), GILENRIQUEZ (2), VILLEGASJUANBAUTISTA (2), CASTROYSALAZAR (1), SARAVIAYMENDOZA (1) |
| medium | `CALDERON_PsiquisYCupido_Autografo` | CALDERON | CALDERON | 29 | 19/29 (66%) | 12.71 | CALDERON (19), VILLEGASJUANBAUTISTA (5), GILENRIQUEZ (2), MARCHANTE (1), LOPEZDELCAMPO (1) |
| medium | `CALDERON_LaberintoMundo_Autografo` | CALDERON | CALDERON | 30 | 17/30 (57%) | 12.48 | CALDERON (17), MARCHANTE (7), VILLEGASJUANBAUTISTA (3), GILENRIQUEZ (3) |
| medium | `CALDERON_SacroPernaso_Autografo` | CALDERON | CALDERON | 28 | 19/28 (68%) | 12.05 | CALDERON (19), GILENRIQUEZ (7), SARAVIAYMENDOZA (1), VILLEGASJUANBAUTISTA (1) |
| medium | `CALDERON_TroyaAbrasada_Autografo` | CALDERON | CALDERON | 161 | 84/161 (52%) | 11.46 | CALDERON (84), CORDERO (10), ALARCON (8), VIDALYSALVADOR (5), LEIVARAMIREZ (5) |
| medium | `CANIZARES_VivaImagen_acto1y3_Autografo` | CANIZARES | CANIZARES | 78 | 54/78 (69%) | 11.05 | CANIZARES (54), HOZYMOTA (21), VIDALYSALVADOR (2), DIAMANTE (1) |
| medium | `CALDERON_DiabloMudo_Autografo` | CALDERON | CALDERON | 26 | 18/26 (69%) | 10.54 | CALDERON (18), GILENRIQUEZ (6), MONTALBAN (1) |
| medium | `LOPE_CastigoSinVenganza_Autografo` | LOPE | LOPE | 140 | 100/140 (71%) | 9.95 | LOPE (100), VARGASMACHUCA (2), CECILIANACIMIENTO (1), REMON (1), CONTRERAS (1) |
| medium | `CASTILLOSOLORZANO_PruebadelosmedicosLa` | CASTILLOSOLORZANO | CASTILLOSOLORZANO | 17 | 16/17 (94%) | 9.79 | CASTILLOSOLORZANO (16), CERVANTES (1) |
| medium | `CALDERON_ValleDeLaZarzuela1` | CALDERON | CALDERON | 29 | 20/29 (69%) | 9.32 | CALDERON (20), GILENRIQUEZ (6), VIDALYSALVADOR (1), LOPEZDELCAMPO (1), VILLEGASJUANBAUTISTA (1) |
| medium | `LOPE_PoderDiscreto_Autografo` | LOPE | LOPE | 139 | 100/139 (72%) | 9.14 | LOPE (100), CASTILLOSOLORZANO (1), GARCIADEPRADO (1), VELEZ (1), PSEUDOHURTADODEMENDOZA (1) |
| medium | `BELMONTE_MartirdeMadrid_acto2_Autografo` | BELMONTE | BELMONTE | 34 | 32/34 (94%) | 9.01 | BELMONTE (32), CALDERON (1), LOPEZDECARDENA (1) |
| medium | `CALDERON_EspigasDeRuth_Autografo` | CALDERON | CALDERON | 28 | 16/28 (57%) | 8.95 | CALDERON (16), VILLEGASJUANBAUTISTA (6), SARAVIAYMENDOZA (2), GILENRIQUEZ (2), VIDALYSALVADOR (1) |
| medium | `CALDERON_CualEsMayorPerfeccionHermosuraODiscrecion` | CALDERON | CALDERON | 77 | 44/77 (57%) | 8.89 | CALDERON (44), LEIVARAMIREZ (6), BATRES (5), QUINONES (2), MORETO (2) |
| medium | `LOPE_NuevaVictoria_Autografo` | LOPE | LOPE | 149 | 91/149 (61%) | 8.80 | LOPE (91), AMESCUA (4), QUINONES (2), QUEVEDO (2), DIAMANTE (1) |
| medium | `CALDERON_SelvaConfusa_Autografo` | CALDERON | CALDERON | 137 | 90/137 (66%) | 8.45 | CALDERON (90), QUINONES (13), MESA (4), MONTALBAN (3), COELLO (3) |
| medium | `LOPE_FavorAgradecido_Autografo` | LOPE | LOPE | 40 | 33/40 (82%) | 8.44 | LOPE (33), HURTADODEMENDOZA (1), MIRACLESSOTOMAYOR (1), ENRIQUEZ (1) |
| medium | `LOPE_LoQuePasa_Autografo` | LOPE | LOPE | 167 | 91/167 (55%) | 8.06 | LOPE (91), VELEZ (11), VIDALYSALVADOR (7), MARCHANTE (3), VALDIVIELSO (1) |
| medium | `LOPE_MarquesDeLasNavas_Autografo` | LOPE | LOPE | 111 | 95/111 (86%) | 7.72 | LOPE (95), MIRACLESSOTOMAYOR (3), TAMAYO (2), ANDOSILLA (1), AGUADOELVIEJO (1) |
| medium | `LOPE_PrimeroBenavides_Autografo` | LOPE | LOPE | 112 | 63/112 (56%) | 7.67 | LOPE (63), MIRACLESSOTOMAYOR (40), SARAVIAYMENDOZA (2), AGUADOELVIEJO (1), SAAVEDRAFAJARDO (1) |
| medium | `CALDERON_DivinoOrfeo_Autografo` | CALDERON | CALDERON | 22 | 13/22 (59%) | 7.66 | CALDERON (13), SARAVIAYMENDOZA (5), GILENRIQUEZ (2), VILLEGASJUANBAUTISTA (1), BANCESCANDAMO (1) |
| medium | `CALDERON_HidalgaValle_Autografo` | CALDERON | CALDERON | 21 | 13/21 (62%) | 7.63 | CALDERON (13), GILENRIQUEZ (6), BOLEAYALVARADO (1), VILLEGASJUANBAUTISTA (1) |
| medium | `CASTILLOSOLORZANO_BarbadorEl` | CASTILLOSOLORZANO | CASTILLOSOLORZANO | 14 | 13/14 (93%) | 7.54 | CASTILLOSOLORZANO (13), CERVANTES (1) |
| medium | `LOPE_HazanasSegundoDavid_Autografo` | LOPE | LOPE | 21 | 16/21 (76%) | 7.39 | LOPE (16), CAXESI (4), HURTADODEMENDOZA (1) |
| medium | `LOPE_NinezRojas_Autografo` | LOPE | LOPE | 135 | 90/135 (67%) | 7.35 | LOPE (90), VALDIVIELSO (8), LOPEZDECARDENA (3), BATRES (3), CASTILLOSOLORZANO (2) |
| medium | `LOPE_CoronaDeHungria_Autografo` | LOPE | LOPE | 57 | 41/57 (72%) | 7.22 | LOPE (41), QUEVEDO (9), CERVANTES (6) |
| medium | `LOPE_SinSecreto_Autografo` | LOPE | LOPE | 61 | 33/61 (54%) | 6.74 | LOPE (33), QUEVEDO (15), CERVANTES (7), REMON (2) |
| medium | `LOPE_AmorConVista_Autografo` | LOPE | LOPE | 145 | 88/145 (61%) | 5.99 | LOPE (88), BATRES (9), VIDALYSALVADOR (2), VARGASMACHUCA (2), PSEUDOHURTADODEMENDOZA (2) |
| medium | `LOPE_PiadosoAragones_Autografo` | LOPE | LOPE | 147 | 96/147 (65%) | 5.52 | LOPE (96), VIDALYSALVADOR (7), BATRES (2), VELEZ (2), VALDIVIELSO (1) |
| medium | `LOPE_BrasilRestituido_Autografo` | LOPE | LOPE | 53 | 38/53 (72%) | 5.39 | LOPE (38), QUEVEDO (7), CERVANTES (4), VELEZ (1), REMON (1) |
| medium | `LOPE_AyVerdades_Autografo` | LOPE | LOPE | 59 | 38/59 (64%) | 5.16 | LOPE (38), QUEVEDO (13), CERVANTES (5), REMON (1), BANCESCANDAMO (1) |
| medium | `LOPE_DelMonteSale_Autografo` | LOPE | LOPE | 157 | 95/157 (60%) | 5.09 | LOPE (95), VIDALYSALVADOR (6), BELMONTE (3), MIRACLESSOTOMAYOR (1), CASTILLOSOLORZANO (1) |
| medium | `CERVANTES_autografofalso` | CERVANTES | CERVANTES | 1 | 1/1 (100%) | 4.97 | CERVANTES (1) |
| medium | `VIDALYSALVADOR_PacesDeIngenioYBelleza` | VIDALYSALVADOR | VIDALYSALVADOR | 186 | 175/186 (94%) | 4.56 | VIDALYSALVADOR (175), VARGASMACHUCA (5) |
| medium | `GONGORA_Carta3_Autografo` | GONGORA | GONGORA | 1 | 1/1 (100%) | 4.42 | GONGORA (1) |
| medium | `CERVANTES_Carta_Autografo` | CERVANTES | CERVANTES | 1 | 1/1 (100%) | 4.10 | CERVANTES (1) |
| medium | `CALDERON_AnoSantoRAH_Autografo` | CALDERON | CALDERON | 54 | 31/54 (57%) | 4.09 | CALDERON (31), CARVAJAL (13), GONGORA (8), REMON (1), ROMEROROQUE (1) |
| medium | `VIDALYSALVADOR_FuegoDeLasRiquezasYDestruccionDeSagunto` | VIDALYSALVADOR | VIDALYSALVADOR | 124 | 85/124 (68%) | 3.78 | VIDALYSALVADOR (85), QUEVEDO (20), BELMONTE (7), VARGASMACHUCA (2), GONGORA (1) |
| medium | `HOZYMOTA_Castigodelamiseria_Autografo` | HOZYMOTA | HOZYMOTA | 1 | 1/1 (100%) | 3.24 | HOZYMOTA (1) |
| low | `CALDERON_ProtestacionFe_Autografo` | CALDERON | CALDERON | 129 | 53/129 (41%) | 14.43 | CALDERON (53), VIDALYSALVADOR (15), AVELLANEDA (12), VERATASSIS (10), VARGASMACHUCA (4) |
| low | `LOPE_DeCuandoAca_Autografo` | LOPE | LOPE | 143 | 67/143 (47%) | 12.48 | LOPE (67), MESA (39), VIDALYSALVADOR (5), QUEVEDO (1), QUINONES (1) |
| low | `MIRAAMESCUA_BELMONTE_MartirdeMadrid.pdf` | AMESCUA | AMESCUA | 157 | 76/157 (48%) | 12.14 | AMESCUA (76), BELMONTE (32), CASTILLOSOLORZANO (9), CUEVAYSILVA (2), VIDALYSALVADOR (2) |
| low | `Calderon_MayormonstruoloscelosEl` | CALDERON | CALDERON | 161 | 45/161 (28%) | 8.68 | CALDERON (45), LEIVARAMIREZ (41), QUINONES (30), BATRES (16), VIDALYSALVADOR (7) |
| low | `ZORRILLA_HidalgaHermosura_acto2_Autografo` | ROJASZORRILLA | ROJASZORRILLA | 46 | 22/46 (48%) | 8.57 | ROJASZORRILLA (22), ZABALETA (8), GILENRIQUEZ (7), CARVAJAL (6), LOPEZDELCAMPO (2) |
| low | `CALDERON_TriunfarMuriendo_Autografo` | CALDERON | CALDERON | 27 | 13/27 (48%) | 8.45 | CALDERON (13), GILENRIQUEZ (10), MARCHANTE (3), VILLEGASJUANBAUTISTA (1) |
| low | `ROJASZORRILLA_NuestraSenoradeAtocha_Autografo` | ROJASZORRILLA | ROJASZORRILLA | 159 | 51/159 (32%) | 8.42 | ROJASZORRILLA (51), QUINONES (46), MONTALBAN (19), LEIVARAMIREZ (14), MORETO (4) |
| low | `Calderon_DosamantesdelcieloLos` | CALDERON | CALDERON | 73 | 35/73 (48%) | 7.40 | CALDERON (35), BELMONTE (10), ROJASZORRILLA (4), MESA (3), PAREDES (2) |
| low | `LOPE_CaballeroDelSacramento_Autografo` | LOPE | LOPE | 121 | 59/121 (49%) | 7.28 | LOPE (59), REMON (41), CERVANTES (3), LEONORCUEVA (2), CASTILLOSOLORZANO (1) |
| low | `CALDERON_InmunidadSagrado_Autografo` | CALDERON | CALDERON | 24 | 8/24 (33%) | 5.52 | CALDERON (8), MARCHANTE (7), GILENRIQUEZ (3), SARAVIAYMENDOZA (3), CASTROYSALAZAR (2) |
| low | `CALDERON_LoaAnoSantoRAH_Autografo` | CALDERON | CALDERON | 10 | 4/10 (40%) | 4.05 | CALDERON (4), GONGORA (3), GARCIADEPRADO (1), CARVAJAL (1) |
| low | `LOPE_QuienMas_Autografo` | LOPE | LOPE | 153 | 59/153 (39%) | 4.00 | LOPE (59), QUEVEDO (35), REMON (10), BELMONTE (4), LORENZANA (2) |
| low | `Calderon_Peorestaqueestaba` | CALDERON | CALDERON | 69 | 31/69 (45%) | 3.55 | CALDERON (31), QUINONES (12), ROJASZORRILLA (8), BATRES (4), LEIVARAMIREZ (2) |
| low | `CLARAMONTE_PacienciaFortuna` | CLARAMONTE | CLARAMONTE | 55 | 15/55 (27%) | 3.49 | CLARAMONTE (15), LORENZANA (13), PACHECO (10), LICENCIADOROJAS (7), JUANDESOTO (5) |
| low | `CALDERON_NoHayMasFortuna_Autografo` | CALDERON | CALDERON | 53 | 26/53 (49%) | 3.32 | CALDERON (26), GONGORA (14), GILENRIQUEZ (6), REMON (3), CARVAJAL (2) |
| low | `LOPE_MelindresBelisa_Autografo` | LOPE | LOPE | 36 | 25/36 (69%) | 2.80 | LOPE (25), GALLEGOS (6), CLARAMONTE (2), GONZALEZDEBARCIA (1), HURTADODEMENDOZA (1) |
| low | `CERVANTES_expedientesolicitudlicencia` | CERVANTES | CERVANTES | 2 | 2/2 (100%) | 2.09 | CERVANTES (2) |
| low | `LOPE_ArcaDeNoeOMundoAlReves` | LOPE | LOPE | 124 | 27/124 (22%) | 1.35 | LOPE (27), BATRES (19), CALDERON (12), AMESCUA (11), ROJASZORRILLA (8) |
| low | `LOPE_Truhandelcielo_Parma` | LOPE | LOPE | 55 | 32/55 (58%) | 1.32 | LOPE (32), MESA (6), QUINONES (4), CARVAJAL (4), GARCIADEPRADO (3) |
| low | `ENRIQUEZ_CardenalDonGilDeAlbornoz` | ENRIQUEZ | ENRIQUEZ | 96 | 59/96 (62%) | 1.09 | ENRIQUEZ (59), VIDALYSALVADOR (23), PAREDES (4), GARCIADEPRADO (3), LEIVARAMIREZ (2) |
| low | `GARCES_Loajuegopelota_Autografo` | GARCIADEPRADO | GARCIADEPRADO | 14 | 3/14 (21%) | 1.03 | GARCIADEPRADO (3), CALDERON (3), HURTADODEMENDOZA (2), QUINONES (2), AMESCUA (1) |
| low | `CANIZARES_LoQueValeElSerDevoto_British` | CANIZARES | CANIZARES | 134 | 33/134 (25%) | 0.75 | CANIZARES (33), FAJARDOYACEVEDO (21), CALLE (14), BATRES (14), GARCIADEPRADO (13) |
| low | `ENRIQUEZ_FernaMendezPintoEnLaChina` | ENRIQUEZ | ENRIQUEZ | 131 | 42/131 (32%) | 0.67 | ENRIQUEZ (42), BELMONTE (22), BATRES (16), LEIVARAMIREZ (12), VIDALYSALVADOR (6) |
| low | `ENRIQUEZ_JerusalenConquistada` | ENRIQUEZ | ENRIQUEZ | 48 | 28/48 (58%) | 0.54 | ENRIQUEZ (28), SANDOVAL (8), LEIVARAMIREZ (3), BELMONTE (2), BATRES (2) |
| low | `CERVANTES_autografo` | CERVANTES | CERVANTES | 2 | 1/2 (50%) | 0.43 | CERVANTES (1), AMESCUA (1) |
| low | `MONTALBAN_LindonaDeGalicia` | MONTALBAN | MONTALBAN | 122 | 47/122 (38%) | 0.33 | MONTALBAN (47), QUEVEDO (16), BATRES (13), LEIVARAMIREZ (8), VIDALYSALVADOR (8) |

## 2. Catalog disagreement

Manuscripts where the filename names a known trained author but the model predicts a different trained scribe. Per the methodology note, disagreement is not necessarily error.

**719 manuscripts** (high: 41, medium: 209, low: 469)

| Tier | Manuscript | Cataloged | Model says | Pages | Agreement | Margin | Top-5 |
|---|---|---|---|---:|---:|---:|---|
| high | `CALDERON_HadoyDivisaBnF_2` | CALDERON | GONZALEZDETORRES | 162 | 159/162 (98%) | 39.85 | GONZALEZDETORRES (159), LANINI (1), MELO (1), VARGASMACHUCA (1) |
| high | `Calderon_Pleitomatrimonialdelcuerpoyela` | CALDERON | VIDALYSALVADOR | 42 | 36/42 (86%) | 32.97 | VIDALYSALVADOR (36), MELO (1), CARVAJAL (1) |
| high | `ROJASZORRILLA_Atribuido_FOLCHDECARDONA_LoMejorEsLoMejorOMejorCercoDeRoma` | ROJASZORRILLA | CASTROYSALAZAR | 57 | 50/57 (88%) | 27.67 | CASTROYSALAZAR (50), ROMEROROQUE (3), CERVANTES (1), HURTADODEMENDOZA (1) |
| high | `LOPE_AlcaldeZalamea_Parma` | LOPE | AVELLANEDA | 42 | 39/42 (93%) | 27.52 | AVELLANEDA (39), CERVANTES (1), LEONORCUEVA (1) |
| high | `CALDERON_VinadelsenorLa_Hisp` | CALDERON | GARCIADEPRADO | 43 | 39/43 (91%) | 27.25 | GARCIADEPRADO (39), CALDERON (2), CONTRERAS (1) |
| high | `CALDERON_AMariaElCorazon` | CALDERON | MOLINAYMENDOZA | 22 | 20/22 (91%) | 25.23 | MOLINAYMENDOZA (20), GONZALEZDEBARCIA (1), TORRESLORENZODE (1) |
| high | `CALDERON_PsiquisYCupido` | CALDERON | GILENRIQUEZ | 45 | 40/45 (89%) | 24.66 | GILENRIQUEZ (40), CERVANTES (1), VARGASMACHUCA (1), LANINI (1) |
| high | `HURTADOMENDOZA_Cadalococonsutema_Autografo` | HURTADODEMENDOZA | PSEUDOHURTADODEMENDOZA | 129 | 104/129 (81%) | 21.22 | PSEUDOHURTADODEMENDOZA (104), LICENCIADOROJAS (3), DIAMANTE (3), CASTILLOSOLORZANO (1), GOMEZACOSTA (1) |
| high | `VALDIVIESO_AlabanzaDelTrabajo` | VALDIVIELSO | LORENZANA | 2 | 2/2 (100%) | 18.97 | LORENZANA (2) |
| high | `Calderon_autos_Novenatomo5` | CALDERON | CASTROYSALAZAR | 300 | 261/300 (87%) | 18.96 | CASTROYSALAZAR (261), VIDALYSALVADOR (12), MELO (8), CANIZARES (7), ROMEROROQUE (3) |
| high | `MORETO_TravesurasSonValor` | MORETO | CASTROYSALAZAR | 102 | 98/102 (96%) | 18.89 | CASTROYSALAZAR (98), PAREDES (2), VIDALYSALVADOR (1) |
| high | `CALDERON_InmunidadDelSagrado` | CALDERON | MOLINAYMENDOZA | 24 | 23/24 (96%) | 18.69 | MOLINAYMENDOZA (23), ROMEROROQUE (1) |
| high | `CALDERON_AlimentosDelHombre2` | CALDERON | MOLINAYMENDOZA | 31 | 25/31 (81%) | 18.44 | MOLINAYMENDOZA (25), CASTROYSALAZAR (3), TORRESLORENZODE (2), ROMEROROQUE (1) |
| high | `CALDERON_AlimentosDelHombre` | CALDERON | GONZALEZDEBARCIA | 43 | 42/43 (98%) | 17.82 | GONZALEZDEBARCIA (42), BANCESCANDAMO (1) |
| high | `CALDERON_VerdaderoDiosPan` | CALDERON | GONZALEZDEBARCIA | 40 | 39/40 (98%) | 17.53 | GONZALEZDEBARCIA (39), LANINI (1) |
| high | `CALDERON_DivinoOrfeo` | CALDERON | GONZALEZDEBARCIA | 30 | 30/30 (100%) | 17.24 | GONZALEZDEBARCIA (30) |
| high | `LOPE_TrabajosdejacobBritish` | LOPE | CANIZARES | 39 | 34/39 (87%) | 16.82 | CANIZARES (34), GILENRIQUEZ (2), LEONORCUEVA (1), DIAMANTE (1), CASTROYSALAZAR (1) |
| high | `LOPE_FortunamerecidaLa_British` | LOPE | CANIZARES | 46 | 41/46 (89%) | 16.39 | CANIZARES (41), MORETO (3), GILENRIQUEZ (1), LEIVARAMIREZ (1) |
| high | `LOPE_EspanolesenFlandesBritish` | LOPE | CANIZARES | 50 | 41/50 (82%) | 15.71 | CANIZARES (41), CASTROYSALAZAR (6), GONZALEZDETORRES (2), LANINI (1) |
| high | `ROJAS_PrudenciaEnElCastigo` | LICENCIADOROJAS | AVELLANEDA | 52 | 44/52 (85%) | 15.46 | AVELLANEDA (44), AMESCUA (1), CALDERON (1), DIAMANTE (1), VIDALYSALVADOR (1) |
| high | `GONZALEZDEBARCIA_Mayorefectohayquecelos` | GONZALEZDEBARCIA | VIDALYSALVADOR | 155 | 132/155 (85%) | 15.17 | VIDALYSALVADOR (132), ENRIQUEZ (15), GILENRIQUEZ (2), CASTILLOSOLORZANO (1), AMESCUA (1) |
| high | `Calderon_Mujerllorayvenceras` | CALDERON | GARCIAMARCOS | 86 | 72/86 (84%) | 14.56 | GARCIAMARCOS (72), GONZALEZDEBARCIA (1), AVELLANEDA (1), SANDOVAL (1), LEIVARAMIREZ (1) |
| high | `QUINONES_Alforjas` | QUINONES | REMON | 11 | 11/11 (100%) | 14.33 | REMON (11) |
| high | `CALDERON_ValleZarzuela` | CALDERON | VIDALYSALVADOR | 104 | 100/104 (96%) | 13.94 | VIDALYSALVADOR (100), CORDERO (1) |
| high | `CALDERON_ConviteGeneral_British` | CALDERON | VIDALYSALVADOR | 111 | 111/111 (100%) | 13.75 | VIDALYSALVADOR (111) |
| high | `Calderon_ManosblancasnoofendenLas` | CALDERON | VIDALYSALVADOR | 103 | 95/103 (92%) | 13.72 | VIDALYSALVADOR (95), BELMONTE (2) |
| high | `Calderon_autos_Novenatomo2` | CALDERON | CASTROYSALAZAR | 285 | 228/285 (80%) | 13.64 | CASTROYSALAZAR (228), VIDALYSALVADOR (40), SANDOVAL (4), MELO (2), ENRIQUEZ (2) |
| high | `CALDERON_RedencionCautivos_BHM` | CALDERON | VIDALYSALVADOR | 68 | 63/68 (93%) | 13.03 | VIDALYSALVADOR (63), LEONORCUEVA (2), BELMONTE (1) |
| high | `CALDERON_AlcaideDeSiMismo1` | CALDERON | ROJASZORRILLA | 78 | 74/78 (95%) | 12.85 | ROJASZORRILLA (74), VALDIVIELSO (1) |
| high | `CALDERON_DiabloMudo` | CALDERON | MOLINAYMENDOZA | 26 | 23/26 (88%) | 12.23 | MOLINAYMENDOZA (23), CASTROYSALAZAR (2), TORRESLORENZODE (1) |
| high | `LOPE_Principemelancolico` | LOPE | CALLE | 44 | 41/44 (93%) | 12.18 | CALLE (41), BELMONTE (2) |
| high | `MORETO_Perendeca` | MORETO | LEIVARAMIREZ | 15 | 13/15 (87%) | 12.09 | LEIVARAMIREZ (13), GONZALEZDEBARCIA (1) |
| high | `CALDERON_JardinDeFalerina4` | CALDERON | VIDALYSALVADOR | 82 | 66/82 (80%) | 11.73 | VIDALYSALVADOR (66) |
| high | `MONTALBAN_PuertaMacarena1Parte` | MONTALBAN | AVELLANEDA | 40 | 36/40 (90%) | 11.51 | AVELLANEDA (36), REMON (1) |
| high | `CALDERON_PleitoMatrimonial_rubrica` | CALDERON | VIDALYSALVADOR | 69 | 65/69 (94%) | 11.48 | VIDALYSALVADOR (65), CASTILLOSOLORZANO (1) |
| high | `CALDERON_IglesiaSitiada` | CALDERON | GONZALEZDEBARCIA | 28 | 27/28 (96%) | 11.19 | GONZALEZDEBARCIA (27), VIDALYSALVADOR (1) |
| high | `CALDERON_LirioAzucena1_BHM` | CALDERON | VIDALYSALVADOR | 72 | 64/72 (89%) | 11.16 | VIDALYSALVADOR (64), GONZALEZDEBARCIA (3), ROMEROROQUE (2), ALARCON (1) |
| high | `CALDERON_CuraYEnfermedad2` | CALDERON | GILENRIQUEZ | 60 | 50/60 (83%) | 10.97 | GILENRIQUEZ (50), CASTROYSALAZAR (5), AVELLANEDA (4) |
| high | `LOPE_DiscretaenamoradaBritish` | LOPE | CANIZARES | 51 | 41/51 (80%) | 10.87 | CANIZARES (41), GILENRIQUEZ (5), CASTROYSALAZAR (4), BOLEAYALVARADO (1) |
| high | `QUEVEDO_edictocontraHurtadodeMendoza` | QUEVEDO | VARGASMACHUCA | 2 | 2/2 (100%) | 10.66 | VARGASMACHUCA (2) |
| high | `CALDERON_NoHayMasFortunaQueDios2` | CALDERON | MOLINAYMENDOZA | 25 | 22/25 (88%) | 10.09 | MOLINAYMENDOZA (22), GONZALEZDEBARCIA (1), ALARCON (1), CANIZARES (1) |
| medium | `LOPE_AdulteraPerdonadaLa` | LOPE | LICENCIADOROJAS | 31 | 20/31 (64%) | 41.37 | LICENCIADOROJAS (20), PSEUDOHURTADODEMENDOZA (1), CUEVAYSILVA (1), GONZALEZDEBARCIA (1) |
| medium | `LOPE_HermanoFrancisco` | LOPE | CARVAJAL | 51 | 36/51 (71%) | 23.94 | CARVAJAL (36), QUEVEDO (15) |
| medium | `Calderon_Fierasafeminaamor` | CALDERON | CASTROYSALAZAR | 49 | 39/49 (80%) | 21.71 | CASTROYSALAZAR (39) |
| medium | `Calderon_SecretavenganzadedonLopedeAlme` | CALDERON | BELMONTE | 59 | 47/59 (80%) | 19.62 | BELMONTE (47), MONTALBAN (3), CERVANTES (1), SANDOVAL (1), ROJASZORRILLA (1) |
| medium | `LOPE_Gansooro` | LOPE | MEDINA | 44 | 28/44 (64%) | 19.32 | MEDINA (28), TORRESLORENZODE (12), GILENRIQUEZ (3) |
| medium | `Calderon_Casacondospuertas_2` | CALDERON | CLARAMONTE | 58 | 45/58 (78%) | 16.62 | CLARAMONTE (45), AGUADOELVIEJO (3), GONZALEZDEBARCIA (2), LICENCIADOROJAS (1) |
| medium | `Calderon_HijosdelafortunaTeagenesyClari` | CALDERON | MORETO | 84 | 65/84 (77%) | 16.39 | MORETO (65), LOPEZDELCAMPO (2), GILENRIQUEZ (2), CECILIANACIMIENTO (1), GRACIAN (1) |
| medium | `Calderon_Autossacramentales_2` | CALDERON | MOLINAYMENDOZA | 239 | 149/239 (62%) | 16.07 | MOLINAYMENDOZA (149), MORETO (44), JIMENEZSEDENO (10), ALARCON (9), CASTILLOSOLORZANO (5) |
| medium | `LOPE_LlaveHonraBritish` | LOPE | CANIZARES | 40 | 28/40 (70%) | 15.15 | CANIZARES (28), GILENRIQUEZ (8), CASTROYSALAZAR (4) |
| medium | `LOPE_EnganaraquienenganaBritish` | LOPE | GILENRIQUEZ | 37 | 26/37 (70%) | 14.90 | GILENRIQUEZ (26), CASTROYSALAZAR (7), LANINI (4) |
| medium | `CALDERON_JardinDeFalerina2` | CALDERON | MOLINAYMENDOZA | 29 | 21/29 (72%) | 14.34 | MOLINAYMENDOZA (21), CASTROYSALAZAR (7), JIMENEZSEDENO (1) |
| medium | `CALDERON_AutosSacramentalesTomoPrimero` | CALDERON | MOLINAYMENDOZA | 253 | 194/253 (77%) | 14.29 | MOLINAYMENDOZA (194), CASTROYSALAZAR (12), JIMENEZSEDENO (7), TORRESLORENZODE (7), ROMEROROQUE (5) |
| medium | `CALDERON_AfectosDeOdioYAmor` | CALDERON | BELMONTE | 128 | 89/128 (70%) | 14.25 | BELMONTE (89), CALLE (9), VIDALYSALVADOR (6), JIMENEZSEDENO (2), GONZALEZDEBARCIA (1) |
| medium | `LOPE_CuerdoLoco_Autografo` | LOPE | REMON | 127 | 97/127 (76%) | 13.92 | REMON (97), LEONORCUEVA (7), CERVANTES (5), LICENCIADOROJAS (2), HOZYMOTA (1) |
| medium | `Calderon_TriunfodeJuanRanaEl` | CALDERON | SANDOVAL | 12 | 7/12 (58%) | 13.80 | SANDOVAL (7), CERVANTES (1), CASTILLOSOLORZANO (1), VIDALYSALVADOR (1), GRACIAN (1) |
| medium | `CLARAMONTE_MuertePoncioPilates` | CLARAMONTE | REMON | 48 | 38/48 (79%) | 13.01 | REMON (38), CARVAJAL (4), ROJASZORRILLA (3), CAXESI (3) |
| medium | `CALDERON_AutosSacramentalesTomoSegundo` | CALDERON | MOLINAYMENDOZA | 249 | 160/249 (64%) | 12.67 | MOLINAYMENDOZA (160), TORRESLORENZODE (21), ALARCON (20), CAXESI (10), BANCESCANDAMO (5) |
| medium | `CALDERON_SaberdelMalydelBien` | CALDERON | BELMONTE | 58 | 38/58 (66%) | 12.65 | BELMONTE (38), LEIVARAMIREZ (12), CERVANTES (1), HURTADODEMENDOZA (1), SANDOVAL (1) |
| medium | `ROJASZORRILLA_CelosdeRodamonte_British` | ROJASZORRILLA | MORETO | 47 | 28/47 (60%) | 12.58 | MORETO (28), ROSETENINO (4), LORENZANA (3), LANINI (2), GILENRIQUEZ (2) |
| medium | `CALDERON_AutosSacramentales3` | CALDERON | VIDALYSALVADOR | 808 | 527/808 (65%) | 12.42 | VIDALYSALVADOR (527), VERATASSIS (143), PAREDES (43), LANINI (29), MORETO (19) |
| medium | `CALDERON_DiosPorRazonDeEstado3` | CALDERON | MOLINAYMENDOZA | 28 | 22/28 (79%) | 12.37 | MOLINAYMENDOZA (22), JIMENEZSEDENO (4), TORRESLORENZODE (1), LANINI (1) |
| medium | `Calderon_VirgendeSopetranLa` | CALDERON | CLARAMONTE | 53 | 39/53 (74%) | 12.08 | CLARAMONTE (39), AGUADOELVIEJO (2), GONZALEZDEBARCIA (1), ROJASZORRILLA (1), ANDOSILLA (1) |
| medium | `GARCIADEPRADO_ComprarUnHombreSuMuerte_Autografo` | GARCIADEPRADO | ROSETENINO | 110 | 60/110 (55%) | 12.04 | ROSETENINO (60), GARCIADEPRADO (32), CONTRERAS (1), VIDALYSALVADOR (1), HOZYMOTA (1) |
| medium | `LOPE_MaspuedencelosBritish` | LOPE | CANIZARES | 41 | 23/41 (56%) | 12.03 | CANIZARES (23), GILENRIQUEZ (16), CASTROYSALAZAR (2) |
| medium | `Calderon_autos_Novenatomo4` | CALDERON | CASTROYSALAZAR | 294 | 201/294 (68%) | 11.55 | CASTROYSALAZAR (201), VIDALYSALVADOR (76), MELO (3), GONGORA (3), SARAVIAYMENDOZA (2) |
| medium | `VELEZ_AbadesaDelCielo` | VELEZ | MESA | 27 | 14/27 (52%) | 11.13 | MESA (14), TORRESLORENZODE (2), HURTADODEMENDOZA (1), PAREDES (1), AVELLANEDA (1) |
| medium | `CALDERON_AndromedaYPerseo` | CALDERON | SANDOVAL | 50 | 35/50 (70%) | 10.93 | SANDOVAL (35), LEONORCUEVA (4), FAJARDOYACEVEDO (2), CARVAJAL (1), GARCIAMARCOS (1) |
| medium | `LOPE_duda_ContrariosdeAmor` | LOPE | BELMONTE | 68 | 45/68 (66%) | 10.58 | BELMONTE (45), TORRESLORENZODE (5), LEIVARAMIREZ (5), SANDOVAL (3), ROJASVILLANDRANDO (3) |
| medium | `CALDERON_ArmasHermosura` | CALDERON | JIMENEZSEDENO | 72 | 44/72 (61%) | 10.57 | JIMENEZSEDENO (44), BOLEAYALVARADO (20), GILENRIQUEZ (2), LICENCIADOROJAS (1), MEDINA (1) |
| medium | `CANIZARES_ElProdigioDeLaSagraSorJuanaDeLaCruz` | CANIZARES | CASTROYSALAZAR | 67 | 39/67 (58%) | 10.36 | CASTROYSALAZAR (39), CANIZARES (23), LICENCIADOROJAS (1), LEONORCUEVA (1) |
| medium | `Calderon_SitiodeBredaEl` | CALDERON | BELMONTE | 68 | 40/68 (59%) | 10.23 | BELMONTE (40), ROJASZORRILLA (17), LEIVARAMIREZ (4), CERVANTES (2) |
| medium | `VELEZ_GUEVARA_ObligacionesdeHonor` | VELEZ | LORENZANA | 30 | 17/30 (57%) | 10.10 | LORENZANA (17), CECILIANACIMIENTO (11), VIDALYSALVADOR (1), GILENRIQUEZ (1) |
| medium | `CALDERON_GranTeatroDelMundo` | CALDERON | BELMONTE | 24 | 15/24 (62%) | 10.01 | BELMONTE (15), VIDALYSALVADOR (3), GONZALEZDEBARCIA (3), LANINI (2), CORDERO (1) |
| medium | `CALDERON_PrimerRefugioDelHombre` | CALDERON | MOLINAYMENDOZA | 27 | 24/27 (89%) | 9.99 | MOLINAYMENDOZA (24), CASTROYSALAZAR (1), JIMENEZSEDENO (1), ROMEROROQUE (1) |
| medium | `LOPE_LoqueestadeterminadoBritish` | LOPE | CANIZARES | 44 | 29/44 (66%) | 9.99 | CANIZARES (29), GILENRIQUEZ (11), CASTROYSALAZAR (4) |
| medium | `Calderon_PrincipeconstanteEsclavoporsup` | CALDERON | VIDALYSALVADOR | 60 | 37/60 (62%) | 9.98 | VIDALYSALVADOR (37), BELMONTE (16), CECILIANACIMIENTO (1), CERVANTES (1) |
| medium | `CALDERON_LlamadosYEscogidos_British` | CALDERON | VIDALYSALVADOR | 44 | 38/44 (86%) | 9.81 | VIDALYSALVADOR (38), LANINI (4), VERATASSIS (1), DIAMANTE (1) |
| medium | `CLARAMONTE_AtaudParaElVivo2` | CLARAMONTE | CANIZARES | 26 | 13/26 (50%) | 9.77 | CANIZARES (13), CASTROYSALAZAR (2), MORETO (2), VERATASSIS (1), GILENRIQUEZ (1) |
| medium | `ROJAS_NuestraSenoraRosario` | LICENCIADOROJAS | CARVAJAL | 20 | 18/20 (90%) | 9.66 | CARVAJAL (18), ALARCON (1), CAXESI (1) |
| medium | `Calderon_Autossacramentalesalegoricosyh` | CALDERON | VIDALYSALVADOR | 422 | 234/422 (56%) | 9.31 | VIDALYSALVADOR (234), CASTROYSALAZAR (151), LANINI (11), AVELLANEDA (8), MELO (6) |
| medium | `LOPE_GODINEZ_CoronaDerribada_Parma` | LOPE | MESA | 44 | 37/44 (84%) | 9.28 | MESA (37), MONTALBAN (6), CUEVAYSILVA (1) |
| medium | `GONGORA_Poesias` | GONGORA | MEDINA | 509 | 450/509 (88%) | 9.25 | MEDINA (450), LICENCIADOROJAS (17), LEONORCUEVA (17), AVELLANEDA (4), CERVANTES (3) |
| medium | `MONTALBAN_SantoDomingoEnSoriano` | MONTALBAN | MATOSFRAGOSO | 100 | 90/100 (90%) | 9.22 | MATOSFRAGOSO (90), VIDALYSALVADOR (2) |
| medium | `CLARAMONTE_AtaudParaElVivo` | CLARAMONTE | CASTROYSALAZAR | 55 | 37/55 (67%) | 9.13 | CASTROYSALAZAR (37), SANDOVAL (10), LICENCIADOROJAS (2), MELO (1) |
| medium | `Calderon_NohaymasfortunaqueDios_2` | CALDERON | CASTROYSALAZAR | 36 | 25/36 (69%) | 9.09 | CASTROYSALAZAR (25), MORETO (3), PACHECO (1), MOLINAYMENDOZA (1) |
| medium | `MONTALBAN_Atribuido_ElImposibleVencidoOlimpiaYVireno2y3Jornada` | MONTALBAN | TORRESLORENZODE | 43 | 28/43 (65%) | 8.97 | TORRESLORENZODE (28), CALLE (6), SANDOVAL (1), BELMONTE (1), FAJARDOYACEVEDO (1) |
| medium | `CALDERON_ADiosPorRazonDeEstado` | CALDERON | GONZALEZDEBARCIA | 48 | 33/48 (69%) | 8.94 | GONZALEZDEBARCIA (33), CORDERO (3), GODINEZMANRIQUE (3) |
| medium | `Calderon_GalanfantasmaEl` | CALDERON | CALLE | 86 | 61/86 (71%) | 8.88 | CALLE (61), LEIVARAMIREZ (8), GARCIAMARCOS (4), ROSETENINO (2), LANINI (1) |
| medium | `CALDERON_DiablomudoEl_Hispanic` | CALDERON | VIDALYSALVADOR | 44 | 41/44 (93%) | 8.82 | VIDALYSALVADOR (41), AMESCUA (1), GARCIADEPRADO (1), CASTILLOSOLORZANO (1) |
| medium | `ENRIQUEZ_ALoQueObliganLosCelos` | ENRIQUEZ | BELMONTE | 69 | 47/69 (68%) | 8.65 | BELMONTE (47), ENRIQUEZ (10), GONGORA (1), GARCIAMARCOS (1) |
| medium | `TIRSO_VELEZ_RomeraDeSantiago` | TIRSO | CASTROYSALAZAR | 54 | 45/54 (83%) | 8.57 | CASTROYSALAZAR (45), SANDOVAL (6), GILENRIQUEZ (1), REMON (1) |
| medium | `CALDERON_FortunasDeAndromedaYPerseo` | CALDERON | VERATASSIS | 132 | 114/132 (86%) | 8.55 | VERATASSIS (114), BOLEAYALVARADO (2), AVELLANEDA (2), REMON (1) |
| medium | `LOPE_PiadosovalencianoEl_British` | LOPE | GONZALEZDETORRES | 47 | 35/47 (74%) | 8.51 | GONZALEZDETORRES (35), CASTILLOSOLORZANO (6), LLOBREGATYESTEVE (4), HOZYMOTA (1) |
| medium | `Calderon_Primerrefugiodelhombreyprobati` | CALDERON | VIDALYSALVADOR | 38 | 20/38 (53%) | 8.37 | VIDALYSALVADOR (20), MOLINAYMENDOZA (13), CERVANTES (1) |
| medium | `CALDERON_AutosSacramentales2` | CALDERON | GONZALEZDEBARCIA | 408 | 345/408 (85%) | 8.19 | GONZALEZDEBARCIA (345), CANIZARES (17), ROMEROROQUE (13), MOLINAYMENDOZA (10), AVELLANEDADELACUEVA (5) |
| medium | `CALDERON_DivinaFilotea_BHM` | CALDERON | VIDALYSALVADOR | 104 | 102/104 (98%) | 7.99 | VIDALYSALVADOR (102) |
| medium | `Calderon_autos_Novenatomo11` | CALDERON | CASTROYSALAZAR | 336 | 181/336 (54%) | 7.95 | CASTROYSALAZAR (181), VIDALYSALVADOR (101), CANIZARES (12), GARCIAMARCOS (11), DIAMANTE (6) |
| medium | `CALDERON_Lirioyazucena_loa` | CALDERON | CARVAJAL | 12 | 9/12 (75%) | 7.87 | CARVAJAL (9), LORENZANA (2), CERVANTES (1) |
| medium | `TAMAYO_DescendenciaVelez` | TAMAYO | TORRESLORENZODE | 34 | 24/34 (71%) | 7.84 | TORRESLORENZODE (24), MEDINA (5), VARGAS (3), SARAVIAYMENDOZA (1), SANDOVAL (1) |
| medium | `Calderon_MisteriosdelamisaLos` | CALDERON | GONZALEZDEBARCIA | 40 | 27/40 (68%) | 7.67 | GONZALEZDEBARCIA (27), GODINEZMANRIQUE (2), CORDERO (1) |
| medium | `CALDERON_Mejorestaqueestaba_Hisp` | CALDERON | ROSETENINO | 64 | 33/64 (52%) | 7.63 | ROSETENINO (33), PAREDES (15), ENRIQUEZ (4), BATRES (3), QUINONES (2) |
| medium | `CALDERON_InmunidadSagrado_BHM` | CALDERON | VIDALYSALVADOR | 82 | 80/82 (98%) | 7.50 | VIDALYSALVADOR (80), HOZYMOTA (1) |
| medium | `CALDERON_VerdaderodiosPanEl_British` | CALDERON | VIDALYSALVADOR | 70 | 38/70 (54%) | 7.48 | VIDALYSALVADOR (38), CANIZARES (8), CASTROYSALAZAR (7), LANINI (6), GONZALEZDEBARCIA (3) |
| medium | `ALARCON_Vencidovencedor_Parma` | ALARCON | QUEVEDO | 58 | 42/58 (72%) | 7.44 | QUEVEDO (42), BELMONTE (6), MONTALBAN (5), LEIVARAMIREZ (2), VERATASSIS (1) |
| medium | `CALDERON_PolifemoCirce_acto3_Autografo` | CALDERON | QUINONES | 33 | 28/33 (85%) | 7.35 | QUINONES (28), CALDERON (3), BELMONTE (1), MONTALBAN (1) |
| medium | `CALDERON_NuevoHospicioDePobres` | CALDERON | VERATASSIS | 124 | 113/124 (91%) | 7.34 | VERATASSIS (113), GONZALEZDEBARCIA (1), VIDALYSALVADOR (1), AVELLANEDA (1) |
| medium | `GONGORA_Obras` | GONGORA | AVELLANEDA | 709 | 564/709 (80%) | 7.21 | AVELLANEDA (564), LICENCIADOROJAS (68), CECILIANACIMIENTO (10), MEDINA (4), MELO (3) |
| medium | `LOPE_Porfiarhastamorir_British` | LOPE | GONZALEZDETORRES | 46 | 33/46 (72%) | 7.07 | GONZALEZDETORRES (33), CASTILLOSOLORZANO (8), LLOBREGATYESTEVE (3), GONGORA (1) |
| medium | `ROJAS_SelvadeAmor` | LICENCIADOROJAS | LORENZANA | 20 | 14/20 (70%) | 7.04 | LORENZANA (14), PACHECO (5) |
| medium | `LOPE_DivinaVencedora_Parma` | LOPE | GARCIADEPRADO | 41 | 32/41 (78%) | 6.98 | GARCIADEPRADO (32), ENRIQUEZ (5), BATRES (2), MONTALBAN (1), CASTILLOSOLORZANO (1) |
| medium | `CALDERON_DevocionDeLaMisa` | CALDERON | VIDALYSALVADOR | 41 | 25/41 (61%) | 6.96 | VIDALYSALVADOR (25), PAREDES (14), BANCESCANDAMO (1), GONZALEZDEBARCIA (1) |
| medium | `CALDERON_Redencioncautivos_loa` | CALDERON | LORENZANA | 12 | 7/12 (58%) | 6.95 | LORENZANA (7), CARVAJAL (3), CERVANTES (1), TORRESLORENZODE (1) |
| medium | `CALDERON_devocionmisa_loa` | CALDERON | CARVAJAL | 12 | 8/12 (67%) | 6.90 | CARVAJAL (8), LORENZANA (3), CERVANTES (1) |
| medium | `CALDERON_JardinDeFalerina1` | CALDERON | VERATASSIS | 100 | 76/100 (76%) | 6.76 | VERATASSIS (76), VIDALYSALVADOR (2), CASTILLOSOLORZANO (1), AVELLANEDA (1), SANDOVAL (1) |
| medium | `LOPE_NuestraSenoraRosario` | LOPE | TORRESLORENZODE | 17 | 15/17 (88%) | 6.72 | TORRESLORENZODE (15), LORENZANA (2) |
| medium | `MONTALBAN_ComoPadreYComoRey` | MONTALBAN | VIDALYSALVADOR | 190 | 167/190 (88%) | 6.63 | VIDALYSALVADOR (167), LICENCIADOROJAS (4), LOPEZDELCAMPO (1), LEONORCUEVA (1), QUINONES (1) |
| medium | `CALDERON_ViaticoCordero` | CALDERON | MELO | 41 | 37/41 (90%) | 6.61 | MELO (37), SANDOVAL (3), ONAVIEDMAYTORRES (1) |
| medium | `ENRIQUEZ_AmorConVistaYCordura` | ENRIQUEZ | PAREDES | 70 | 43/70 (61%) | 6.60 | PAREDES (43), VARGASMACHUCA (14), ONAVIEDMAYTORRES (1), VIDALYSALVADOR (1), CECILIANACIMIENTO (1) |
| medium | `CALDERON_AndromedaYPerseo4` | CALDERON | VERATASSIS | 84 | 42/84 (50%) | 6.60 | VERATASSIS (42), SANDOVAL (35), AVELLANEDA (2), HOZYMOTA (1), MEDINA (1) |
| medium | `CALDERON_escondidoytapada` | CALDERON | AVELLANEDA | 40 | 33/40 (82%) | 6.48 | AVELLANEDA (33), LICENCIADOROJAS (7) |
| medium | `Calderon_GranmercadodelmundoEl` | CALDERON | GONZALEZDEBARCIA | 47 | 32/47 (68%) | 6.43 | GONZALEZDEBARCIA (32), GODINEZMANRIQUE (3), CANIZARES (2), LICENCIADOROJAS (1), GARCIADEPRADO (1) |
| medium | `Calderon_EspigasdeRuthLas` | CALDERON | MELO | 58 | 46/58 (79%) | 6.39 | MELO (46), GONZALEZDEBARCIA (1), SANDOVAL (1), VARGASMACHUCA (1) |
| medium | `CALDERON_DosEstrellasDeFrancia` | CALDERON | GONZALEZDEBARCIA | 25 | 22/25 (88%) | 6.38 | GONZALEZDEBARCIA (22), CASTROYSALAZAR (1), VIDALYSALVADOR (1), BANCESCANDAMO (1) |
| medium | `CALDERON_SemillaCizana_BHM` | CALDERON | VIDALYSALVADOR | 95 | 94/95 (99%) | 6.36 | VIDALYSALVADOR (94) |
| medium | `CALDERON_EcoYNarciso1` | CALDERON | VIDALYSALVADOR | 92 | 63/92 (68%) | 6.35 | VIDALYSALVADOR (63), GARCIADEPRADO (8), DIAMANTE (4), LEONORCUEVA (1), CANIZARES (1) |
| medium | `LOPE_Acreedores` | LOPE | CAXESI | 14 | 8/14 (57%) | 6.29 | CAXESI (8), REMON (5), CARVAJAL (1) |
| medium | `CALDERON_AutosHarvard` | CALDERON | SANDOVAL | 746 | 421/746 (56%) | 6.27 | SANDOVAL (421), CASTROYSALAZAR (216), LANINI (38), PAREDES (20), MELO (10) |
| medium | `CALDERON_FloresPompaDeAbril` | CALDERON | MOLINAYMENDOZA | 6 | 5/6 (83%) | 6.26 | MOLINAYMENDOZA (5), TORRESLORENZODE (1) |
| medium | `CANIZARES_TemploymontedeFilisyDemofonte_British` | CANIZARES | SANDOVAL | 127 | 96/127 (76%) | 6.25 | SANDOVAL (96), CASTROYSALAZAR (11), VERATASSIS (4), GILENRIQUEZ (3), LEONORCUEVA (2) |
| medium | `CALDERON_MaestrazgoToison_BHM` | CALDERON | VIDALYSALVADOR | 97 | 89/97 (92%) | 6.21 | VIDALYSALVADOR (89), BANCESCANDAMO (1), CASTILLOSOLORZANO (1), PAREDES (1) |
| medium | `Calderon_Troyaabrasada` | CALDERON | CASTROYSALAZAR | 34 | 21/34 (62%) | 6.19 | CASTROYSALAZAR (21), LOPEZDECARDENA (7), CANIZARES (4), VERATASSIS (1), MELO (1) |
| medium | `CALDERON_AcasoYElError_Parma` | CALDERON | AVELLANEDA | 57 | 46/57 (81%) | 6.15 | AVELLANEDA (46), MELO (5), MEDINA (3), SANDOVAL (2), LICENCIADOROJAS (1) |
| medium | `MONTALBAN_DeUnCastigoDosVenganzas_British` | MONTALBAN | ROJASZORRILLA | 94 | 61/94 (65%) | 6.13 | ROJASZORRILLA (61), QUEVEDO (14), GALLEGOS (11), BELMONTE (2), CUENCAYARGUELLO (1) |
| medium | `CALDERON_Arcacaptiva` | CALDERON | CARVAJAL | 47 | 33/47 (70%) | 6.11 | CARVAJAL (33), LORENZANA (12), CERVANTES (2) |
| medium | `LOPE_BautismoPrincipe_USevilla` | LOPE | MORETO | 50 | 31/50 (62%) | 6.08 | MORETO (31), CANIZARES (15), GILENRIQUEZ (3), ROJASZORRILLA (1) |
| medium | `CALDERON_MaestrazgoDeToison` | CALDERON | VIDALYSALVADOR | 34 | 28/34 (82%) | 6.02 | VIDALYSALVADOR (28), PAREDES (2), GONZALEZDEBARCIA (2), LANINI (1), BANCESCANDAMO (1) |
| medium | `CALDERON_DiabloMudo_BHM` | CALDERON | VIDALYSALVADOR | 87 | 79/87 (91%) | 6.01 | VIDALYSALVADOR (79), GONZALEZDEBARCIA (5), GODINEZMANRIQUE (1) |
| medium | `CALDERON_PielGedeon2_BHM` | CALDERON | VIDALYSALVADOR | 64 | 57/64 (89%) | 5.94 | VIDALYSALVADOR (57), MOLINAYMENDOZA (5) |
| medium | `CALDERON_AnoSantoDeRoma2` | CALDERON | GONZALEZDEBARCIA | 48 | 32/48 (67%) | 5.80 | GONZALEZDEBARCIA (32), GARCIADEPRADO (5), GODINEZMANRIQUE (1) |
| medium | `CALDERON_OrdenDeMelchisedech2` | CALDERON | VIDALYSALVADOR | 32 | 28/32 (88%) | 5.79 | VIDALYSALVADOR (28), PAREDES (2), CANIZARES (1), DIAMANTE (1) |
| medium | `ROJASZORRILLA_Memorialdelosquedefienden_autografo` | ROJASZORRILLA | ENRIQUEZ | 9 | 5/9 (56%) | 5.78 | ENRIQUEZ (5), CECILIANACIMIENTO (4) |
| medium | `CALDERON_AnoSantoDeRoma3` | CALDERON | GONZALEZDEBARCIA | 49 | 33/49 (67%) | 5.77 | GONZALEZDEBARCIA (33), GARCIADEPRADO (5), CORDERO (1), CONTRERAS (1) |
| medium | `CALDERON_SuenosHayQueVerdadSon` | CALDERON | GONZALEZDEBARCIA | 45 | 26/45 (58%) | 5.75 | GONZALEZDEBARCIA (26), VIDALYSALVADOR (12), PAREDES (5), CASTROYSALAZAR (2) |
| medium | `CALDERON_LoaJuegoPelota` | CALDERON | TORRESLORENZODE | 14 | 7/14 (50%) | 5.67 | TORRESLORENZODE (7), PAREDES (2), VIDALYSALVADOR (1), GILENRIQUEZ (1), BELMONTE (1) |
| medium | `CALDERON_MaestrazgoDelTuson_Autografo` | CALDERON | VIDALYSALVADOR | 112 | 65/112 (58%) | 5.65 | VIDALYSALVADOR (65), PAREDES (15), PSEUDOHURTADODEMENDOZA (1), LEIVARAMIREZ (1), COELLO (1) |
| medium | `CALDERON_SemillaYLaCizana` | CALDERON | VIDALYSALVADOR | 33 | 28/33 (85%) | 5.65 | VIDALYSALVADOR (28), CANIZARES (3), GARCIADEPRADO (1), CORDERO (1) |
| medium | `TIRSO_BalconesDeMadrid_Parma` | TIRSO | LICENCIADOROJAS | 62 | 47/62 (76%) | 5.65 | LICENCIADOROJAS (47), CARVAJAL (6), CERVANTES (5), REMON (2), LORENZANA (1) |
| medium | `DIAMANTE_ManceboDelCamino` | DIAMANTE | TORRESLORENZODE | 140 | 87/140 (62%) | 5.63 | TORRESLORENZODE (87), LEIVARAMIREZ (12), VIDALYSALVADOR (11), JIMENEZSEDENO (6), PAREDES (2) |
| medium | `CALDERON_AnoSantoEnMadrid` | CALDERON | MELO | 40 | 29/40 (72%) | 5.62 | MELO (29), SANDOVAL (5), VARGASMACHUCA (3), ONAVIEDMAYTORRES (3) |
| medium | `CALDERON_BastaCallar_Autografo` | CALDERON | LEIVARAMIREZ | 175 | 104/175 (59%) | 5.58 | LEIVARAMIREZ (104), BATRES (18), CALLE (9), CALDERON (7), QUINONES (5) |
| medium | `GONGORA_Poesiasycorrecciones` | GONGORA | VIDALYSALVADOR | 398 | 202/398 (51%) | 5.53 | VIDALYSALVADOR (202), PAREDES (60), VALDIVIELSO (43), CECILIANACIMIENTO (41), CASTILLOSOLORZANO (17) |
| medium | `CALDERON_Pintordeshonra` | CALDERON | CARVAJAL | 47 | 33/47 (70%) | 5.46 | CARVAJAL (33), LORENZANA (11), CERVANTES (2), GARCIADEPRADO (1) |
| medium | `CALDERON_JardinDeFalerina3` | CALDERON | VERATASSIS | 112 | 103/112 (92%) | 5.45 | VERATASSIS (103), LICENCIADOROJAS (1), LOPEZDELCAMPO (1), VIDALYSALVADOR (1) |
| medium | `CALDERON_LaberintodelMundoBNE` | CALDERON | GONZALEZDEBARCIA | 60 | 47/60 (78%) | 5.40 | GONZALEZDEBARCIA (47), GODINEZMANRIQUE (2), GONGORA (1), BOLEAYALVARADO (1) |
| medium | `LOPE_EsclavoVenecia_Parma` | LOPE | QUEVEDO | 47 | 33/47 (70%) | 5.39 | QUEVEDO (33), MONTALBAN (6), BELMONTE (4), LEIVARAMIREZ (2), CASTILLOSOLORZANO (1) |
| medium | `LOPE_Montanesa` | LOPE | CALLE | 48 | 32/48 (67%) | 5.38 | CALLE (32), SANDOVAL (4), VARGAS (2), JUANDESOTO (2), GARCIAMARCOS (1) |
| medium | `Calderon_Saberdelmalydelbien_2` | CALDERON | CASTROYSALAZAR | 88 | 52/88 (59%) | 5.33 | CASTROYSALAZAR (52), ROMEROROQUE (14), JIMENEZSEDENO (7), MOLINAYMENDOZA (2), GARCIAMARCOS (2) |
| medium | `CALDERON_DivinaFilotea` | CALDERON | LORENZANA | 54 | 30/54 (56%) | 5.33 | LORENZANA (30), CARVAJAL (23), CERVANTES (1) |
| medium | `CALDERON_NaveDelMercader1` | CALDERON | VIDALYSALVADOR | 94 | 83/94 (88%) | 5.30 | VIDALYSALVADOR (83), VERATASSIS (4), CASTROYSALAZAR (2), MARCHANTE (2), VALDIVIELSO (1) |
| medium | `LOPE_PastorSoldado` | LOPE | REMON | 54 | 29/54 (54%) | 5.25 | REMON (29), ENRIQUEZ (15), BELMONTE (9), QUEVEDO (1) |
| medium | `CALDERON_AnoSantoRoma_loa` | CALDERON | CARVAJAL | 8 | 7/8 (88%) | 5.22 | CARVAJAL (7), CERVANTES (1) |
| medium | `CALDERON_ConsumoDelVellon_British` | CALDERON | VIDALYSALVADOR | 47 | 24/47 (51%) | 5.22 | VIDALYSALVADOR (24), CANIZARES (14), GONGORA (6), CASTROYSALAZAR (1), GARCIADEPRADO (1) |
| medium | `LOPE_ObrassonAmores_Parma` | LOPE | BELMONTE | 55 | 40/55 (73%) | 5.19 | BELMONTE (40), SANDOVAL (7), LEIVARAMIREZ (4), VALDIVIELSO (2), VERATASSIS (1) |
| medium | `Calderon_Dichaydesdichadelhombre` | CALDERON | ENRIQUEZ | 41 | 24/41 (58%) | 5.19 | ENRIQUEZ (24), MOLINAYMENDOZA (5), BELMONTE (2), SANDOVAL (1), FAJARDOYACEVEDO (1) |
| medium | `CALDERON_AndromedayPerseo_Pelayo` | CALDERON | CARVAJAL | 47 | 34/47 (72%) | 5.19 | CARVAJAL (34), LORENZANA (12), CERVANTES (1) |
| medium | `CALDERON_LoQueVa_Autografo` | CALDERON | GILENRIQUEZ | 31 | 16/31 (52%) | 5.14 | GILENRIQUEZ (16), CALDERON (12), MARCHANTE (2), VILLEGASJUANBAUTISTA (1) |
| medium | `LOPE_RamilletesdeMadrid_Parma` | LOPE | LEIVARAMIREZ | 57 | 41/57 (72%) | 5.08 | LEIVARAMIREZ (41), BELMONTE (11), MORETO (1) |
| medium | `CALDERON_PrimerFlorCarmelo` | CALDERON | VIDALYSALVADOR | 92 | 63/92 (68%) | 4.99 | VIDALYSALVADOR (63), PAREDES (6), LICENCIADOROJAS (2), CASTILLOSOLORZANO (2), CERVANTES (1) |
| medium | `Calderon_LirioylaazucenaolapazgeneralEl` | CALDERON | GONZALEZDEBARCIA | 56 | 33/56 (59%) | 4.86 | GONZALEZDEBARCIA (33), GODINEZMANRIQUE (8), AVELLANEDADELACUEVA (2), CORDERO (2), PAREDES (1) |
| medium | `VIDALYSALVADOR_MusicaEnsenaElAmor` | VIDALYSALVADOR | PAREDES | 53 | 45/53 (85%) | 4.84 | PAREDES (45), VIDALYSALVADOR (4), BARREDA (1) |
| medium | `LOPE_Amistadpagada` | LOPE | AVELLANEDA | 58 | 46/58 (79%) | 4.83 | AVELLANEDA (46), QUEVEDO (11), VIDALYSALVADOR (1) |
| medium | `CALDERON_Diablomudo_loa` | CALDERON | CARVAJAL | 12 | 10/12 (83%) | 4.81 | CARVAJAL (10), LORENZANA (2) |
| medium | `CALDERON_PrimerRefugio_British` | CALDERON | VIDALYSALVADOR | 64 | 40/64 (62%) | 4.79 | VIDALYSALVADOR (40), GONGORA (16), LANINI (2), VARGASMACHUCA (1), CANIZARES (1) |
| medium | `CALDERON_DiabloMudo3` | CALDERON | SANDOVAL | 112 | 64/112 (57%) | 4.75 | SANDOVAL (64), VERATASSIS (40), MELO (1), GONGORA (1), MENESES (1) |
| medium | `CALDERON_PrimerRefugioDelHombre1` | CALDERON | VIDALYSALVADOR | 68 | 52/68 (76%) | 4.75 | VIDALYSALVADOR (52), MONTALBAN (6), VERATASSIS (2), VALDIVIELSO (2), AMESCUA (1) |
| medium | `CALDERON_LoaParaElAutoDeElDivinoOrfeo` | CALDERON | MOLINAYMENDOZA | 14 | 9/14 (64%) | 4.75 | MOLINAYMENDOZA (9), CALLE (2), JIMENEZSEDENO (1), FAJARDOYACEVEDO (1), AVELLANEDADELACUEVA (1) |
| medium | `CALDERON_SacroParnaso_loa` | CALDERON | CARVAJAL | 12 | 11/12 (92%) | 4.75 | CARVAJAL (11), LORENZANA (1) |
| medium | `CALDERON_LaberintoMundo_BHM` | CALDERON | VIDALYSALVADOR | 99 | 90/99 (91%) | 4.72 | VIDALYSALVADOR (90), MOLINAYMENDOZA (4), HOZYMOTA (1), FAJARDOYACEVEDO (1), BELMONTE (1) |
| medium | `HOZ_ComolaLunaMenguante` | HOZYMOTA | GONZALEZDEBARCIA | 69 | 48/69 (70%) | 4.64 | GONZALEZDEBARCIA (48), VIDALYSALVADOR (9), GARCIADEPRADO (8), LEONORCUEVA (1), CASTROYSALAZAR (1) |
| medium | `CALDERON_AmarYSerAmado` | CALDERON | VIDALYSALVADOR | 36 | 22/36 (61%) | 4.59 | VIDALYSALVADOR (22), BELMONTE (13), VERATASSIS (1) |
| medium | `CALDERON_OrdenDeMelchisedech` | CALDERON | MELO | 41 | 37/41 (90%) | 4.58 | MELO (37), CASTROYSALAZAR (2), SANDOVAL (2) |
| medium | `CALDERON_MemoriaMayorencantoamor_Autografo` | CALDERON | HURTADODEMENDOZA | 2 | 2/2 (100%) | 4.56 | HURTADODEMENDOZA (2) |
| medium | `LOPE_SegundoDavid_British` | LOPE | GARCIADEPRADO | 35 | 28/35 (80%) | 4.45 | GARCIADEPRADO (28), BATRES (2), LEIVARAMIREZ (2), SANDOVAL (1), LOPE (1) |
| medium | `CALDERON_CorderoDeIsaias1` | CALDERON | VIDALYSALVADOR | 115 | 75/115 (65%) | 4.43 | VIDALYSALVADOR (75), MOLINAYMENDOZA (32), GONZALEZDEBARCIA (4), GONZALEZDETORRES (2), CASTROYSALAZAR (2) |
| medium | `CALDERON_AnoSantoRoma` | CALDERON | CARVAJAL | 48 | 29/48 (60%) | 4.39 | CARVAJAL (29), LORENZANA (15), CERVANTES (2), GILENRIQUEZ (1), BANCESCANDAMO (1) |
| medium | `LOPE_LocuraporlaHonra_Parma` | LOPE | BELMONTE | 53 | 31/53 (58%) | 4.39 | BELMONTE (31), LEIVARAMIREZ (15), VIDALYSALVADOR (3), QUEVEDO (1), VERATASSIS (1) |
| medium | `CALDERON_Venenoytriaca` | CALDERON | CARVAJAL | 52 | 43/52 (83%) | 4.38 | CARVAJAL (43), LORENZANA (4), CERVANTES (2), BANCESCANDAMO (2), TORRESLORENZODE (1) |
| medium | `CALDERON_LirioAzucena` | CALDERON | CARVAJAL | 52 | 42/52 (81%) | 4.37 | CARVAJAL (42), LORENZANA (5), CERVANTES (4), HOZYMOTA (1) |
| medium | `LOPE_AlmenasDeToro` | LOPE | ROMEROROQUE | 56 | 31/56 (55%) | 4.35 | ROMEROROQUE (31), LOPEZDECASTRO (8), GALLEGOS (6), GONZALEZDEBARCIA (1), CASTILLOSOLORZANO (1) |
| medium | `CALDERON_LoadelapiadosaHermandad` | CALDERON | GONZALEZDEBARCIA | 10 | 9/10 (90%) | 4.33 | GONZALEZDEBARCIA (9), LANINI (1) |
| medium | `CALDERON_afectosodioamor` | CALDERON | AVELLANEDA | 49 | 45/49 (92%) | 4.31 | AVELLANEDA (45), LICENCIADOROJAS (1), CLARAMONTE (1) |
| medium | `Calderon_Bastacallar` | CALDERON | ROSETENINO | 60 | 30/60 (50%) | 4.26 | ROSETENINO (30), TORRESLORENZODE (7), LANINI (4), MULSA (4), LICENCIADOROJAS (1) |
| medium | `HURTADODEMENDOZA_QuererPorSoloQuerer` | HURTADODEMENDOZA | VIDALYSALVADOR | 204 | 103/204 (50%) | 4.26 | VIDALYSALVADOR (103), VARGASMACHUCA (64), CECILIANACIMIENTO (7), JIMENEZSEDENO (3), PAREDES (2) |
| medium | `CALDERON_PastorFido_BHM` | CALDERON | VIDALYSALVADOR | 70 | 45/70 (64%) | 4.26 | VIDALYSALVADOR (45), MOLINAYMENDOZA (21) |
| medium | `LOPE_ArmindaCelosa` | LOPE | FAJARDOYACEVEDO | 50 | 35/50 (70%) | 4.22 | FAJARDOYACEVEDO (35), ROMEROROQUE (5), GARCIAMARCOS (2), CARVAJAL (1), ENRIQUEZ (1) |
| medium | `CALDERON_DiaMayorDias_rubrica` | CALDERON | GONGORA | 103 | 86/103 (84%) | 4.20 | GONGORA (86), VIDALYSALVADOR (10), SANTATERESA (1), GONZALEZDEBARCIA (1), BARREDA (1) |
| medium | `LOPE_VerdaderoAmante_Sorbonne` | LOPE | GARCIADEPRADO | 73 | 40/73 (55%) | 4.20 | GARCIADEPRADO (40), SARAVIAYMENDOZA (12), ENRIQUEZ (3), HURTADODEMENDOZA (2), QUINONES (1) |
| medium | `CALDERON_Triunfarmuriendo` | CALDERON | CARVAJAL | 46 | 31/46 (67%) | 4.18 | CARVAJAL (31), LORENZANA (12), CERVANTES (3) |
| medium | `CALDERON_EspigasdeRuth` | CALDERON | CARVAJAL | 48 | 26/48 (54%) | 4.17 | CARVAJAL (26), LORENZANA (21), CERVANTES (1) |
| medium | `CALDERON_NaveDelMercader` | CALDERON | VERATASSIS | 120 | 115/120 (96%) | 4.13 | VERATASSIS (115), VIDALYSALVADOR (2) |
| medium | `CALDERON_ViaticoCordero_BHM` | CALDERON | VIDALYSALVADOR | 102 | 96/102 (94%) | 4.12 | VIDALYSALVADOR (96), MOLINAYMENDOZA (2), GONZALEZDEBARCIA (1), GONGORA (1), CASTROYSALAZAR (1) |
| medium | `CANIZARES_HastaLoInsensibleAdora` | CANIZARES | CASTROYSALAZAR | 33 | 24/33 (73%) | 4.12 | CASTROYSALAZAR (24), GILENRIQUEZ (6), VERATASSIS (1), GONGORA (1), CERVANTES (1) |
| medium | `CALDERON_PajedonAlvaro` | CALDERON | LOPEZDECARDENA | 61 | 35/61 (57%) | 4.11 | LOPEZDECARDENA (35), LANINI (14), VERATASSIS (4), LORENZANA (2), VALDIVIELSO (2) |
| medium | `CALDERON_EspigasDeRuth_British` | CALDERON | GARCIADEPRADO | 44 | 33/44 (75%) | 4.05 | GARCIADEPRADO (33), ROJASVILLANDRANDO (5), CARVAJAL (2), BATRES (2), MARCHANTE (1) |
| medium | `LOPE_Mejoralcaldeelrey_Hisp` | LOPE | VIDALYSALVADOR | 52 | 38/52 (73%) | 4.04 | VIDALYSALVADOR (38), GARCIADEPRADO (9), GONGORA (2), ENRIQUEZ (1), CANIZARES (1) |
| medium | `LOPE_AudienciasDelReyDonPedro` | LOPE | TORRESLORENZODE | 63 | 38/63 (60%) | 4.03 | TORRESLORENZODE (38), PAREDES (8), LEIVARAMIREZ (4), GARCIAMARCOS (2), LICENCIADOROJAS (1) |
| medium | `VELEZ_GUEVARA_LuceroDeCastilla` | VELEZ | MARCHANTE | 77 | 50/77 (65%) | 4.02 | MARCHANTE (50), SARAVIAYMENDOZA (11), GILENRIQUEZ (7), GARCIADEPRADO (5), SANDOVAL (1) |
| medium | `CALDERON_SegundoEscipion_PBA` | CALDERON | MELO | 227 | 196/227 (86%) | 4.01 | MELO (196), GARCIAMARCOS (4), VIDALYSALVADOR (2), LICENCIADOROJAS (1), GONZALEZDETORRES (1) |
| medium | `CALDERON_SegundoScipion` | CALDERON | MELO | 227 | 196/227 (86%) | 4.01 | MELO (196), GARCIAMARCOS (4), VIDALYSALVADOR (2), LICENCIADOROJAS (1), GONZALEZDETORRES (1) |
| medium | `Calderon_PsiquisyCupido_2` | CALDERON | GONZALEZDEBARCIA | 42 | 27/42 (64%) | 4.00 | GONZALEZDEBARCIA (27), GARCIADEPRADO (2), CANIZARES (1), ROMEROROQUE (1), GODINEZMANRIQUE (1) |
| medium | `LOPE_Amigohastalamuerte_Parma` | LOPE | AVELLANEDA | 68 | 55/68 (81%) | 3.97 | AVELLANEDA (55), LICENCIADOROJAS (6), CUEVAYSILVA (2), LANINI (1) |
| medium | `CALDERON_llamadosyescogidos_loa` | CALDERON | CARVAJAL | 11 | 9/11 (82%) | 3.91 | CARVAJAL (9), CERVANTES (2) |
| medium | `MORETO_SieteDurmientes` | MORETO | ONAVIEDMAYTORRES | 112 | 78/112 (70%) | 3.90 | ONAVIEDMAYTORRES (78), SANDOVAL (16), AVELLANEDADELACUEVA (6), LANINI (3), CALLE (2) |
| medium | `BELMONTE_AciertoEnElEnganoYRobadordesuHonraEl` | BELMONTE | QUINONES | 145 | 86/145 (59%) | 3.89 | QUINONES (86), CALLE (12), LOPEZJACINTO (6), CONTRERAS (5), FAJARDOYACEVEDO (5) |
| medium | `GARCES_AmorParaSerPerfectoHaDeTenerCuatroEses` | GARCIADEPRADO | VIDALYSALVADOR | 126 | 113/126 (90%) | 3.89 | VIDALYSALVADOR (113), DIAMANTE (5), VALDIVIELSO (1), GONGORA (1), VERATASSIS (1) |
| medium | `Calderon_Pleitomatrimonial4` | CALDERON | CANIZARES | 36 | 23/36 (64%) | 3.88 | CANIZARES (23), MATOSFRAGOSO (3), LORENZANA (2), AVELLANEDADELACUEVA (1), CUENCAYARGUELLO (1) |
| medium | `LOPE_Bautismodel_principedeMarruecos_Parma` | LOPE | BELMONTE | 60 | 43/60 (72%) | 3.84 | BELMONTE (43), LEIVARAMIREZ (6), AVELLANEDA (2), SANDOVAL (2), VERATASSIS (2) |
| medium | `CALDERON_CuboDeLaAlmudena` | CALDERON | VIDALYSALVADOR | 34 | 19/34 (56%) | 3.82 | VIDALYSALVADOR (19), PAREDES (6), GONZALEZDEBARCIA (6), BELMONTE (2), LANINI (1) |
| medium | `MENESES_VidaDeSanEstacio` | MENESES | GONGORA | 54 | 27/54 (50%) | 3.81 | GONGORA (27), CARVAJAL (18), TORRESLORENZODE (4), JUANDESOTO (2), QUEVEDO (2) |
| medium | `MORETO_Parecidocorte` | MORETO | VALDIVIELSO | 73 | 67/73 (92%) | 3.81 | VALDIVIELSO (67), VIDALYSALVADOR (2), LEONORCUEVA (1), MONTALBAN (1) |
| medium | `HURTADOMENDOZA_ExaminadorMiserPalomo` | HURTADODEMENDOZA | TORRESLORENZODE | 9 | 9/9 (100%) | 3.80 | TORRESLORENZODE (9) |
| medium | `CALDERON_Alimentoshombre_loa` | CALDERON | CARVAJAL | 11 | 10/11 (91%) | 3.80 | CARVAJAL (10), CERVANTES (1) |
| medium | `CALDERON_Serpientemetal` | CALDERON | CARVAJAL | 60 | 48/60 (80%) | 3.77 | CARVAJAL (48), LORENZANA (8), CERVANTES (2), BANCESCANDAMO (2) |
| medium | `MONTALBAN_CardenaldeMoron` | MONTALBAN | VERATASSIS | 155 | 144/155 (93%) | 3.77 | VERATASSIS (144), LEIVARAMIREZ (4), GONGORA (3), MORETO (3), SANDOVAL (1) |
| medium | `GONGORA_FirmezasdeIsabeLas` | GONGORA | CASTILLOSOLORZANO | 88 | 50/88 (57%) | 3.73 | CASTILLOSOLORZANO (50), GARCIADEPRADO (16), CALLE (9), PAREDES (6), CORDERO (1) |
| medium | `MONTALBAN_JuanCapistrano_British` | MONTALBAN | VIDALYSALVADOR | 142 | 82/142 (58%) | 3.72 | VIDALYSALVADOR (82), CASTROYSALAZAR (26), CANIZARES (25), GONGORA (4), SANTATERESA (1) |
| medium | `ROJAS_ZORRILLA_RobodeElena` | LICENCIADOROJAS | LORENZANA | 22 | 15/22 (68%) | 3.71 | LORENZANA (15), CAXESI (4), CECILIANACIMIENTO (1), CONTRERAS (1), LICENCIADOROJAS (1) |
| medium | `LOPE_BizarriasBelisa_Autografo` | LOPE | TAMAYO | 67 | 37/67 (55%) | 3.67 | TAMAYO (37), LOPE (5), MENESES (4), ROJASVILLANDRANDO (4), PSEUDOHURTADODEMENDOZA (2) |
| medium | `LANINI_AllaVanLeyesDoQuierenReyes_Autografo_2` | LANINI | MESA | 74 | 43/74 (58%) | 3.66 | MESA (43), AGUADOELVIEJO (5), QUINONES (2), LICENCIADOROJAS (1), TAMAYO (1) |
| medium | `LOPE_FortunaMerecida_Parma` | LOPE | BELMONTE | 58 | 42/58 (72%) | 3.62 | BELMONTE (42), VERATASSIS (4), LEIVARAMIREZ (4), VALDIVIELSO (2), VIDALYSALVADOR (2) |
| medium | `CALDERON_Teatromundo` | CALDERON | CARVAJAL | 44 | 35/44 (80%) | 3.61 | CARVAJAL (35), LORENZANA (6), QUEVEDO (1), HOZYMOTA (1), CERVANTES (1) |
| medium | `DELAHOZ_CarlosVsobreTunez` | HOZYMOTA | CASTROYSALAZAR | 58 | 38/58 (66%) | 3.58 | CASTROYSALAZAR (38), GILENRIQUEZ (13), CANIZARES (5), LICENCIADOROJAS (1), LANINI (1) |
| medium | `CALDERON_Pleitomatrimonial_Pelayo` | CALDERON | CARVAJAL | 52 | 34/52 (65%) | 3.56 | CARVAJAL (34), LORENZANA (14), CERVANTES (2), CECILIANACIMIENTO (1), GILENRIQUEZ (1) |
| medium | `AMESCUA_VidaYMuerteDeSanLazaro` | AMESCUA | SANDOVAL | 66 | 53/66 (80%) | 3.49 | SANDOVAL (53), REMON (4), LEONORCUEVA (3), CERVANTES (2), ROMEROROQUE (1) |
| medium | `CALDERON_AMariaDelCorazon3` | CALDERON | MOLINAYMENDOZA | 82 | 64/82 (78%) | 3.43 | MOLINAYMENDOZA (64), VIDALYSALVADOR (4), SARAVIAYMENDOZA (3), FAJARDOYACEVEDO (2), GILENRIQUEZ (2) |
| medium | `CALDERON_LoaVenenoYLaTriaca` | CALDERON | VARGASMACHUCA | 8 | 5/8 (62%) | 3.42 | VARGASMACHUCA (5), MELO (2), CASTROYSALAZAR (1) |
| medium | `CALDERON_AcasoYElError2` | CALDERON | AVELLANEDA | 96 | 77/96 (80%) | 3.40 | AVELLANEDA (77), SANDOVAL (7), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), QUINONES (1) |
| medium | `CALDERON_PrimeroSoyYo1` | CALDERON | LEIVARAMIREZ | 40 | 23/40 (57%) | 3.38 | LEIVARAMIREZ (23), BELMONTE (7), QUEVEDO (7), VIDALYSALVADOR (2), ENRIQUEZ (1) |
| medium | `CALDERON_SemillaylacizanaLa_Hisp` | CALDERON | ROJASZORRILLA | 9 | 5/9 (56%) | 3.34 | ROJASZORRILLA (5), VIDALYSALVADOR (2), CALDERON (1), GARCIADEPRADO (1) |
| medium | `Calderon_PurgatoriodesanPatricioEl` | CALDERON | VARGAS | 140 | 79/140 (56%) | 3.33 | VARGAS (79), MEDINA (26), GONZALEZDETORRES (4), CALLE (3), MIRACLESSOTOMAYOR (1) |
| medium | `Calderon_NinadeGomezAriasLa` | CALDERON | GARCIAMARCOS | 87 | 49/87 (56%) | 3.33 | GARCIAMARCOS (49), ROMEROROQUE (13), FAJARDOYACEVEDO (11), JIMENEZSEDENO (2), GONZALEZDEBARCIA (1) |
| medium | `CALDERON_PsiquisCupido2parte` | CALDERON | CARVAJAL | 42 | 25/42 (60%) | 3.28 | CARVAJAL (25), LORENZANA (9), CERVANTES (7), BANCESCANDAMO (1) |
| medium | `CALDERON_LoaPastorFido` | CALDERON | MELO | 8 | 4/8 (50%) | 3.28 | MELO (4), VARGASMACHUCA (3), RUANO (1) |
| medium | `CALDERON_PleitoMatrimonial1` | CALDERON | AVELLANEDA | 106 | 89/106 (84%) | 3.24 | AVELLANEDA (89), VERATASSIS (6), DIAMANTE (2), VARGASMACHUCA (1), MARCHANTE (1) |
| medium | `CALDERON_PiscinayRefugioHombre` | CALDERON | VIDALYSALVADOR | 104 | 91/104 (88%) | 3.18 | VIDALYSALVADOR (91), VARGASMACHUCA (9), GONGORA (2), MELO (1) |
| medium | `CALDERON_PsiquisyCupido2_loa` | CALDERON | CARVAJAL | 11 | 6/11 (55%) | 3.16 | CARVAJAL (6), CERVANTES (3), LORENZANA (2) |
| medium | `CALDERON_VerdaderoDiosPan_Pelayo` | CALDERON | CARVAJAL | 59 | 43/59 (73%) | 3.15 | CARVAJAL (43), LORENZANA (8), CERVANTES (4), GARCIADEPRADO (2), QUEVEDO (1) |
| medium | `LOPE_tratocorteferiasMadrid` | LOPE | ROJASVILLANDRANDO | 36 | 30/36 (83%) | 3.07 | ROJASVILLANDRANDO (30), MEDINA (2), VARGAS (1), MESA (1), LICENCIADOROJAS (1) |
| medium | `ZORRILLA_QUINONES_MONTESER_DoctorBorregoEl_Atribuido` | ROJASZORRILLA | VARGASMACHUCA | 7 | 4/7 (57%) | 3.05 | VARGASMACHUCA (4), VIDALYSALVADOR (2), MARCHANTE (1) |
| low | `LANINI_ALII_VidaMuerte_Autografo` | LANINI | GILENRIQUEZ | 86 | 29/86 (34%) | 24.27 | GILENRIQUEZ (29), MATOSFRAGOSO (19), DIAMANTE (11), AVELLANEDADELACUEVA (11), ZABALETA (7) |
| low | `LANINI_AntonioRocaLaMuerteVenturosa_Autografo` | LANINI | BELMONTE | 69 | 22/69 (32%) | 20.33 | BELMONTE (22), LANINI (18), BATRES (13), GILENRIQUEZ (3), ROJASZORRILLA (2) |
| low | `Belmonte_Auntiemporeyyvasallo` | BELMONTE | VARGAS | 132 | 42/132 (32%) | 17.24 | VARGAS (42), BELMONTE (26), MORETO (13), LEIVARAMIREZ (10), CALLE (10) |
| low | `Belmonte_Calderon_Zorrilla_Mejoramigoelmuerto` | BELMONTE | CALDERON | 161 | 41/161 (26%) | 13.97 | CALDERON (41), BELMONTE (31), ALARCON (29), MENESES (12), VIDALYSALVADOR (3) |
| low | `MORETO_CANCER_MATOS_HijoProdig` | MORETO | CARVAJAL | 47 | 21/47 (45%) | 12.69 | CARVAJAL (21), LORENZANA (18), REMON (5), TORRESLORENZODE (3) |
| low | `Calderon_TiaLa` | CALDERON | AVELLANEDA | 258 | 81/258 (31%) | 12.38 | AVELLANEDA (81), VIDALYSALVADOR (53), CECILIANACIMIENTO (33), CASTILLOSOLORZANO (27), ENRIQUEZ (13) |
| low | `CALDERON_MIRAAMESCUA_MONTALBAN_PolifemoCirce_Autografo` | CALDERON | PSEUDOHURTADODEMENDOZA | 171 | 37/171 (22%) | 12.28 | PSEUDOHURTADODEMENDOZA (37), MONTALBAN (34), QUINONES (30), VIDALYSALVADOR (21), AVELLANEDADELACUEVA (8) |
| low | `Calderon_JosedelasmujeresEl` | CALDERON | JIMENEZSEDENO | 67 | 32/67 (48%) | 11.39 | JIMENEZSEDENO (32), FAJARDOYACEVEDO (14), TORRESLORENZODE (2), GONZALEZDEBARCIA (1), GARCIAMARCOS (1) |
| low | `LOPE_MaestrodedanzarBritish` | LOPE | CANIZARES | 50 | 24/50 (48%) | 10.90 | CANIZARES (24), GILENRIQUEZ (20), CASTROYSALAZAR (6) |
| low | `Calderon_GuisadosLos` | CALDERON | VIDALYSALVADOR | 14 | 3/14 (21%) | 10.14 | VIDALYSALVADOR (3), CASTROYSALAZAR (2) |
| low | `Calderon_EncantosdelaculpaLos` | CALDERON | VIDALYSALVADOR | 121 | 57/121 (47%) | 10.12 | VIDALYSALVADOR (57), GONZALEZDEBARCIA (55) |
| low | `CANIZARES_ConfesadayConfesorSanJuan` | CANIZARES | LANINI | 33 | 14/33 (42%) | 9.30 | LANINI (14), GILENRIQUEZ (7), LORENZANA (6), GONZALEZDETORRES (3), CASTROYSALAZAR (2) |
| low | `Calderon_NiAmorselibradeamorAmorenamora` | CALDERON | MOLINAYMENDOZA | 79 | 26/79 (33%) | 9.26 | MOLINAYMENDOZA (26), SANDOVAL (20), JIMENEZSEDENO (7), CALLE (5), FAJARDOYACEVEDO (4) |
| low | `CANIZARES_Acualmejorconfesada` | CANIZARES | MORETO | 72 | 25/72 (35%) | 8.65 | MORETO (25), LANINI (22), VIDALYSALVADOR (13), LOPEZDELCAMPO (3), CASTROYSALAZAR (3) |
| low | `LOPE_VidaYMuerteTeresa1_Autografo` | LOPE | GARCIADEPRADO | 67 | 23/67 (34%) | 8.35 | GARCIADEPRADO (23), BELMONTE (12), VIDALYSALVADOR (8), ENRIQUEZ (8), LOPE (4) |
| low | `CALDERON_AutosSacramentalesTomoTercero` | CALDERON | GONZALEZDEBARCIA | 407 | 190/407 (47%) | 8.12 | GONZALEZDEBARCIA (190), VIDALYSALVADOR (70), PAREDES (47), MELO (26), AVELLANEDA (20) |
| low | `ROJASZORRILLA_PersilesySegismunda` | ROJASZORRILLA | MORETO | 37 | 18/37 (49%) | 8.00 | MORETO (18), LOPEZDECARDENA (9), MESA (4), DAVILAYPALOMARES (2), ROSETENINO (2) |
| low | `CALDERON_RedencionDeCautivos2` | CALDERON | MOLINAYMENDOZA | 26 | 12/26 (46%) | 7.91 | MOLINAYMENDOZA (12), GONZALEZDEBARCIA (4), BANCESCANDAMO (4), ALARCON (2), CAXESI (2) |
| low | `CALDERON_MisticaYReal_Autografo` | CALDERON | GILENRIQUEZ | 27 | 12/27 (44%) | 7.70 | GILENRIQUEZ (12), CALDERON (12), BOLEAYALVARADO (2), MARCHANTE (1) |
| low | `Calderon_autos_Novenatomo8` | CALDERON | VIDALYSALVADOR | 287 | 111/287 (39%) | 7.64 | VIDALYSALVADOR (111), CASTROYSALAZAR (48), GONZALEZDEBARCIA (46), AVELLANEDADELACUEVA (25), GONGORA (7) |
| low | `COELLO_AdulteraCastigadaLa` | COELLO | GILENRIQUEZ | 22 | 4/22 (18%) | 7.49 | GILENRIQUEZ (4), MORETO (4), CANIZARES (4), LANINI (2), PACHECO (1) |
| low | `Calderon_Bienvengasmal` | CALDERON | TORRESLORENZODE | 55 | 16/55 (29%) | 7.49 | TORRESLORENZODE (16), CASTILLOSOLORZANO (10), GARCIAMARCOS (9), GONZALEZDEBARCIA (3), ROMEROROQUE (3) |
| low | `CALDERON_TuProjimo_Autografo` | CALDERON | VILLEGASJUANBAUTISTA | 33 | 15/33 (46%) | 7.38 | VILLEGASJUANBAUTISTA (15), GILENRIQUEZ (8), CALDERON (4), BOLEAYALVARADO (2), CASTROYSALAZAR (2) |
| low | `LANINI_ReydonAlfonsoelBuenooBatalladelasNavas_British` | LANINI | CASTROYSALAZAR | 52 | 20/52 (38%) | 7.30 | CASTROYSALAZAR (20), MORETO (11), VERATASSIS (6), GILENRIQUEZ (3), LEONORCUEVA (2) |
| low | `VELEZ_AmorEnVicainoYlosCelosEnFrances` | VELEZ | BELMONTE | 59 | 24/59 (41%) | 7.25 | BELMONTE (24), ANDOSILLA (9), MOLINAYMENDOZA (6), MESA (5), ROJASZORRILLA (4) |
| low | `LOPE_Molino` | LOPE | MESA | 28 | 11/28 (39%) | 7.21 | MESA (11), RUIZALCEO (4), ROJASVILLANDRANDO (4), CUEVAYSILVA (4), PACHECO (3) |
| low | `LOPE_PortuguesaBritish` | LOPE | GILENRIQUEZ | 39 | 14/39 (36%) | 7.16 | GILENRIQUEZ (14), CANIZARES (14), CASTROYSALAZAR (8), LANINI (3) |
| low | `Calderon_DevociondelamisaLa` | CALDERON | ROMEROROQUE | 48 | 19/48 (40%) | 7.07 | ROMEROROQUE (19), GONZALEZDEBARCIA (17), AVELLANEDADELACUEVA (2), CARVAJAL (1), CANIZARES (1) |
| low | `LOPE_ComediasManuscritoBNE` | LOPE | LOPEZDECARDENA | 257 | 45/257 (18%) | 7.06 | LOPEZDECARDENA (45), LORENZANA (45), GILENRIQUEZ (38), BANCESCANDAMO (37), BARRIONUEVO (12) |
| low | `Calderon_Saberdeunavez` | CALDERON | TORRESLORENZODE | 48 | 20/48 (42%) | 6.61 | TORRESLORENZODE (20), JIMENEZSEDENO (9), GILENRIQUEZ (6), CASTROYSALAZAR (2), CLARAMONTE (1) |
| low | `MORETO_AntesMorirQuePecar` | MORETO | COELLO | 36 | 10/36 (28%) | 6.57 | COELLO (10), GONZALEZDEBARCIA (4), BANCESCANDAMO (3), PAREDES (3), FAJARDOYACEVEDO (3) |
| low | `CALDERON_AMaria_Autografo` | CALDERON | VILLEGASJUANBAUTISTA | 23 | 9/23 (39%) | 6.55 | VILLEGASJUANBAUTISTA (9), CALDERON (5), GILENRIQUEZ (4), MARCHANTE (3), SARAVIAYMENDOZA (2) |
| low | `Calderon_auto_RedenciondeCautivos3` | CALDERON | GONZALEZDEBARCIA | 38 | 16/38 (42%) | 6.47 | GONZALEZDEBARCIA (16), CANIZARES (9), CASTROYSALAZAR (4), MELO (4), ROMEROROQUE (1) |
| low | `Calderon_EspigasdeRuthAutosacramentalLa` | CALDERON | CASTROYSALAZAR | 34 | 11/34 (32%) | 6.18 | CASTROYSALAZAR (11), CANIZARES (7), MOLINAYMENDOZA (5), BOLEAYALVARADO (3), REMON (1) |
| low | `LOPE_duda_FundacionAlhambra` | LOPE | TORRESLORENZODE | 31 | 13/31 (42%) | 5.97 | TORRESLORENZODE (13), GOMEZACOSTA (6), RUIZALCEO (4), ROJASVILLANDRANDO (3), JUANDESOTO (2) |
| low | `LOPE_VidaYMuerteTeresa2_Autografo` | LOPE | BELMONTE | 33 | 8/33 (24%) | 5.94 | BELMONTE (8), LOPE (8), ENRIQUEZ (8), CORDERO (5), CASTILLOSOLORZANO (2) |
| low | `MORETO_HijoObediente` | MORETO | LEIVARAMIREZ | 104 | 34/104 (33%) | 5.94 | LEIVARAMIREZ (34), CASTILLOSOLORZANO (21), CORDERO (9), VERATASSIS (9), GILENRIQUEZ (7) |
| low | `CALDERON_AutosSacramentales` | CALDERON | CASTROYSALAZAR | 629 | 158/629 (25%) | 5.77 | CASTROYSALAZAR (158), SANDOVAL (143), MORETO (45), PAREDES (44), GONZALEZDEBARCIA (25) |
| low | `CALDERON_Arbol_mejor_fruto_auto` | CALDERON | GONZALEZDEBARCIA | 46 | 16/46 (35%) | 5.76 | GONZALEZDEBARCIA (16), CASTROYSALAZAR (15), MELO (7), VIDALYSALVADOR (2), GARCIAMARCOS (1) |
| low | `CALDERON_JosedelasmujeresEl_Hisp` | CALDERON | GARCIADEPRADO | 51 | 18/51 (35%) | 5.67 | GARCIADEPRADO (18), CALDERON (13), ROJASZORRILLA (8), VIDALYSALVADOR (2), LEIVARAMIREZ (2) |
| low | `Calderon_MisticayrealBabiloniaAutosacra` | CALDERON | GONZALEZDEBARCIA | 42 | 6/42 (14%) | 5.55 | GONZALEZDEBARCIA (6), CASTROYSALAZAR (6), ROMEROROQUE (5), GARCIAMARCOS (5), FAJARDOYACEVEDO (3) |
| low | `VALDIVIESO_ArbolDeLaGracia` | VALDIVIELSO | CUENCAYARGUELLO | 26 | 7/26 (27%) | 5.37 | CUENCAYARGUELLO (7), CASTROYSALAZAR (7), BARREDA (4), LEONORCUEVA (1), CARVAJAL (1) |
| low | `ROJAS_AlcaldeArdite` | LICENCIADOROJAS | QUINONES | 47 | 22/47 (47%) | 5.35 | QUINONES (22), FAJARDOYACEVEDO (13), CARVAJAL (2), CALLE (2), SANTATERESA (1) |
| low | `LOPE_NacimientoUrsonValentin` | LOPE | TORRESLORENZODE | 36 | 13/36 (36%) | 5.31 | TORRESLORENZODE (13), ROJASVILLANDRANDO (8), RUIZALCEO (5), PACHECO (3), GOMEZACOSTA (3) |
| low | `LOPE_Amazonas` | LOPE | FAJARDOYACEVEDO | 81 | 35/81 (43%) | 5.22 | FAJARDOYACEVEDO (35), PAREDES (14), GARCIAMARCOS (14), LEIVARAMIREZ (2), ANDOSILLA (1) |
| low | `Calderon_NuevopalaciodeRetiroAutosacram` | CALDERON | MOLINAYMENDOZA | 34 | 13/34 (38%) | 5.05 | MOLINAYMENDOZA (13), CANIZARES (6), BOLEAYALVARADO (5), CASTROYSALAZAR (2), MELO (1) |
| low | `CLARAMONTE_Araucana` | CLARAMONTE | ROJASZORRILLA | 26 | 10/26 (38%) | 5.04 | ROJASZORRILLA (10), BELMONTE (3), CAXESI (2), BATRES (1) |
| low | `SANTATERESA_PapelesCarmelitanos` | SANTATERESA | LEONORCUEVA | 373 | 100/373 (27%) | 5.01 | LEONORCUEVA (100), SANDOVAL (44), LICENCIADOROJAS (42), LOPEZDECASTRO (26), SANTATERESA (25) |
| low | `DIAMANTE_VenenopParaSi_Autografo` | DIAMANTE | GILENRIQUEZ | 73 | 29/73 (40%) | 4.96 | GILENRIQUEZ (29), LANINI (25), LICENCIADOROJAS (2), LEONORCUEVA (1), PAREDES (1) |
| low | `LOPE_AlbriciasNuestraSenoraLas` | LOPE | SALAZARYTORRES | 22 | 10/22 (46%) | 4.93 | SALAZARYTORRES (10), GONZALEZDEBARCIA (1), SANDOVAL (1), SANTATERESA (1), TAMAYO (1) |
| low | `Calderon_autos_Novenatomo10` | CALDERON | VIDALYSALVADOR | 367 | 150/367 (41%) | 4.90 | VIDALYSALVADOR (150), CANIZARES (63), CASTROYSALAZAR (35), DIAMANTE (25), GONGORA (22) |
| low | `CALDERON_AutosSacramentalesTomoSexto` | CALDERON | GONZALEZDEBARCIA | 370 | 116/370 (31%) | 4.85 | GONZALEZDEBARCIA (116), VIDALYSALVADOR (105), BELMONTE (39), ENRIQUEZ (36), CORDERO (25) |
| low | `CALDERON_MayorencantoamorEl_Hisp` | CALDERON | ROJASZORRILLA | 41 | 11/41 (27%) | 4.76 | ROJASZORRILLA (11), CALDERON (8), CARVAJAL (7), HURTADODEMENDOZA (2), LOPEZDELCAMPO (2) |
| low | `MIRAAMESCUA_EjemploMayor_Autografo` | AMESCUA | BATRES | 145 | 33/145 (23%) | 4.76 | BATRES (33), AMESCUA (25), CASTILLOSOLORZANO (15), CALDERON (12), VIDALYSALVADOR (8) |
| low | `Calderon_FaetonhijodelsolEl` | CALDERON | FAJARDOYACEVEDO | 57 | 18/57 (32%) | 4.74 | FAJARDOYACEVEDO (18), CLARAMONTE (13), ANDOSILLA (6), BELMONTE (4), CALDERON (4) |
| low | `CALDERON_PostrerDuelo_Autografo` | CALDERON | LEIVARAMIREZ | 151 | 73/151 (48%) | 4.72 | LEIVARAMIREZ (73), BATRES (23), TORRESLORENZODE (13), GARCIADEPRADO (3), ALARCON (3) |
| low | `Calderon_Tambienhaydueloenlasdamas` | CALDERON | ROMEROROQUE | 74 | 28/74 (38%) | 4.70 | ROMEROROQUE (28), GARCIAMARCOS (14), CALLE (9), MOLINAYMENDOZA (7), SANDOVAL (4) |
| low | `ENRIQUEZ_GOMEZ_CapitanChincilla` | ENRIQUEZ | PAREDES | 56 | 22/56 (39%) | 4.60 | PAREDES (22), CAXESI (10), TORRESLORENZODE (6), CARVAJAL (6), GOMEZACOSTA (2) |
| low | `VALDIVIESO_AngelDeLaGuarda` | VALDIVIELSO | ALARCON | 70 | 28/70 (40%) | 4.59 | ALARCON (28), GARCIADEPRADO (10), CONTRERAS (9), MESA (3), CARVAJAL (2) |
| low | `LOPE_Mesoncorte` | LOPE | CAXESI | 30 | 11/30 (37%) | 4.59 | CAXESI (11), TORRESLORENZODE (7), ROJASVILLANDRANDO (4), PACHECO (3), PAREDES (1) |
| low | `Calderon_SacristanmujerEl` | CALDERON | QUINONES | 16 | 6/16 (38%) | 4.56 | QUINONES (6), CECILIANACIMIENTO (1), CANIZARES (1), ANDOSILLA (1), GONZALEZDETORRES (1) |
| low | `Calderon_HornodeBabiloniaymisticayrealB` | CALDERON | GONZALEZDEBARCIA | 56 | 18/56 (32%) | 4.42 | GONZALEZDEBARCIA (18), CASTROYSALAZAR (13), VIDALYSALVADOR (5), MULSA (3), ROMEROROQUE (2) |
| low | `CALDERON_AmarYSerAmado1` | CALDERON | AVELLANEDA | 123 | 51/123 (42%) | 4.38 | AVELLANEDA (51), SANDOVAL (33), VARGASMACHUCA (17), MELO (6), CASTILLOSOLORZANO (1) |
| low | `CALDERON_DiabloMudo2` | CALDERON | VIDALYSALVADOR | 32 | 14/32 (44%) | 4.29 | VIDALYSALVADOR (14), BELMONTE (14), GONZALEZDEBARCIA (3), BANCESCANDAMO (1) |
| low | `MONTALBAN_PuertaMacarena2Parte` | MONTALBAN | SANDOVAL | 136 | 64/136 (47%) | 4.28 | SANDOVAL (64), VERATASSIS (47), VIDALYSALVADOR (2), AVELLANEDA (2), LICENCIADOROJAS (1) |
| low | `LOPE_ComoHaDeUsarseElBien` | LOPE | REMON | 45 | 19/45 (42%) | 4.25 | REMON (19), CASTILLOSOLORZANO (7), VARGASMACHUCA (4), HURTADODEMENDOZA (2), FAJARDOYACEVEDO (2) |
| low | `AVELLANEDA_QuienMeCompraEscarpines` | AVELLANEDA | ROMEROROQUE | 14 | 4/14 (29%) | 4.18 | ROMEROROQUE (4), LICENCIADOROJAS (1) |
| low | `Calderon_ToreadorElcaballerodeplazaEl` | CALDERON | VERATASSIS | 16 | 6/16 (38%) | 4.14 | VERATASSIS (6), VIDALYSALVADOR (2) |
| low | `Calderon_FaetonHijodelsolFaetonEl` | CALDERON | MORETO | 146 | 55/146 (38%) | 4.12 | MORETO (55), ROSETENINO (38), MENESES (18), ALARCON (2), VARGASMACHUCA (1) |
| low | `Calderon_DamaduendeLa` | CALDERON | MOLINAYMENDOZA | 76 | 25/76 (33%) | 4.10 | MOLINAYMENDOZA (25), LEIVARAMIREZ (15), GARCIAMARCOS (5), SANDOVAL (4), GONZALEZDEBARCIA (3) |
| low | `ALARCON_Anticristo_Parma` | ALARCON | QUEVEDO | 37 | 14/37 (38%) | 3.98 | QUEVEDO (14), LOPE (7), CARVAJAL (6), JUANDESOTO (4), CASTILLOSOLORZANO (3) |
| low | `CALDERON_MonstruoJardines_Autografo` | CALDERON | QUINONES | 131 | 49/131 (37%) | 3.94 | QUINONES (49), ROJASZORRILLA (15), BATRES (15), MORETO (14), CALDERON (10) |
| low | `Calderon_autos_Novenatomo3` | CALDERON | VIDALYSALVADOR | 288 | 84/288 (29%) | 3.89 | VIDALYSALVADOR (84), ENRIQUEZ (39), GONZALEZDEBARCIA (34), CORDERO (34), CASTROYSALAZAR (33) |
| low | `LOPE_HijoReduan` | LOPE | CALLE | 44 | 17/44 (39%) | 3.85 | CALLE (17), TORRESLORENZODE (13), SANDOVAL (5), JUANDESOTO (3), LEIVARAMIREZ (2) |
| low | `Calderon_Enlavidatodoesverdadytodomenti` | CALDERON | GARCIAMARCOS | 99 | 41/99 (41%) | 3.79 | GARCIAMARCOS (41), JIMENEZSEDENO (23), FAJARDOYACEVEDO (12), CASTROYSALAZAR (5), MOLINAYMENDOZA (2) |
| low | `Calderon_ParnasoSegundapartedeLaRabiaEl` | CALDERON | HURTADODEMENDOZA | 18 | 4/18 (22%) | 3.72 | HURTADODEMENDOZA (4), CARVAJAL (2), CASTILLOSOLORZANO (1), QUINONES (1) |
| low | `LOPE_CaballeroDelMilagro` | LOPE | DAVILAYPALOMARES | 58 | 19/58 (33%) | 3.60 | DAVILAYPALOMARES (19), LOPEZDECARDENA (14), ROJASZORRILLA (12), BARRIONUEVO (3), GARCIADEPRADO (1) |
| low | `LOPE_AmorBandolero` | LOPE | MENESES | 67 | 14/67 (21%) | 3.57 | MENESES (14), BELMONTE (10), MESA (8), ANDOSILLA (7), TORRESLORENZODE (6) |
| low | `CALDERON_FERNANDEZ_AmarYSerAmado2` | CALDERON | VIDALYSALVADOR | 367 | 113/367 (31%) | 3.56 | VIDALYSALVADOR (113), PAREDES (107), ENRIQUEZ (47), BELMONTE (38), TORRESLORENZODE (15) |
| low | `LOPE_AmarPorBurla` | LOPE | MESA | 62 | 24/62 (39%) | 3.55 | MESA (24), BELMONTE (10), ANDOSILLA (7), VILLEGASDELACRUZ (4), ENRIQUEZ (2) |
| low | `CALDERON_AutosSacramentalesAlegoricos` | CALDERON | MELO | 388 | 173/388 (45%) | 3.53 | MELO (173), VARGASMACHUCA (81), ONAVIEDMAYTORRES (69), SANDOVAL (35), LOPEZDECASTRO (11) |
| low | `LOPE_AcerodeMadrid_Parma` | LOPE | LANINI | 61 | 30/61 (49%) | 3.53 | LANINI (30), AVELLANEDA (20), VERATASSIS (7), PACHECO (1) |
| low | `Calderon_autos_Novenatomo6` | CALDERON | VIDALYSALVADOR | 240 | 72/240 (30%) | 3.43 | VIDALYSALVADOR (72), GONZALEZDEBARCIA (61), CASTROYSALAZAR (28), ROSETENINO (15), FAJARDOYACEVEDO (14) |
| low | `Calderon_HadoydivisadeLeonidoydeMarfisa` | CALDERON | ROJASZORRILLA | 78 | 18/78 (23%) | 3.43 | ROJASZORRILLA (18), ALARCON (17), LORENZANA (13), MORETO (5), CALDERON (4) |
| low | `MONTALBAN_AmantesDeTeruel_British` | MONTALBAN | BELMONTE | 119 | 45/119 (38%) | 3.42 | BELMONTE (45), ROJASZORRILLA (42), QUEVEDO (23), GALLEGOS (3), GONZALEZDEBARCIA (1) |
| low | `CALDERON_CadaUnoParaSi_Autografo` | CALDERON | QUINONES | 207 | 58/207 (28%) | 3.28 | QUINONES (58), ROJASZORRILLA (29), BELMONTE (27), JIMENEZSEDENO (16), CALDERON (14) |
| low | `Calderon_Deunacausadosefectosoamorhaced` | CALDERON | PAREDES | 32 | 7/32 (22%) | 3.17 | PAREDES (7), VARGASMACHUCA (4), FAJARDOYACEVEDO (4), CECILIANACIMIENTO (4), ROMEROROQUE (2) |
| low | `Calderon_SegundoEscipionEl` | CALDERON | VIDALYSALVADOR | 100 | 35/100 (35%) | 3.16 | VIDALYSALVADOR (35), PAREDES (27), JIMENEZSEDENO (12), LOPEZDELCAMPO (6), ALARCON (6) |
| low | `CANIZARES_AmandoBienNoSeOfenderaUnDesden_Autografo` | CANIZARES | CARVAJAL | 46 | 16/46 (35%) | 3.15 | CARVAJAL (16), LICENCIADOROJAS (10), CANIZARES (4), SANDOVAL (3), GILENRIQUEZ (2) |
| low | `Calderon_PostrerduelodeEspana` | CALDERON | LEIVARAMIREZ | 136 | 34/136 (25%) | 3.08 | LEIVARAMIREZ (34), TORRESLORENZODE (25), MORETO (18), CALDERON (13), BATRES (7) |
| low | `LOPE_MayordomodeladuquesaParma` | LOPE | VIDALYSALVADOR | 58 | 27/58 (47%) | 3.07 | VIDALYSALVADOR (27), BELMONTE (27), PAREDES (2), AVELLANEDA (1), BARRIONUEVO (1) |
| low | `CALDERON_DiadeSanBlasMadrid` | CALDERON | CASTROYSALAZAR | 59 | 19/59 (32%) | 3.07 | CASTROYSALAZAR (19), LORENZANA (14), MORETO (9), CANIZARES (9), LANINI (3) |
| low | `CALDERON_MisteriosDeLaMisa` | CALDERON | VARGASMACHUCA | 36 | 16/36 (44%) | 3.04 | VARGASMACHUCA (16), MELO (14), SANDOVAL (5), LOPEZDECASTRO (1) |
| low | `CALDERON_JardinDeFalerina_British` | CALDERON | AVELLANEDADELACUEVA | 30 | 11/30 (37%) | 3.00 | AVELLANEDADELACUEVA (11), GILENRIQUEZ (4), SANDOVAL (4), GARCIADEPRADO (3), VERATASSIS (3) |
| low | `Calderon_PlazueladeSantaCruzLa` | CALDERON | BOLEAYALVARADO | 14 | 2/14 (14%) | 2.98 | BOLEAYALVARADO (2), PACHECO (1), GARCIADEPRADO (1), FBQUIROS (1), TORRESLORENZODE (1) |
| low | `VELEZ_ALoQueObligaElSerRey` | VELEZ | FAJARDOYACEVEDO | 70 | 21/70 (30%) | 2.95 | FAJARDOYACEVEDO (21), BATRES (12), QUINONES (9), BELMONTE (7), PAREDES (4) |
| low | `CALDERON_SacroParnaso_BHM` | CALDERON | VIDALYSALVADOR | 94 | 80/94 (85%) | 2.95 | VIDALYSALVADOR (80), GONGORA (3), VARGASMACHUCA (2), GALLEGOS (1), MOLINAYMENDOZA (1) |
| low | `CALDERON_Viaticocordero_loa` | CALDERON | CARVAJAL | 8 | 7/8 (88%) | 2.94 | CARVAJAL (7), CERVANTES (1) |
| low | `CALDERON_LoaParaElAnoSantoDeRoma` | CALDERON | VIDALYSALVADOR | 25 | 19/25 (76%) | 2.91 | VIDALYSALVADOR (19), GONZALEZDEBARCIA (3), HURTADODEMENDOZA (1) |
| low | `TIRSO_SantaJuanaSegunda` | TIRSO | BATRES | 98 | 48/98 (49%) | 2.91 | BATRES (48), LEIVARAMIREZ (16), QUINONES (8), ENRIQUEZ (6), MESA (4) |
| low | `CALDERON_AndromedaYPerseo3` | CALDERON | GONGORA | 65 | 59/65 (91%) | 2.90 | GONGORA (59), VIDALYSALVADOR (2), CASTROYSALAZAR (1), VARGASMACHUCA (1), CERVANTES (1) |
| low | `CALDERON_AutosSacramentalesTomoQuinto` | CALDERON | VIDALYSALVADOR | 386 | 151/386 (39%) | 2.89 | VIDALYSALVADOR (151), PAREDES (47), ENRIQUEZ (36), GONZALEZDEBARCIA (17), GARCIADEPRADO (17) |
| low | `LOPE_MayorVirtud_Autografo` | LOPE | CERVANTES | 38 | 33/38 (87%) | 2.89 | CERVANTES (33), HURTADODEMENDOZA (4), LOPE (1) |
| low | `CALDERON_OrdenDeMelchisedech3` | CALDERON | VIDALYSALVADOR | 72 | 52/72 (72%) | 2.87 | VIDALYSALVADOR (52), VERATASSIS (7), CASTROYSALAZAR (4), VALDIVIELSO (3), MARCHANTE (1) |
| low | `Calderon_OrdenesmilitaresoPruebasdelseg` | CALDERON | LEIVARAMIREZ | 149 | 53/149 (36%) | 2.86 | LEIVARAMIREZ (53), CASTILLOSOLORZANO (27), HURTADODEMENDOZA (11), ENRIQUEZ (6), VIDALYSALVADOR (4) |
| low | `Calderon_JudasMacabeoolosMacabeos` | CALDERON | ENRIQUEZ | 70 | 34/70 (49%) | 2.85 | ENRIQUEZ (34), QUINONES (16), BELMONTE (4), VILLEGASDELACRUZ (3), CONTRERAS (1) |
| low | `Tirso_LadronesAporreados` | TIRSO | QUINONES | 8 | 2/8 (25%) | 2.84 | QUINONES (2), CALDERON (2), DIAMANTE (2), ROJASZORRILLA (1), MATOSFRAGOSO (1) |
| low | `VELEZ_AGUILAR_AgraviosPerdonadosLos` | VELEZ | GARCIAMARCOS | 68 | 43/68 (63%) | 2.83 | GARCIAMARCOS (43), FAJARDOYACEVEDO (4), VARGAS (4), VARGASMACHUCA (3), CALLE (2) |
| low | `MONTALBAN_MujerDePeribanez` | MONTALBAN | VERATASSIS | 144 | 84/144 (58%) | 2.82 | VERATASSIS (84), VIDALYSALVADOR (32), GARCIADEPRADO (15), BELMONTE (1) |
| low | `Calderon_JacaraentreunmusicoelMelladoys` | CALDERON | MOLINAYMENDOZA | 14 | 2/14 (14%) | 2.82 | MOLINAYMENDOZA (2), CASTILLOSOLORZANO (1), LEIVARAMIREZ (1) |
| low | `LOPE_NocheToledana_Parma` | LOPE | QUEVEDO | 52 | 16/52 (31%) | 2.82 | QUEVEDO (16), BELMONTE (9), BATRES (7), CARVAJAL (7), CASTILLOSOLORZANO (5) |
| low | `Calderon_DiamayordelosdiasEl` | CALDERON | GONZALEZDEBARCIA | 384 | 211/384 (55%) | 2.82 | GONZALEZDEBARCIA (211), VIDALYSALVADOR (41), GODINEZMANRIQUE (34), CORDERO (24), GARCIADEPRADO (21) |
| low | `CALDERON_TuProjimoComoATi` | CALDERON | PAREDES | 38 | 25/38 (66%) | 2.81 | PAREDES (25), TORRESLORENZODE (6), ENRIQUEZ (5), VIDALYSALVADOR (1), LANINI (1) |
| low | `CALDERON_SegundoBlason_Bayerische` | CALDERON | VIDALYSALVADOR | 221 | 96/221 (43%) | 2.81 | VIDALYSALVADOR (96), FAJARDOYACEVEDO (39), PAREDES (39), VARGASMACHUCA (25), GARCIAMARCOS (7) |
| low | `CALDERON_HornoBabilonia_loa` | CALDERON | CARVAJAL | 12 | 7/12 (58%) | 2.81 | CARVAJAL (7), LORENZANA (4), CERVANTES (1) |
| low | `Calderon_HumilidadcoronadadelasplantasL` | CALDERON | GARCIADEPRADO | 40 | 6/40 (15%) | 2.81 | GARCIADEPRADO (6), AVELLANEDADELACUEVA (4), MULSA (4), HOZYMOTA (4), CANIZARES (3) |
| low | `CALDERON_AndromedaPerseoconsuloa_Bayerische` | CALDERON | MELO | 290 | 222/290 (77%) | 2.80 | MELO (222), CASTROYSALAZAR (28), VIDALYSALVADOR (19), VARGASMACHUCA (8), GARCIAMARCOS (1) |
| low | `LOPE_AlejandroElSegundoCesarElPrimero` | LOPE | BELMONTE | 71 | 36/71 (51%) | 2.79 | BELMONTE (36), SANDOVAL (19), FAJARDOYACEVEDO (1), QUINONES (1), LEIVARAMIREZ (1) |
| low | `CALDERON_Inmunidadsagrado_loa` | CALDERON | CARVAJAL | 12 | 7/12 (58%) | 2.79 | CARVAJAL (7), LORENZANA (3), GARCIADEPRADO (1), CERVANTES (1) |
| low | `CALDERON_DiosPorRazonDeEstado4` | CALDERON | ONAVIEDMAYTORRES | 51 | 20/51 (39%) | 2.77 | ONAVIEDMAYTORRES (20), VARGASMACHUCA (16), MELO (9), SANDOVAL (5), LOPEZDECASTRO (1) |
| low | `LOPE_AcertarErrando_Parma` | LOPE | AVELLANEDA | 49 | 30/49 (61%) | 2.77 | AVELLANEDA (30), MEDINA (15), LANINI (1), REMON (1) |
| low | `LOPE_CardenalBelen_Dedicatoria_Autografo` | LOPE | QUEVEDO | 5 | 3/5 (60%) | 2.77 | QUEVEDO (3), REMON (1), ROMEROROQUE (1) |
| low | `GONGORA_JAUREGUI_poesias` | GONGORA | MEDINA | 76 | 14/76 (18%) | 2.76 | MEDINA (14), SANDOVAL (13), AVELLANEDA (13), ENRIQUEZ (9), VARGAS (4) |
| low | `CALDERON_LoaHermandaddelrefugioRAH_Autografo` | CALDERON | GILENRIQUEZ | 12 | 8/12 (67%) | 2.76 | GILENRIQUEZ (8), CALDERON (2), REMON (1), SARAVIAYMENDOZA (1) |
| low | `CALDERON_EntremesParaElAutoDeLosSuenosDeJose` | CALDERON | MELO | 15 | 7/15 (47%) | 2.76 | MELO (7), BARREDA (4), PAREDES (2), GONGORA (1), CASTROYSALAZAR (1) |
| low | `CALDERON_SacroParnaso_British` | CALDERON | GARCIADEPRADO | 55 | 24/55 (44%) | 2.76 | GARCIADEPRADO (24), CARVAJAL (11), CALDERON (6), ROJASVILLANDRANDO (5), BATRES (3) |
| low | `CALDERON_AlcaideDeSiMismo` | CALDERON | ANDOSILLA | 53 | 23/53 (43%) | 2.76 | ANDOSILLA (23), ROJASZORRILLA (10), LORENZANA (3), HURTADODEMENDOZA (2), MORETO (2) |
| low | `CALDERON_TuProjimoComoATi2` | CALDERON | JIMENEZSEDENO | 52 | 23/52 (44%) | 2.75 | JIMENEZSEDENO (23), BELMONTE (16), MOLINAYMENDOZA (4), MORETO (2), BOLEAYALVARADO (2) |
| low | `CALDERON_ApoloYClimene1` | CALDERON | SANDOVAL | 160 | 110/160 (69%) | 2.74 | SANDOVAL (110), GILENRIQUEZ (17), VERATASSIS (11), MARCHANTE (11), AVELLANEDA (3) |
| low | `CALDERON_Diamayordias_loa` | CALDERON | CARVAJAL | 11 | 7/11 (64%) | 2.73 | CARVAJAL (7), LORENZANA (2), QUEVEDO (1), CERVANTES (1) |
| low | `CALDERON_PleitoMatrimonial2` | CALDERON | AVELLANEDA | 96 | 62/96 (65%) | 2.71 | AVELLANEDA (62), SANDOVAL (17), VERATASSIS (12), AMESCUA (1), GONGORA (1) |
| low | `Calderon_FieraelrayoylapiedraLa` | CALDERON | FAJARDOYACEVEDO | 318 | 194/318 (61%) | 2.71 | FAJARDOYACEVEDO (194), MOLINAYMENDOZA (35), ROMEROROQUE (19), SANTATERESA (7), CASTILLOSOLORZANO (5) |
| low | `CALDERON_AutoDeLasPlantas` | CALDERON | FAJARDOYACEVEDO | 62 | 31/62 (50%) | 2.71 | FAJARDOYACEVEDO (31), JIMENEZSEDENO (11), AVELLANEDADELACUEVA (5), COELLO (3), LEONORCUEVA (2) |
| low | `LOPE_ArenalSevilla_Parma` | LOPE | BELMONTE | 52 | 26/52 (50%) | 2.70 | BELMONTE (26), LEIVARAMIREZ (18), VIDALYSALVADOR (3), VERATASSIS (1), ENRIQUEZ (1) |
| low | `CALDERON_PastorFido` | CALDERON | LORENZANA | 55 | 29/55 (53%) | 2.70 | LORENZANA (29), CARVAJAL (20), QUEVEDO (2), CERVANTES (2), HOZYMOTA (2) |
| low | `CALDERON_LoaVerdaderoDiosPan` | CALDERON | VARGASMACHUCA | 20 | 16/20 (80%) | 2.70 | VARGASMACHUCA (16), VIDALYSALVADOR (2) |
| low | `LOPE_AmarServirYEsperar` | LOPE | CALLE | 73 | 25/73 (34%) | 2.70 | CALLE (25), LEIVARAMIREZ (16), CASTILLOSOLORZANO (6), JIMENEZSEDENO (6), PAREDES (5) |
| low | `CALDERON_Maestrazgotoison_loa` | CALDERON | CARVAJAL | 12 | 6/12 (50%) | 2.70 | CARVAJAL (6), CERVANTES (4), LORENZANA (2) |
| low | `CALDERON_LoquehaceunManto` | CALDERON | CASTROYSALAZAR | 67 | 48/67 (72%) | 2.69 | CASTROYSALAZAR (48), MORETO (7), PAREDES (5), LANINI (3), LORENZANA (2) |
| low | `Calderon_PuentedeMantibleLa` | CALDERON | GARCIAMARCOS | 106 | 59/106 (56%) | 2.68 | GARCIAMARCOS (59), MELO (36), GONZALEZDEBARCIA (1), SANDOVAL (1) |
| low | `CALDERON_SiembraDelSenor` | CALDERON | VIDALYSALVADOR | 28 | 9/28 (32%) | 2.68 | VIDALYSALVADOR (9), PAREDES (9), GONZALEZDEBARCIA (5), TORRESLORENZODE (3), ENRIQUEZ (2) |
| low | `ENRIQUEZ_FernanMendezPintoPrimeraParte` | ENRIQUEZ | QUEVEDO | 110 | 41/110 (37%) | 2.68 | QUEVEDO (41), GARCIADEPRADO (19), QUINONES (12), ROJASZORRILLA (9), CALDERON (6) |
| low | `CALDERON_CenaDelReyBaltasar` | CALDERON | PAREDES | 30 | 16/30 (53%) | 2.67 | PAREDES (16), VIDALYSALVADOR (6), TORRESLORENZODE (3), ENRIQUEZ (2), LANINI (1) |
| low | `CALDERON_IndultoGeneral2` | CALDERON | VIDALYSALVADOR | 92 | 75/92 (82%) | 2.66 | VIDALYSALVADOR (75), GONZALEZDEBARCIA (7), MOLINAYMENDOZA (6), CASTILLOSOLORZANO (2) |
| low | `CANIZARES_Yomeentiendo` | CANIZARES | CASTROYSALAZAR | 60 | 32/60 (53%) | 2.66 | CASTROYSALAZAR (32), LORENZANA (9), MORETO (9), CANIZARES (4), LANINI (2) |
| low | `CALDERON_MisteriosDeLaMisa_British` | CALDERON | GARCIADEPRADO | 41 | 21/41 (51%) | 2.65 | GARCIADEPRADO (21), CARVAJAL (13), BATRES (2), GONGORA (1), GILENRIQUEZ (1) |
| low | `QUEVEDO_HospitaldemalcasadosEl` | QUEVEDO | QUINONES | 8 | 3/8 (38%) | 2.65 | QUINONES (3), MESA (2), HURTADODEMENDOZA (1), LEONORCUEVA (1) |
| low | `LOPE_REMON_DonJuandeAustria` | LOPE | CLARAMONTE | 55 | 21/55 (38%) | 2.64 | CLARAMONTE (21), CARVAJAL (10), MESA (6), LORENZANA (5), CAXESI (4) |
| low | `AVELLANEDA_QuienMeCompraEscarpines1` | AVELLANEDA | CASTILLOSOLORZANO | 13 | 10/13 (77%) | 2.64 | CASTILLOSOLORZANO (10), AVELLANEDA (1), VIDALYSALVADOR (1) |
| low | `Calderon_ExaltaciondelaCruzLa` | CALDERON | PAREDES | 73 | 21/73 (29%) | 2.64 | PAREDES (21), COELLO (21), CORDERO (20), JIMENEZSEDENO (3), BARREDA (2) |
| low | `LOPE_AmigoHastaLaMuerte` | LOPE | CARVAJAL | 43 | 10/43 (23%) | 2.62 | CARVAJAL (10), ROMEROROQUE (9), CASTILLOSOLORZANO (4), ROJASVILLANDRANDO (3), GARCIADEPRADO (2) |
| low | `CALDERON_AlimentosDelHombre3` | CALDERON | ONAVIEDMAYTORRES | 53 | 24/53 (45%) | 2.62 | ONAVIEDMAYTORRES (24), MELO (11), VARGASMACHUCA (9), SANDOVAL (6), LOPEZDECASTRO (3) |
| low | `LOPE_AcreedoresLos` | LOPE | VILLEGASJUANBAUTISTA | 22 | 4/22 (18%) | 2.61 | VILLEGASJUANBAUTISTA (4), MENESES (2), CAXESI (2), LOPEZDECASTRO (1), ALARCON (1) |
| low | `VALDIVIESO_AmistadEnElPeligro` | VALDIVIELSO | CASTILLOSOLORZANO | 41 | 17/41 (42%) | 2.59 | CASTILLOSOLORZANO (17), VIDALYSALVADOR (3), GARCIADEPRADO (3), CARVAJAL (2), JUANDESOTO (2) |
| low | `CALDERON_LoaAnoSantoDeRoma` | CALDERON | MELO | 7 | 7/7 (100%) | 2.59 | MELO (7) |
| low | `MONTALBAN_PedroUrdemalas` | MONTALBAN | GARCIADEPRADO | 49 | 20/49 (41%) | 2.59 | GARCIADEPRADO (20), CASTROYSALAZAR (6), MOLINAYMENDOZA (5), CARVAJAL (4), LORENZANA (4) |
| low | `TIRSO_RUIZDEALARCON_AMESCUA_CautelaContraCautela` | TIRSO | CERVANTES | 51 | 34/51 (67%) | 2.55 | CERVANTES (34), LORENZANA (4), REMON (4), HURTADODEMENDOZA (4), CARVAJAL (2) |
| low | `CALDERON_ApoloYClimene` | CALDERON | BELMONTE | 41 | 24/41 (58%) | 2.53 | BELMONTE (24), QUEVEDO (3), ROJASZORRILLA (3), BANCESCANDAMO (1), CONTRERAS (1) |
| low | `LOPE_Principeperfecto_Parma` | LOPE | BELMONTE | 57 | 39/57 (68%) | 2.53 | BELMONTE (39), VALDIVIELSO (4), VERATASSIS (3), LEIVARAMIREZ (3), SANDOVAL (2) |
| low | `Calderon_HijodelsolFaeronEl` | CALDERON | MELO | 129 | 46/129 (36%) | 2.52 | MELO (46), AVELLANEDA (43), SANDOVAL (21), GARCIAMARCOS (6), MEDINA (2) |
| low | `MONTALBAN_ComoAPadre_British` | MONTALBAN | GARCIADEPRADO | 97 | 56/97 (58%) | 2.52 | GARCIADEPRADO (56), CALDERON (18), QUINONES (8), CARVAJAL (3), ROJASZORRILLA (3) |
| low | `CALDERON_EstatuaDePrometeo` | CALDERON | GARCIADEPRADO | 138 | 83/138 (60%) | 2.50 | GARCIADEPRADO (83), MORETO (13), SARAVIAYMENDOZA (10), CANIZARES (8), AVELLANEDA (4) |
| low | `QUEVEDO_GalanFantasma` | QUEVEDO | BELMONTE | 144 | 28/144 (19%) | 2.50 | BELMONTE (28), CALDERON (20), ROJASZORRILLA (16), QUINONES (16), AMESCUA (16) |
| low | `Calderon_TresmayoresprodigiosdeAfricade` | CALDERON | MENESES | 77 | 26/77 (34%) | 2.49 | MENESES (26), ALARCON (14), BATRES (8), LORENZANA (4), ANDOSILLA (4) |
| low | `LOPE_AmanteAgradecido_Parma` | LOPE | LOPEZDECARDENA | 50 | 24/50 (48%) | 2.49 | LOPEZDECARDENA (24), AVELLANEDA (19), MESA (3), PAREDES (1), VERATASSIS (1) |
| low | `CALDERON_hombreDios_loa` | CALDERON | CARVAJAL | 12 | 6/12 (50%) | 2.48 | CARVAJAL (6), CERVANTES (3), GARCIADEPRADO (2), QUEVEDO (1) |
| low | `CERVANTES_CelosoExtremeno` | CERVANTES | TORRESLORENZODE | 72 | 21/72 (29%) | 2.47 | TORRESLORENZODE (21), CARVAJAL (16), ROMEROROQUE (15), CERVANTES (12), REMON (3) |
| low | `CALDERON_RedencionDeCautivos` | CALDERON | AVELLANEDA | 37 | 13/37 (35%) | 2.47 | AVELLANEDA (13), MELO (11), PAREDES (8), VIDALYSALVADOR (2), TORRESLORENZODE (1) |
| low | `Calderon_NuevoPalaciodelRetiroEl` | CALDERON | GONZALEZDEBARCIA | 44 | 18/44 (41%) | 2.46 | GONZALEZDEBARCIA (18), AVELLANEDADELACUEVA (12), GODINEZMANRIQUE (3), VIDALYSALVADOR (1) |
| low | `LOPE_AmarporveramarBritish` | LOPE | CARVAJAL | 108 | 50/108 (46%) | 2.46 | CARVAJAL (50), AVELLANEDADELACUEVA (26), GARCIADEPRADO (15), MORETO (11), LORENZANA (2) |
| low | `CALDERON_NoHayMasFortunaQueDios` | CALDERON | PAREDES | 34 | 14/34 (41%) | 2.46 | PAREDES (14), VIDALYSALVADOR (11), BELMONTE (5), ENRIQUEZ (2), SANDOVAL (2) |
| low | `Calderon_ParavenceraAmorquerervencerle` | CALDERON | MOLINAYMENDOZA | 72 | 19/72 (26%) | 2.45 | MOLINAYMENDOZA (19), GARCIAMARCOS (17), CASTROYSALAZAR (16), SANDOVAL (6), ROMEROROQUE (2) |
| low | `CALDERON_Maestrazgotuson` | CALDERON | LORENZANA | 55 | 24/55 (44%) | 2.45 | LORENZANA (24), CERVANTES (16), CARVAJAL (14), GILENRIQUEZ (1) |
| low | `Calderon_SemillaylacizanaAutosacramenta` | CALDERON | MOLINAYMENDOZA | 41 | 9/41 (22%) | 2.44 | MOLINAYMENDOZA (9), GONZALEZDEBARCIA (7), CASTROYSALAZAR (5), LANINI (3), SANDOVAL (2) |
| low | `CALDERON_ADiosPorRazonDeEstado2` | CALDERON | ENRIQUEZ | 40 | 33/40 (82%) | 2.43 | ENRIQUEZ (33), PAREDES (4), BANCESCANDAMO (1), CASTILLOSOLORZANO (1), GARCIAMARCOS (1) |
| low | `CALDERON_SiquisYCupido_British` | CALDERON | GONGORA | 88 | 61/88 (69%) | 2.43 | GONGORA (61), CASTILLOSOLORZANO (14), CASTROYSALAZAR (4), VIDALYSALVADOR (3), MELO (2) |
| low | `GARCES_BANCESCANDAMO_GranTriunfoDeTomiris` | GARCIADEPRADO | BELMONTE | 166 | 109/166 (66%) | 2.40 | BELMONTE (109), VIDALYSALVADOR (32), QUEVEDO (12), LEONORCUEVA (2), AMESCUA (1) |
| low | `MORETO_HijoObediente_Parma` | MORETO | GONGORA | 43 | 21/43 (49%) | 2.40 | GONGORA (21), GILENRIQUEZ (10), CASTROYSALAZAR (8), SARAVIAYMENDOZA (3), VIDALYSALVADOR (1) |
| low | `Calderon_SegundaesposaAutosacramentalLa` | CALDERON | ROMEROROQUE | 46 | 15/46 (33%) | 2.37 | ROMEROROQUE (15), GONZALEZDEBARCIA (14), CANIZARES (5), GONGORA (3), CARVAJAL (1) |
| low | `CALDERON_JardinDeFalerina` | CALDERON | PAREDES | 45 | 24/45 (53%) | 2.37 | PAREDES (24), VIDALYSALVADOR (18), BELMONTE (3) |
| low | `ROJASZORRILLA_GalanValienteDiscreto` | ROJASZORRILLA | CORDERO | 25 | 11/25 (44%) | 2.36 | CORDERO (11), BARREDA (5), GARCIAMARCOS (3), PAREDES (2), VIDALYSALVADOR (1) |
| low | `CALDERON_LepraConstantino` | CALDERON | VERATASSIS | 92 | 48/92 (52%) | 2.35 | VERATASSIS (48), SANDOVAL (20), AVELLANEDA (16), LOPE (1), PSEUDOHURTADODEMENDOZA (1) |
| low | `VELEZ_CristianisimaLis_Autografo` | VELEZ | PSEUDOHURTADODEMENDOZA | 140 | 41/140 (29%) | 2.35 | PSEUDOHURTADODEMENDOZA (41), CASTILLOSOLORZANO (38), LEIVARAMIREZ (13), LOPE (7), CONTRERAS (3) |
| low | `CALDERON_SacroPernaso` | CALDERON | VIDALYSALVADOR | 34 | 24/34 (71%) | 2.34 | VIDALYSALVADOR (24), PAREDES (2), CASTROYSALAZAR (2), CALDERON (1), MORETO (1) |
| low | `CALDERON_LoaHornoDeBabilonia` | CALDERON | MELO | 10 | 3/10 (30%) | 2.33 | MELO (3), VARGASMACHUCA (3), CASTROYSALAZAR (3), ONAVIEDMAYTORRES (1) |
| low | `CALDERON_MayorEncantoAmor_Autografo` | CALDERON | MENESES | 34 | 11/34 (32%) | 2.33 | MENESES (11), ROJASZORRILLA (8), CALDERON (4), LEIVARAMIREZ (2), BATRES (2) |
| low | `CALDERON_ValleDeLaZarzuela` | CALDERON | VIDALYSALVADOR | 32 | 16/32 (50%) | 2.32 | VIDALYSALVADOR (16), PAREDES (3), DIAMANTE (3), CALDERON (2), CORDERO (2) |
| low | `ENRIQUEZ_FernanMendezPintoSegundaParte` | ENRIQUEZ | GARCIADEPRADO | 96 | 33/96 (34%) | 2.31 | GARCIADEPRADO (33), QUINONES (13), CALDERON (12), GILENRIQUEZ (8), QUEVEDO (5) |
| low | `CALDERON_ObrerosDelSenor` | CALDERON | MOLINAYMENDOZA | 62 | 21/62 (34%) | 2.30 | MOLINAYMENDOZA (21), VIDALYSALVADOR (14), CANIZARES (5), LEIVARAMIREZ (5), HOZYMOTA (5) |
| low | `CALDERON_AutosBNF2` | CALDERON | GILENRIQUEZ | 280 | 116/280 (41%) | 2.29 | GILENRIQUEZ (116), HOZYMOTA (40), VIDALYSALVADOR (30), ROSETENINO (25), GONZALEZDEBARCIA (14) |
| low | `MONTALBAN_CaballerodelFebo_Autografo` | MONTALBAN | ENRIQUEZ | 38 | 28/38 (74%) | 2.29 | ENRIQUEZ (28), QUINONES (4), BATRES (1), REMON (1), VARGASMACHUCA (1) |
| low | `LANINI_CincoBlancas` | LANINI | CASTROYSALAZAR | 100 | 85/100 (85%) | 2.29 | CASTROYSALAZAR (85), VIDALYSALVADOR (5), JIMENEZSEDENO (3), GILENRIQUEZ (2), VERATASSIS (2) |
| low | `CALDERON_HadoYDivisa_Modena` | CALDERON | GONGORA | 36 | 15/36 (42%) | 2.28 | GONGORA (15), CALLE (10), CARVAJAL (4), GARCIADEPRADO (3), AVELLANEDADELACUEVA (2) |
| low | `CALDERON_EcoYNarciso` | CALDERON | PAREDES | 39 | 17/39 (44%) | 2.27 | PAREDES (17), CASTILLOSOLORZANO (11), ENRIQUEZ (9), GONZALEZDEBARCIA (2) |
| low | `QUEVEDO_MaridoFantasma` | QUEVEDO | MESA | 32 | 8/32 (25%) | 2.27 | MESA (8), LICENCIADOROJAS (1), AMESCUA (1), CASTILLOSOLORZANO (1), VIDALYSALVADOR (1) |
| low | `LOPE_CEPEDA_Espanolaycortesano_Parma` | LOPE | CARVAJAL | 54 | 15/54 (28%) | 2.26 | CARVAJAL (15), QUINONES (14), LOPE (13), AGUADOELVIEJO (4), CAXESI (2) |
| low | `CALDERON_UniversalRedencion` | CALDERON | PAREDES | 23 | 9/23 (39%) | 2.26 | PAREDES (9), VIDALYSALVADOR (6), GONZALEZDEBARCIA (5), TORRESLORENZODE (1), BANCESCANDAMO (1) |
| low | `ZORRILLA_AspidesDeCleopatra` | ROJASZORRILLA | CANIZARES | 106 | 41/106 (39%) | 2.24 | CANIZARES (41), ROJASZORRILLA (22), GONGORA (12), CARVAJAL (11), CAXESI (8) |
| low | `VARGAS_BELMONTE_AUnTiempoReyYVasallo` | VARGAS | BATRES | 153 | 88/153 (57%) | 2.21 | BATRES (88), QUINONES (15), GARCIADEPRADO (8), LICENCIADOROJAS (1), AMESCUA (1) |
| low | `Calderon_PostrerduelodeEspanaEl` | CALDERON | JIMENEZSEDENO | 120 | 32/120 (27%) | 2.21 | JIMENEZSEDENO (32), LEIVARAMIREZ (16), TORRESLORENZODE (16), BELMONTE (14), VIDALYSALVADOR (9) |
| low | `LOPE_AlcaideDeMadrid` | LOPE | MESA | 70 | 20/70 (29%) | 2.20 | MESA (20), TORRESLORENZODE (18), TAMAYO (8), ALARCON (8), ANDOSILLA (3) |
| low | `AMESCUA_AmorIngenioMujer` | AMESCUA | VERATASSIS | 61 | 32/61 (52%) | 2.18 | VERATASSIS (32), MORETO (12), GONGORA (4), CASTROYSALAZAR (3), LEIVARAMIREZ (2) |
| low | `Calderon_IglesiasitiadaLa` | CALDERON | GARCIAMARCOS | 34 | 12/34 (35%) | 2.18 | GARCIAMARCOS (12), PAREDES (8), ROMEROROQUE (2), CASTILLOSOLORZANO (2), FAJARDOYACEVEDO (2) |
| low | `CANIZARES_PrincipeDonCarlos` | CANIZARES | VERATASSIS | 146 | 89/146 (61%) | 2.17 | VERATASSIS (89), VIDALYSALVADOR (22), AVELLANEDA (7), AMESCUA (4), PAREDES (4) |
| low | `CALDERON_AutoSacramental_Munich` | CALDERON | MELO | 299 | 217/299 (73%) | 2.16 | MELO (217), VARGASMACHUCA (30), VIDALYSALVADOR (26), CASTROYSALAZAR (7), GARCIAMARCOS (3) |
| low | `CALDERON_ProjimocomoaTi3` | CALDERON | MORETO | 614 | 132/614 (22%) | 2.15 | MORETO (132), VIDALYSALVADOR (90), LANINI (85), TORRESLORENZODE (77), BANCESCANDAMO (43) |
| low | `CALDERON_LoaDiaMayorDeLosDias` | CALDERON | VARGASMACHUCA | 9 | 5/9 (56%) | 2.14 | VARGASMACHUCA (5), MELO (3), ONAVIEDMAYTORRES (1) |
| low | `CALDERON_LoaElViaticoCordero` | CALDERON | VARGASMACHUCA | 7 | 3/7 (43%) | 2.13 | VARGASMACHUCA (3), MELO (2), SANDOVAL (1), CASTROYSALAZAR (1) |
| low | `CANIZARES_LoQueValeSerDevoto` | CANIZARES | GONGORA | 59 | 32/59 (54%) | 2.11 | GONGORA (32), VIDALYSALVADOR (19), CERVANTES (4), CASTROYSALAZAR (2), MEDINA (1) |
| low | `CALDERON_PsiquisyCupido1_loa` | CALDERON | CARVAJAL | 9 | 7/9 (78%) | 2.10 | CARVAJAL (7), QUEVEDO (1), BANCESCANDAMO (1) |
| low | `CALDERON_LoaLosAlimentosDelHombre` | CALDERON | MELO | 9 | 7/9 (78%) | 2.10 | MELO (7), ONAVIEDMAYTORRES (2) |
| low | `CALDERON_LaberintoDelMundo` | CALDERON | DIAMANTE | 32 | 7/32 (22%) | 2.06 | DIAMANTE (7), MORETO (6), VIDALYSALVADOR (5), GARCIADEPRADO (5), CASTROYSALAZAR (3) |
| low | `CALDERON_LoaAnoSantoRomaRAH_Autografo` | CALDERON | GONGORA | 10 | 4/10 (40%) | 2.03 | GONGORA (4), CALDERON (3), GILENRIQUEZ (2), ROJASZORRILLA (1) |
| low | `CALDERON_GranPrincipeDeFez1` | CALDERON | GILENRIQUEZ | 145 | 64/145 (44%) | 2.02 | GILENRIQUEZ (64), SANDOVAL (47), SARAVIAYMENDOZA (8), CASTROYSALAZAR (7), AVELLANEDA (3) |
| low | `CALDERON_LoaElDiabloDelMudo` | CALDERON | MELO | 13 | 6/13 (46%) | 2.02 | MELO (6), ONAVIEDMAYTORRES (4), LOPEZDECASTRO (1), SANDOVAL (1) |
| low | `CALDERON_AutosBNF` | CALDERON | GILENRIQUEZ | 411 | 168/411 (41%) | 2.02 | GILENRIQUEZ (168), ROSETENINO (84), VIDALYSALVADOR (46), HOZYMOTA (41), CANIZARES (23) |
| low | `LOPE_ReinadonaMaria` | LOPE | BATRES | 89 | 44/89 (49%) | 2.02 | BATRES (44), LOPE (24), VILLEGASDELACRUZ (7), QUEVEDO (5), BELMONTE (5) |
| low | `CALDERON_PleitoMatrimonial_British` | CALDERON | SANDOVAL | 76 | 44/76 (58%) | 2.01 | SANDOVAL (44), GONGORA (11), CASTROYSALAZAR (8), VIDALYSALVADOR (6), VARGASMACHUCA (4) |
| low | `CALDERON_LoQueVaDelHombreADios1` | CALDERON | VERATASSIS | 110 | 102/110 (93%) | 2.01 | VERATASSIS (102), QUINONES (3), CERVANTES (1), MONTALBAN (1), SANDOVAL (1) |
| low | `CALDERON_MalPagadorenPajas` | CALDERON | MORETO | 62 | 17/62 (27%) | 2.00 | MORETO (17), LORENZANA (13), GONGORA (9), LOPEZDECASTRO (9), LANINI (5) |
| low | `Calderon_Manosblancasnoofenden` | CALDERON | LEIVARAMIREZ | 94 | 44/94 (47%) | 2.00 | LEIVARAMIREZ (44), BELMONTE (13), VIDALYSALVADOR (10), JIMENEZSEDENO (10), PAREDES (9) |
| low | `LOPE_atribuido_SordosLos_Hispanic` | LOPE | VIDALYSALVADOR | 12 | 5/12 (42%) | 2.00 | VIDALYSALVADOR (5), GILENRIQUEZ (1), GARCIADEPRADO (1), PACHECO (1), CERVANTES (1) |
| low | `CALDERON_Lamayorfineza` | CALDERON | MORETO | 56 | 30/56 (54%) | 1.99 | MORETO (30), GILENRIQUEZ (6), LORENZANA (4), CANIZARES (4), CAXESI (3) |
| low | `Calderon_VidaessuenoLa` | CALDERON | ONAVIEDMAYTORRES | 29 | 15/29 (52%) | 1.98 | ONAVIEDMAYTORRES (15), PAREDES (6), TORRESLORENZODE (3), LANINI (2), GONZALEZDEBARCIA (1) |
| low | `CALDERON_ADiosPorRazonDeEstado10` | CALDERON | VIDALYSALVADOR | 93 | 54/93 (58%) | 1.98 | VIDALYSALVADOR (54), MOLINAYMENDOZA (16), GONGORA (4), FAJARDOYACEVEDO (4), GONZALEZDEBARCIA (4) |
| low | `CALDERON_TeatroDelMundo_British` | CALDERON | SANDOVAL | 64 | 34/64 (53%) | 1.97 | SANDOVAL (34), GONGORA (10), QUEVEDO (7), TORRESLORENZODE (6), GILENRIQUEZ (2) |
| low | `CALDERON_PintordesudeshonraEl_2` | CALDERON | CALLE | 65 | 26/65 (40%) | 1.97 | CALLE (26), GONZALEZDETORRES (19), GARCIAMARCOS (5), SARAVIAYMENDOZA (5), LANINI (3) |
| low | `GARCES_MasDichosoEnSuPatria` | GARCIADEPRADO | SANDOVAL | 39 | 14/39 (36%) | 1.96 | SANDOVAL (14), ENRIQUEZ (5), TORRESLORENZODE (5), CERVANTES (4), AVELLANEDA (3) |
| low | `CALDERON_EncantosDeLaCulpa` | CALDERON | PAREDES | 28 | 14/28 (50%) | 1.96 | PAREDES (14), VIDALYSALVADOR (6), MELO (4), AVELLANEDA (4) |
| low | `CALDERON_ZABALETA_ZORRILLA_HidalgaHermosura` | CALDERON | BELMONTE | 104 | 16/104 (15%) | 1.95 | BELMONTE (16), ROSETENINO (14), DIAMANTE (13), ROJASZORRILLA (11), CALDERON (10) |
| low | `QUEVEDO_MejorLirioFrances` | QUEVEDO | COELLO | 100 | 53/100 (53%) | 1.95 | COELLO (53), VIDALYSALVADOR (19), PAREDES (9), AVELLANEDADELACUEVA (5), GONZALEZDEBARCIA (3) |
| low | `CALDERON_DivinoOrfeo_British` | CALDERON | GARCIADEPRADO | 56 | 45/56 (80%) | 1.95 | GARCIADEPRADO (45), GONZALEZDEBARCIA (8), VIDALYSALVADOR (2), HURTADODEMENDOZA (1) |
| low | `BELMONTE_RenegadaDeValladolid_Autografo` | BELMONTE | GARCIADEPRADO | 108 | 41/108 (38%) | 1.94 | GARCIADEPRADO (41), PAREDES (20), CALLE (14), CASTILLOSOLORZANO (6), VIDALYSALVADOR (6) |
| low | `CALDERON_QueVaDelHombreADios` | CALDERON | VIDALYSALVADOR | 60 | 20/60 (33%) | 1.94 | VIDALYSALVADOR (20), MELO (15), VARGASMACHUCA (12), PAREDES (7), AVELLANEDA (4) |
| low | `VELEZ_DiegoGarciadeParedes` | VELEZ | TAMAYO | 81 | 52/81 (64%) | 1.93 | TAMAYO (52), SALAZARYTORRES (5), AGUADOELVIEJO (5), CANIZARES (4), MULSA (3) |
| low | `CALDERON_VerdaderoDiosPan2` | CALDERON | VIDALYSALVADOR | 108 | 71/108 (66%) | 1.93 | VIDALYSALVADOR (71), GONGORA (15), HURTADODEMENDOZA (13), GONZALEZDEBARCIA (5), MOLINAYMENDOZA (1) |
| low | `CALDERON_Redencioncautivos` | CALDERON | LICENCIADOROJAS | 55 | 29/55 (53%) | 1.93 | LICENCIADOROJAS (29), REMON (23), MEDINA (1), CARVAJAL (1), CECILIANACIMIENTO (1) |
| low | `LOPE_ReinaMariaCheca` | LOPE | BATRES | 108 | 42/108 (39%) | 1.92 | BATRES (42), LOPE (28), QUEVEDO (6), VILLEGASDELACRUZ (5), BELMONTE (4) |
| low | `CALDERON_Socorrogeneral` | CALDERON | CARVAJAL | 47 | 30/47 (64%) | 1.90 | CARVAJAL (30), CERVANTES (6), HOZYMOTA (5), LORENZANA (5), TORRESLORENZODE (1) |
| low | `CALDERON_aprovaticapiscina_loa` | CALDERON | CARVAJAL | 15 | 9/15 (60%) | 1.89 | CARVAJAL (9), LORENZANA (5), CERVANTES (1) |
| low | `LOPE_Alpasarelarroyo_Parma` | LOPE | AVELLANEDA | 48 | 24/48 (50%) | 1.89 | AVELLANEDA (24), PACHECO (14), LANINI (6), LORENZANA (2), VARGAS (1) |
| low | `CALDERON_HumildadCoronadaDeLasPlantas` | CALDERON | GARCIAMARCOS | 36 | 9/36 (25%) | 1.89 | GARCIAMARCOS (9), GONZALEZDEBARCIA (9), VIDALYSALVADOR (5), TORRESLORENZODE (3), PAREDES (3) |
| low | `CALDERON_Mayorazgo` | CALDERON | AMESCUA | 30 | 8/30 (27%) | 1.88 | AMESCUA (8), VIDALYSALVADOR (3), AVELLANEDA (1), DIAMANTE (1), VELEZ (1) |
| low | `CALDERON_MisticaYRealBabilonia` | CALDERON | GONGORA | 87 | 76/87 (87%) | 1.87 | GONGORA (76), SARAVIAYMENDOZA (5), CANIZARES (3), VIDALYSALVADOR (1), GILENRIQUEZ (1) |
| low | `CALDERON_LirioAzucena2_BHM` | CALDERON | VIDALYSALVADOR | 80 | 47/80 (59%) | 1.87 | VIDALYSALVADOR (47), GONGORA (16), VARGASMACHUCA (4), MOLINAYMENDOZA (3), GALLEGOS (2) |
| low | `CALDERON_PielGedeon1_BHM` | CALDERON | VIDALYSALVADOR | 90 | 56/90 (62%) | 1.87 | VIDALYSALVADOR (56), GONGORA (28), HURTADODEMENDOZA (1), VARGASMACHUCA (1), GODINEZMANRIQUE (1) |
| low | `CALDERON_Secretoavoces_2y3jorn_Hisp` | CALDERON | VIDALYSALVADOR | 54 | 24/54 (44%) | 1.86 | VIDALYSALVADOR (24), VERATASSIS (7), MORETO (5), PAREDES (4), LANINI (3) |
| low | `CALDERON_AnoSantoDeRoma` | CALDERON | ROMEROROQUE | 54 | 25/54 (46%) | 1.86 | ROMEROROQUE (25), MELO (7), CASTROYSALAZAR (4), GONZALEZDEBARCIA (3), CARVAJAL (2) |
| low | `CALDERON_OrdendeMelquisedec_Austria` | CALDERON | VIDALYSALVADOR | 85 | 28/85 (33%) | 1.85 | VIDALYSALVADOR (28), GARCIADEPRADO (24), GILENRIQUEZ (7), CANIZARES (4), SARAVIAYMENDOZA (3) |
| low | `LOPE_ConcepciondeNuestraSenora` | LOPE | ANDOSILLA | 30 | 8/30 (27%) | 1.83 | ANDOSILLA (8), MESA (6), GALLEGOS (3), BATRES (3), MENESES (3) |
| low | `CALDERON_LoaIndultoGeneral` | CALDERON | MELO | 13 | 5/13 (38%) | 1.83 | MELO (5), VARGASMACHUCA (4), SANDOVAL (2), MEDINA (1), ONAVIEDMAYTORRES (1) |
| low | `CALDERON_PsiquisCupido1parte` | CALDERON | CARVAJAL | 52 | 25/52 (48%) | 1.81 | CARVAJAL (25), CERVANTES (13), LORENZANA (12), GARCIADEPRADO (2) |
| low | `MONTALBAN_HijoDelSerafin` | MONTALBAN | GILENRIQUEZ | 88 | 27/88 (31%) | 1.79 | GILENRIQUEZ (27), CALLE (23), AVELLANEDADELACUEVA (15), VIDALYSALVADOR (3), BELMONTE (3) |
| low | `MORETO_CANCER_MATOS_AdulteraPenitente` | MORETO | CLARAMONTE | 52 | 12/52 (23%) | 1.78 | CLARAMONTE (12), ANDOSILLA (9), GARCIADEPRADO (8), MOLINAYMENDOZA (7), CANIZARES (6) |
| low | `CALDERON_Adiosrazonestado` | CALDERON | LICENCIADOROJAS | 57 | 52/57 (91%) | 1.78 | LICENCIADOROJAS (52), TORRESLORENZODE (3), LORENZANA (1), CERVANTES (1) |
| low | `CALDERON_MejorAmigoElMuerto` | CALDERON | VIDALYSALVADOR | 127 | 120/127 (94%) | 1.78 | VIDALYSALVADOR (120), CASTROYSALAZAR (4), MORETO (1), COELLO (1), PAREDES (1) |
| low | `CALDERON_AlimentosDelHombre4` | CALDERON | CANIZARES | 68 | 32/68 (47%) | 1.77 | CANIZARES (32), GILENRIQUEZ (26), VIDALYSALVADOR (5), AVELLANEDADELACUEVA (2), CASTROYSALAZAR (1) |
| low | `ROJAS_DesagraviosdelHonor` | LICENCIADOROJAS | JUANDESOTO | 6 | 1/6 (17%) | 1.76 | JUANDESOTO (1), LEIVARAMIREZ (1), QUINONES (1), CALDERON (1) |
| low | `COELLO_EsfuerzoLaDicha` | COELLO | HURTADODEMENDOZA | 25 | 21/25 (84%) | 1.76 | HURTADODEMENDOZA (21), VELEZ (1), QUINONES (1), QUEVEDO (1), LOPE (1) |
| low | `LANINI_AmorConvierteLasPiedras_Autografo` | LANINI | AVELLANEDA | 79 | 54/79 (68%) | 1.75 | AVELLANEDA (54), PAREDES (3), LANINI (3), VARGASMACHUCA (2), QUINONES (2) |
| low | `CALDERON_MisteriosDeLaMisa2` | CALDERON | GONGORA | 66 | 37/66 (56%) | 1.75 | GONGORA (37), CASTROYSALAZAR (15), CANIZARES (5), SARAVIAYMENDOZA (4), CUENCAYARGUELLO (1) |
| low | `LOPE_DesenganodelMundo` | LOPE | LORENZANA | 16 | 9/16 (56%) | 1.75 | LORENZANA (9), ROJASZORRILLA (2), BARRIONUEVO (2), REMON (2), CLARAMONTE (1) |
| low | `CALDERON_Vidasueno2parte` | CALDERON | CERVANTES | 80 | 75/80 (94%) | 1.75 | CERVANTES (75), LICENCIADOROJAS (4), GONGORA (1) |
| low | `CLARAMONTE_AFirmaDeLabios` | CLARAMONTE | MONTALBAN | 64 | 21/64 (33%) | 1.74 | MONTALBAN (21), QUINONES (16), SARAVIAYMENDOZA (7), LEIVARAMIREZ (3), GONZALEZDEBARCIA (2) |
| low | `CALDERON_EntremesFinalLosSuenosdeJoseYSuenosHayQueVerdadesSon` | CALDERON | MELO | 15 | 7/15 (47%) | 1.72 | MELO (7), CASTROYSALAZAR (6), CANIZARES (1) |
| low | `CALDERON_LoaMaestrazgoDelToison` | CALDERON | VARGASMACHUCA | 11 | 5/11 (46%) | 1.72 | VARGASMACHUCA (5), ONAVIEDMAYTORRES (3), SANDOVAL (1), LOPEZDECASTRO (1), MELO (1) |
| low | `CALDERON_ADiosPorRazonDeEstado6` | CALDERON | MORETO | 74 | 16/74 (22%) | 1.72 | MORETO (16), CALLE (14), MOLINAYMENDOZA (6), JIMENEZSEDENO (5), FAJARDOYACEVEDO (4) |
| low | `MONTALBAN_DamaAlferezBritish` | MONTALBAN | VARGAS | 96 | 62/96 (65%) | 1.72 | VARGAS (62), CUEVAYSILVA (23), LICENCIADOROJAS (4), MEDINA (2), RUIZALCEO (2) |
| low | `Calderon_ValledelazarzuelaEl` | CALDERON | GONZALEZDEBARCIA | 57 | 26/57 (46%) | 1.71 | GONZALEZDEBARCIA (26), CORDERO (20), VIDALYSALVADOR (2), GODINEZMANRIQUE (2), LICENCIADOROJAS (1) |
| low | `LOPE_FiestasSantisimoSacramento` | LOPE | GARCIAMARCOS | 117 | 36/117 (31%) | 1.70 | GARCIAMARCOS (36), CASTROYSALAZAR (22), SANDOVAL (18), VERATASSIS (10), MORETO (9) |
| low | `LOPE_Atribuido_MIRADEAMESCUA_Atribuido_LaInquisicion` | LOPE | GALLEGOS | 30 | 13/30 (43%) | 1.70 | GALLEGOS (13), CALLE (7), BELMONTE (4), HOZYMOTA (2), CERVANTES (1) |
| low | `VELEZ_NegrodelMejorAmo_Parma` | VELEZ | MIRACLESSOTOMAYOR | 50 | 19/50 (38%) | 1.69 | MIRACLESSOTOMAYOR (19), CLARAMONTE (8), LOPE (6), QUINONES (6), TAMAYO (2) |
| low | `CALDERON_CuraEnfermedad_BHM` | CALDERON | GONGORA | 98 | 72/98 (74%) | 1.67 | GONGORA (72), VIDALYSALVADOR (15), VARGASMACHUCA (7), HURTADODEMENDOZA (2), GONZALEZDEBARCIA (1) |
| low | `LANINI_QUINONES_GorronesLos_Atribuido` | LANINI | VALDIVIELSO | 5 | 1/5 (20%) | 1.66 | VALDIVIELSO (1), VARGASMACHUCA (1), VIDALYSALVADOR (1), GOMEZACOSTA (1), MARCHANTE (1) |
| low | `CALDERON_DivinaFilotea_rubrica` | CALDERON | MOLINAYMENDOZA | 97 | 40/97 (41%) | 1.66 | MOLINAYMENDOZA (40), FAJARDOYACEVEDO (35), GONZALEZDEBARCIA (11), VIDALYSALVADOR (7), GILENRIQUEZ (1) |
| low | `CALDERON_LirioYLaAzucena` | CALDERON | VIDALYSALVADOR | 36 | 15/36 (42%) | 1.65 | VIDALYSALVADOR (15), GARCIADEPRADO (11), CORDERO (5), CALDERON (4), DIAMANTE (1) |
| low | `DIAMANTE_LANINI_VallesDeSopetran` | DIAMANTE | CERVANTES | 54 | 35/54 (65%) | 1.63 | CERVANTES (35), GONGORA (12), GARCIADEPRADO (6), CASTILLOSOLORZANO (1) |
| low | `CALDERON_ArbolDelMejorFruto2` | CALDERON | MORETO | 84 | 26/84 (31%) | 1.61 | MORETO (26), CASTILLOSOLORZANO (20), LANINI (10), TORRESLORENZODE (10), AVELLANEDA (3) |
| low | `CALDERON_LasPlantas` | CALDERON | VIDALYSALVADOR | 64 | 29/64 (45%) | 1.61 | VIDALYSALVADOR (29), MOLINAYMENDOZA (12), HOZYMOTA (11), CANIZARES (5), LEIVARAMIREZ (4) |
| low | `CALDERON_AndromedaYPerseo5` | CALDERON | CASTILLOSOLORZANO | 55 | 39/55 (71%) | 1.60 | CASTILLOSOLORZANO (39), BATRES (6), VIDALYSALVADOR (4), HURTADODEMENDOZA (2), QUINONES (1) |
| low | `LOPE_Aldeguela` | LOPE | QUINONES | 81 | 40/81 (49%) | 1.59 | QUINONES (40), BATRES (8), ROJASVILLANDRANDO (7), AGUADOELVIEJO (4), MESA (3) |
| low | `CALDERON_CenaReyBaltasar_BHM` | CALDERON | VIDALYSALVADOR | 46 | 28/46 (61%) | 1.59 | VIDALYSALVADOR (28), BELMONTE (7), GARCIADEPRADO (4), CERVANTES (1), CASTILLOSOLORZANO (1) |
| low | `LOPE_CaballeroDeOlmedo1` | LOPE | TORRESLORENZODE | 86 | 47/86 (55%) | 1.58 | TORRESLORENZODE (47), GILENRIQUEZ (13), CARVAJAL (7), BELMONTE (4), SANDOVAL (3) |
| low | `CALDERON_JudasMacabeo_Hispanic` | CALDERON | SANDOVAL | 59 | 40/59 (68%) | 1.58 | SANDOVAL (40), QUEVEDO (9), BELMONTE (4), CARVAJAL (2), AVELLANEDA (1) |
| low | `CALDERON_Nuevamoneda` | CALDERON | CERVANTES | 77 | 74/77 (96%) | 1.57 | CERVANTES (74), LICENCIADOROJAS (2), VERATASSIS (1) |
| low | `VELEZ_ALoQueObligaElSerRey2` | VELEZ | ROJASZORRILLA | 117 | 38/117 (32%) | 1.57 | ROJASZORRILLA (38), GALLEGOS (15), SANDOVAL (12), LEIVARAMIREZ (9), CALLE (6) |
| low | `VELEZ_OtroDemonio` | VELEZ | MEDINA | 26 | 18/26 (69%) | 1.57 | MEDINA (18), COELLO (3), AVELLANEDA (2), PAREDES (1), LICENCIADOROJAS (1) |
| low | `AMESCUA_GalanSecreto` | AMESCUA | CASTILLOSOLORZANO | 120 | 80/120 (67%) | 1.53 | CASTILLOSOLORZANO (80), VERATASSIS (7), CALLE (5), CARVAJAL (4), BATRES (3) |
| low | `Calderon_MayormonstruodelmundoEl` | CALDERON | CASTILLOSOLORZANO | 68 | 21/68 (31%) | 1.52 | CASTILLOSOLORZANO (21), VIDALYSALVADOR (6), ALARCON (5), CAXESI (5), LANINI (5) |
| low | `CALDERON_ElPesameDeLaViuda` | CALDERON | MELO | 13 | 6/13 (46%) | 1.51 | MELO (6), CASTROYSALAZAR (3), CERVANTES (1), CANIZARES (1), REMON (1) |
| low | `CALDERON_JardinFalerina_BHM` | CALDERON | VIDALYSALVADOR | 97 | 62/97 (64%) | 1.51 | VIDALYSALVADOR (62), GONGORA (14), MOLINAYMENDOZA (8), GONZALEZDEBARCIA (8), FAJARDOYACEVEDO (1) |
| low | `CALDERON_LoaLaberintoDelMundo` | CALDERON | ONAVIEDMAYTORRES | 11 | 5/11 (46%) | 1.49 | ONAVIEDMAYTORRES (5), SANDOVAL (3), LOPEZDECASTRO (2), VARGASMACHUCA (1) |
| low | `CERVANTES_Numancia_Hisp` | CERVANTES | ENRIQUEZ | 54 | 33/54 (61%) | 1.48 | ENRIQUEZ (33), CECILIANACIMIENTO (13), QUEVEDO (4), CERVANTES (2), BATRES (2) |
| low | `HURTADODEMENDOZA_GalansindamaEl` | HURTADODEMENDOZA | CERVANTES | 66 | 39/66 (59%) | 1.47 | CERVANTES (39), CASTILLOSOLORZANO (27) |
| low | `CALDERON_ArcaDioscautivaGoliat` | CALDERON | CERVANTES | 98 | 79/98 (81%) | 1.47 | CERVANTES (79), CARVAJAL (8), LICENCIADOROJAS (6), ROJASVILLANDRANDO (2), CECILIANACIMIENTO (2) |
| low | `VALDIVIESO_Escueladivina` | VALDIVIELSO | CERVANTES | 85 | 84/85 (99%) | 1.47 | CERVANTES (84), LICENCIADOROJAS (1) |
| low | `MORETO_PoderDeLaAmistad` | MORETO | SANDOVAL | 128 | 68/128 (53%) | 1.46 | SANDOVAL (68), VERATASSIS (15), VIDALYSALVADOR (14), BELMONTE (13), VARGASMACHUCA (3) |
| low | `CALDERON_LoaMisteriosDeLaMisa` | CALDERON | SANDOVAL | 9 | 4/9 (44%) | 1.46 | SANDOVAL (4), ONAVIEDMAYTORRES (2), LOPEZDECASTRO (2), VARGASMACHUCA (1) |
| low | `COELLO_PeorEsHugallo` | COELLO | GONGORA | 50 | 27/50 (54%) | 1.46 | GONGORA (27), CARVAJAL (12), CASTROYSALAZAR (7), CANIZARES (1), GILENRIQUEZ (1) |
| low | `QUEVEDO_Refranesdelviejoceloso` | QUEVEDO | SANTATERESA | 9 | 4/9 (44%) | 1.45 | SANTATERESA (4), QUINONES (2), CASTILLOSOLORZANO (1), VIDALYSALVADOR (1) |
| low | `HURTADODEMENDOZA_Nohaycelos` | HURTADODEMENDOZA | DIAMANTE | 148 | 114/148 (77%) | 1.44 | DIAMANTE (114), CANIZARES (7), HURTADODEMENDOZA (4), GARCIADEPRADO (3), CALDERON (2) |
| low | `LOPE_SegundoDavid` | LOPE | CERVANTES | 65 | 62/65 (95%) | 1.44 | CERVANTES (62), LICENCIADOROJAS (2) |
| low | `CALDERON_VALDIVIESO_CruzmurioCristo` | CALDERON | CERVANTES | 120 | 115/120 (96%) | 1.44 | CERVANTES (115), LICENCIADOROJAS (5) |
| low | `CALDERON_RabiaPrimeraParte` | CALDERON | GARCIADEPRADO | 20 | 6/20 (30%) | 1.44 | GARCIADEPRADO (6), CONTRERAS (5), HURTADODEMENDOZA (4), CASTILLOSOLORZANO (1) |
| low | `CALDERON_HijoDelSolFaeton` | CALDERON | BATRES | 166 | 74/166 (45%) | 1.44 | BATRES (74), LEIVARAMIREZ (42), CASTILLOSOLORZANO (15), VIDALYSALVADOR (4), CERVANTES (3) |
| low | `MONTALBAN_SocorroDeCadiz` | MONTALBAN | JIMENEZSEDENO | 48 | 14/48 (29%) | 1.44 | JIMENEZSEDENO (14), PAREDES (13), CALLE (6), AVELLANEDADELACUEVA (6), TORRESLORENZODE (3) |
| low | `Calderon_Primerosoyyo` | CALDERON | ENRIQUEZ | 48 | 14/48 (29%) | 1.44 | ENRIQUEZ (14), BELMONTE (8), QUINONES (8), QUEVEDO (6), LEIVARAMIREZ (5) |
| low | `DIAMANTE_ValorNoTieneEdad1` | DIAMANTE | AVELLANEDADELACUEVA | 120 | 43/120 (36%) | 1.43 | AVELLANEDADELACUEVA (43), GODINEZMANRIQUE (23), JIMENEZSEDENO (16), FAJARDOYACEVEDO (9), ALARCON (9) |
| low | `CALDERON_GranMercadoMundo_BHM` | CALDERON | VIDALYSALVADOR | 81 | 40/81 (49%) | 1.43 | VIDALYSALVADOR (40), GONZALEZDEBARCIA (18), GONGORA (16), HURTADODEMENDOZA (4), HOZYMOTA (1) |
| low | `CALDERON_HidalgaValle_BHM` | CALDERON | VIDALYSALVADOR | 74 | 62/74 (84%) | 1.43 | VIDALYSALVADOR (62), GONZALEZDEBARCIA (2), QUEVEDO (2), GALLEGOS (2), VARGASMACHUCA (2) |
| low | `CALDERON_FERNANDEZ_AmarYSerAmado` | CALDERON | GONZALEZDEBARCIA | 50 | 23/50 (46%) | 1.43 | GONZALEZDEBARCIA (23), PAREDES (8), VIDALYSALVADOR (4), FAJARDOYACEVEDO (3), CASTILLOSOLORZANO (1) |
| low | `VARGAS_CANCER_BELMONTE_ReyYVasallo` | VARGAS | HURTADODEMENDOZA | 11 | 9/11 (82%) | 1.41 | HURTADODEMENDOZA (9), CALDERON (1), GARCIADEPRADO (1) |
| low | `MORETO_ReliquiaLa` | MORETO | VARGASMACHUCA | 7 | 2/7 (29%) | 1.41 | VARGASMACHUCA (2), MARCHANTE (2), BELMONTE (1), CECILIANACIMIENTO (1), VALDIVIELSO (1) |
| low | `CALDERON_AcasoYElError` | CALDERON | LANINI | 98 | 57/98 (58%) | 1.39 | LANINI (57), CUEVAYSILVA (8), LICENCIADOROJAS (8), SANDOVAL (7), AVELLANEDA (4) |
| low | `CALDERON_AutosManuscritos` | CALDERON | TORRESLORENZODE | 253 | 81/253 (32%) | 1.38 | TORRESLORENZODE (81), ENRIQUEZ (71), PAREDES (48), VIDALYSALVADOR (14), BATRES (5) |
| low | `CALDERON_OrdenMelchisedech` | CALDERON | VIDALYSALVADOR | 90 | 72/90 (80%) | 1.38 | VIDALYSALVADOR (72), HURTADODEMENDOZA (10), GONZALEZDEBARCIA (5), CASTILLOSOLORZANO (1) |
| low | `CALDERON_AnoSantoEnRoma5` | CALDERON | GONZALEZDEBARCIA | 92 | 20/92 (22%) | 1.37 | GONZALEZDEBARCIA (20), LANINI (16), GARCIAMARCOS (14), PAREDES (11), VERATASSIS (10) |
| low | `CLARAMONTE_InfanzonDeIllescas` | CLARAMONTE | MENESES | 102 | 34/102 (33%) | 1.35 | MENESES (34), CALDERON (27), AMESCUA (8), LEIVARAMIREZ (5), MORETO (4) |
| low | `CALDERON_LoQueVaDelHombreADios` | CALDERON | GONGORA | 108 | 80/108 (74%) | 1.34 | GONGORA (80), CANIZARES (11), CASTROYSALAZAR (9), VIDALYSALVADOR (2), SARAVIAYMENDOZA (2) |
| low | `LOPE_MasPuedenCelos_Autografo` | LOPE | CASTILLOSOLORZANO | 49 | 13/49 (26%) | 1.32 | CASTILLOSOLORZANO (13), LOPE (10), QUINONES (7), CONTRERAS (4), HURTADODEMENDOZA (2) |
| low | `DIAMANTE_MagdalenaDeRoma` | DIAMANTE | AVELLANEDADELACUEVA | 104 | 28/104 (27%) | 1.31 | AVELLANEDADELACUEVA (28), GODINEZMANRIQUE (23), JIMENEZSEDENO (16), CALLE (10), FAJARDOYACEVEDO (8) |
| low | `CALDERON_AndromedaYPerseo2` | CALDERON | MOLINAYMENDOZA | 28 | 8/28 (29%) | 1.31 | MOLINAYMENDOZA (8), GARCIADEPRADO (7), VIDALYSALVADOR (1), CASTILLOSOLORZANO (1), CALLE (1) |
| low | `CANIZARES_MasilustrefregonaLa` | CANIZARES | GONGORA | 64 | 26/64 (41%) | 1.31 | GONGORA (26), GARCIADEPRADO (10), HURTADODEMENDOZA (7), CANIZARES (5), CERVANTES (4) |
| low | `ROSETENINO_TodoSucedeAlReves` | ROSETENINO | HURTADODEMENDOZA | 35 | 28/35 (80%) | 1.31 | HURTADODEMENDOZA (28), GARCIADEPRADO (2), GONGORA (2), QUEVEDO (2) |
| low | `CERVANTES_ExpedienteSobreLosMeritos` | CERVANTES | CUEVAYSILVA | 112 | 42/112 (38%) | 1.29 | CUEVAYSILVA (42), MIRACLESSOTOMAYOR (27), SANTATERESA (6), HURTADODEMENDOZA (6), MESA (5) |
| low | `CALDERON_IndultogeneralEl` | CALDERON | MELO | 84 | 43/84 (51%) | 1.29 | MELO (43), VARGASMACHUCA (17), GONZALEZDETORRES (8), SARAVIAYMENDOZA (7), GARCIAMARCOS (5) |
| low | `ENRIQUEZ_MontanesaDeBurgos` | ENRIQUEZ | QUEVEDO | 91 | 34/91 (37%) | 1.29 | QUEVEDO (34), GALLEGOS (11), SANDOVAL (8), GILENRIQUEZ (6), BELMONTE (4) |
| low | `LANINI_VisperaPascua` | LANINI | CASTILLOSOLORZANO | 30 | 13/30 (43%) | 1.27 | CASTILLOSOLORZANO (13), CONTRERAS (5), MULSA (3), AMESCUA (3), HURTADODEMENDOZA (2) |
| low | `TIRSO_HuertaJuanFernandez_acto2y3` | TIRSO | GONGORA | 144 | 80/144 (56%) | 1.27 | GONGORA (80), HURTADODEMENDOZA (26), FAJARDOYACEVEDO (11), SARAVIAYMENDOZA (8), VARGASMACHUCA (5) |
| low | `CALDERON_CastigoEnTresVenganzas_British` | CALDERON | CARVAJAL | 105 | 31/105 (30%) | 1.27 | CARVAJAL (31), BATRES (28), CASTILLOSOLORZANO (19), ROJASVILLANDRANDO (7), VARGAS (4) |
| low | `COELLO_PeorEsHurgallo` | COELLO | MESA | 132 | 28/132 (21%) | 1.27 | MESA (28), LEIVARAMIREZ (20), PAREDES (20), BATRES (18), CALLE (10) |
| low | `LANINI_VallesDeSopetran` | LANINI | VIDALYSALVADOR | 112 | 57/112 (51%) | 1.26 | VIDALYSALVADOR (57), VALDIVIELSO (17), ENRIQUEZ (5), VERATASSIS (4), GARCIADEPRADO (3) |
| low | `CALDERON_PintorDeSuDeshonra1` | CALDERON | BATRES | 125 | 66/125 (53%) | 1.25 | BATRES (66), LANINI (10), LEIVARAMIREZ (8), TORRESLORENZODE (6), GARCIADEPRADO (5) |
| low | `DIAMANTE_ValorNoTieneEdad` | DIAMANTE | CASTROYSALAZAR | 117 | 67/117 (57%) | 1.22 | CASTROYSALAZAR (67), VIDALYSALVADOR (28), VERATASSIS (10), GILENRIQUEZ (7), GARCIAMARCOS (2) |
| low | `MONTALBAN_NoHayVidaComoLaHonra` | MONTALBAN | VERATASSIS | 142 | 105/142 (74%) | 1.22 | VERATASSIS (105), VIDALYSALVADOR (10), SARAVIAYMENDOZA (9), MARCHANTE (2), DIAMANTE (1) |
| low | `LOPE_Hidalgo` | LOPE | QUEVEDO | 16 | 4/16 (25%) | 1.21 | QUEVEDO (4), AMESCUA (3), VALDIVIELSO (2), LEIVARAMIREZ (1), QUINONES (1) |
| low | `CALDERON_FuegoDeDiosEnElQuererBien` | CALDERON | CERVANTES | 127 | 75/127 (59%) | 1.20 | CERVANTES (75), CASTILLOSOLORZANO (13), HURTADODEMENDOZA (8), CARVAJAL (8), ROMEROROQUE (6) |
| low | `CALDERON_CombiteGeneral` | CALDERON | ENRIQUEZ | 46 | 12/46 (26%) | 1.20 | ENRIQUEZ (12), TORRESLORENZODE (10), PAREDES (10), GARCIAMARCOS (6), CASTILLOSOLORZANO (4) |
| low | `MARCHANTE_GatoYMontera` | MARCHANTE | CONTRERAS | 14 | 7/14 (50%) | 1.20 | CONTRERAS (7), CERVANTES (3), AGUADOELVIEJO (3), SANTATERESA (1) |
| low | `MORETO_SatisfacerCallando` | MORETO | DIAMANTE | 120 | 95/120 (79%) | 1.18 | DIAMANTE (95), CANIZARES (12), GONZALEZDEBARCIA (3), HURTADODEMENDOZA (3), AMESCUA (2) |
| low | `Calderon_GranprincipedeFezdonBaltasarde` | CALDERON | MEDINA | 81 | 40/81 (49%) | 1.17 | MEDINA (40), PAREDES (8), LANINI (6), TORRESLORENZODE (6), VIDALYSALVADOR (5) |
| low | `CALDERON_Mariacorazon_loa` | CALDERON | CERVANTES | 8 | 3/8 (38%) | 1.16 | CERVANTES (3), LORENZANA (3), CARVAJAL (2) |
| low | `CALDERON_DiablomudoEl` | CALDERON | GONZALEZDETORRES | 90 | 21/90 (23%) | 1.15 | GONZALEZDETORRES (21), CALLE (18), GONZALEZDEBARCIA (16), GARCIAMARCOS (7), VIDALYSALVADOR (3) |
| low | `CANIZARES_PrincipeDonCarlos_Parma` | CANIZARES | CARVAJAL | 61 | 16/61 (26%) | 1.15 | CARVAJAL (16), GONZALEZDEBARCIA (14), GARCIADEPRADO (12), CERVANTES (9), GALLEGOS (2) |
| low | `MARCHANTE_Espejos` | MARCHANTE | AGUADOELVIEJO | 14 | 9/14 (64%) | 1.15 | AGUADOELVIEJO (9), CERVANTES (3), SANTATERESA (1), CUENCAYARGUELLO (1) |
| low | `BELMONTE_MejorAmigoElMuerto` | BELMONTE | SANDOVAL | 151 | 40/151 (26%) | 1.14 | SANDOVAL (40), GILENRIQUEZ (20), PAREDES (15), GONGORA (14), VIDALYSALVADOR (9) |
| low | `CALDERON_AnoSantoDeRoma4` | CALDERON | ENRIQUEZ | 43 | 27/43 (63%) | 1.14 | ENRIQUEZ (27), LANINI (5), TORRESLORENZODE (4), CORDERO (3), PAREDES (2) |
| low | `CALDERON_SegundoBlasonAustria` | CALDERON | HURTADODEMENDOZA | 94 | 26/94 (28%) | 1.13 | HURTADODEMENDOZA (26), VIDALYSALVADOR (24), GONZALEZDEBARCIA (22), GONGORA (12), CERVANTES (2) |
| low | `LOPE_ColoquioentresanJuanyelninojesus` | LOPE | VALDIVIELSO | 10 | 3/10 (30%) | 1.13 | VALDIVIELSO (3), AVELLANEDA (2), LOPEZDECARDENA (2), VERATASSIS (2) |
| low | `MORETO_EmpezarASerAmigos` | MORETO | GILENRIQUEZ | 252 | 75/252 (30%) | 1.13 | GILENRIQUEZ (75), MARCHANTE (58), VERATASSIS (48), VIDALYSALVADOR (47), AVELLANEDA (6) |
| low | `DIAMANTE_JoanSanchezDeTalavera` | DIAMANTE | VIDALYSALVADOR | 166 | 47/166 (28%) | 1.12 | VIDALYSALVADOR (47), VERATASSIS (21), CASTROYSALAZAR (18), GILENRIQUEZ (18), BELMONTE (8) |
| low | `CALDERON_TesoroEscondido` | CALDERON | GONGORA | 110 | 73/110 (66%) | 1.12 | GONGORA (73), VIDALYSALVADOR (21), HURTADODEMENDOZA (12), VARGASMACHUCA (1) |
| low | `CALDERON_MisticayRealBabilonia_1` | CALDERON | REMON | 61 | 33/61 (54%) | 1.11 | REMON (33), CERVANTES (18), LICENCIADOROJAS (4), MEDINA (2), SANDOVAL (1) |
| low | `CALDERON_DevocionMisa_rubrica` | CALDERON | GONGORA | 80 | 45/80 (56%) | 1.10 | GONGORA (45), CASTILLOSOLORZANO (7), CASTROYSALAZAR (4), VIDALYSALVADOR (4), HURTADODEMENDOZA (4) |
| low | `LOPE_MarquesdelasnavasEl_British` | LOPE | CASTILLOSOLORZANO | 34 | 21/34 (62%) | 1.10 | CASTILLOSOLORZANO (21), LOPEZJACINTO (3), ZABALETA (2), FAJARDOYACEVEDO (2), PSEUDOHURTADODEMENDOZA (2) |
| low | `VELEZ_PrincipeesclavoEscanderbecEl_atribuido` | VELEZ | CALLE | 108 | 21/108 (19%) | 1.10 | CALLE (21), CARVAJAL (16), RUIZALCEO (9), VARGAS (8), QUINONES (7) |
| low | `VELEZ_AbadesaDelCielo1` | VELEZ | MESA | 30 | 10/30 (33%) | 1.10 | MESA (10), AGUADOELVIEJO (3), QUINONES (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `CALDERON_IndultoGeneral1` | CALDERON | VIDALYSALVADOR | 57 | 26/57 (46%) | 1.09 | VIDALYSALVADOR (26), GONGORA (24), CERVANTES (2), GONZALEZDEBARCIA (1), GARCIADEPRADO (1) |
| low | `MARCHANTE_VirgenDeLaSalceda` | MARCHANTE | VERATASSIS | 89 | 32/89 (36%) | 1.06 | VERATASSIS (32), CASTROYSALAZAR (29), VIDALYSALVADOR (14), SANDOVAL (4), GARCIAMARCOS (2) |
| low | `CALDERON_OrdendeMelquisedec_Hisp` | CALDERON | GARCIADEPRADO | 34 | 16/34 (47%) | 1.06 | GARCIADEPRADO (16), VIDALYSALVADOR (7), ENRIQUEZ (4), QUINONES (1), HURTADODEMENDOZA (1) |
| low | `CALDERON_FuegoDeDiosEnElQuererBien1` | CALDERON | LEIVARAMIREZ | 130 | 31/130 (24%) | 1.05 | LEIVARAMIREZ (31), VIDALYSALVADOR (22), BELMONTE (22), BATRES (13), ROJASZORRILLA (8) |
| low | `CALDERON_HadoyDivisaBnF` | CALDERON | GONGORA | 157 | 72/157 (46%) | 1.05 | GONGORA (72), VIDALYSALVADOR (28), VARGASMACHUCA (24), CERVANTES (22), MELO (3) |
| low | `VIDALYSALVADOR_Disimularesvencer` | VIDALYSALVADOR | SARAVIAYMENDOZA | 140 | 55/140 (39%) | 1.04 | SARAVIAYMENDOZA (55), CASTILLOSOLORZANO (31), VERATASSIS (25), CALLE (22), GARCIAMARCOS (3) |
| low | `VALDIVIESO_LOPE_PrudenteAbigail` | VALDIVIELSO | CERVANTES | 81 | 74/81 (91%) | 1.04 | CERVANTES (74), LICENCIADOROJAS (5), GONGORA (1) |
| low | `CANIZARES_HOZYMOTA_SantoninodelaGuardia` | CANIZARES | VERATASSIS | 66 | 28/66 (42%) | 1.03 | VERATASSIS (28), GONGORA (19), MORETO (6), QUEVEDO (4), GARCIADEPRADO (3) |
| low | `CALDERON_ADiosPorRazonDeEstado5` | CALDERON | AVELLANEDADELACUEVA | 76 | 24/76 (32%) | 1.00 | AVELLANEDADELACUEVA (24), VERATASSIS (11), CALLE (10), PAREDES (6), GONGORA (5) |
| low | `LOPE_Testimoniovengado_Erfurt` | LOPE | VARGASMACHUCA | 12 | 5/12 (42%) | 1.00 | VARGASMACHUCA (5), VIDALYSALVADOR (1), GONGORA (1), FAJARDOYACEVEDO (1), HURTADODEMENDOZA (1) |
| low | `Calderon_autos_Novenatomo7` | CALDERON | HURTADODEMENDOZA | 331 | 46/331 (14%) | 0.99 | HURTADODEMENDOZA (46), PSEUDOHURTADODEMENDOZA (42), CERVANTES (41), CASTILLOSOLORZANO (37), HOZYMOTA (28) |
| low | `CANIZARES_Comedias` | CANIZARES | AVELLANEDA | 405 | 170/405 (42%) | 0.98 | AVELLANEDA (170), LEIVARAMIREZ (122), LEONORCUEVA (42), QUEVEDO (20), SANDOVAL (17) |
| low | `LOPE_CALDERON_MATOS_Ingratoagradecido_atribuido` | LOPE | ROJASVILLANDRANDO | 52 | 25/52 (48%) | 0.98 | ROJASVILLANDRANDO (25), CARVAJAL (19), VIDALYSALVADOR (2), GONGORA (1), VALDIVIELSO (1) |
| low | `CALDERON_ADiosporrazondeestado_Hispanic` | CALDERON | VIDALYSALVADOR | 41 | 18/41 (44%) | 0.98 | VIDALYSALVADOR (18), GONGORA (8), VARGASMACHUCA (5), FAJARDOYACEVEDO (2), MARCHANTE (1) |
| low | `CERVANTES_TratodeArgelEl_Hisp` | CERVANTES | QUEVEDO | 46 | 20/46 (44%) | 0.97 | QUEVEDO (20), ENRIQUEZ (20), CECILIANACIMIENTO (3), CERVANTES (1), VARGASMACHUCA (1) |
| low | `Calderon_BarbudaLa` | CALDERON | FAJARDOYACEVEDO | 16 | 2/16 (12%) | 0.97 | FAJARDOYACEVEDO (2), LICENCIADOROJAS (1), CASTILLOSOLORZANO (1), ROMEROROQUE (1), CANIZARES (1) |
| low | `CALDERON_LepraConstantino_BHM` | CALDERON | GONGORA | 94 | 34/94 (36%) | 0.97 | GONGORA (34), VIDALYSALVADOR (27), HURTADODEMENDOZA (27), VARGASMACHUCA (3), SAAVEDRAFAJARDO (2) |
| low | `CALDERON_DivinoJason` | CALDERON | CERVANTES | 77 | 59/77 (77%) | 0.97 | CERVANTES (59), LICENCIADOROJAS (18) |
| low | `CALDERON_DosestrellasdeFrancia_Pelayo` | CALDERON | CERVANTES | 77 | 59/77 (77%) | 0.97 | CERVANTES (59), LICENCIADOROJAS (18) |
| low | `LOPE_PradosdeLeonLos` | LOPE | VARGASMACHUCA | 130 | 58/130 (45%) | 0.96 | VARGASMACHUCA (58), CORDERO (39), HURTADODEMENDOZA (18), CERVANTES (7), PAREDES (4) |
| low | `CALDERON_DuelosDeAmor_British` | CALDERON | MELO | 138 | 70/138 (51%) | 0.96 | MELO (70), AVELLANEDA (25), CASTROYSALAZAR (12), LANINI (9), GONGORA (6) |
| low | `MORETO_Cercodelashembras` | MORETO | MULSA | 18 | 6/18 (33%) | 0.96 | MULSA (6), SANTATERESA (3), CONTRERAS (2), CUEVAYSILVA (2), AMESCUA (1) |
| low | `VERATASSIS_BaileDelAgradoYLaEsquivez` | VERATASSIS | ENRIQUEZ | 6 | 2/6 (33%) | 0.95 | ENRIQUEZ (2), GONZALEZDEBARCIA (2), GODINEZMANRIQUE (1), ALARCON (1) |
| low | `CALDERON_EstatuaPrometeo` | CALDERON | VIDALYSALVADOR | 188 | 35/188 (19%) | 0.93 | VIDALYSALVADOR (35), VERATASSIS (33), CASTILLOSOLORZANO (21), GARCIADEPRADO (18), VARGASMACHUCA (14) |
| low | `GONGORA_Carta2_Autografo` | GONGORA | CECILIANACIMIENTO | 1 | 1/1 (100%) | 0.92 | CECILIANACIMIENTO (1) |
| low | `CALDERON_ArcaDeDiosCautiva1` | CALDERON | GONZALEZDEBARCIA | 93 | 44/93 (47%) | 0.92 | GONZALEZDEBARCIA (44), FAJARDOYACEVEDO (23), GONGORA (14), VIDALYSALVADOR (6), GODINEZMANRIQUE (1) |
| low | `CALDERON_CadaUnoParaSi` | CALDERON | CALLE | 164 | 58/164 (35%) | 0.92 | CALLE (58), CASTILLOSOLORZANO (23), VIDALYSALVADOR (13), GARCIADEPRADO (11), TORRESLORENZODE (9) |
| low | `BELMONTE_FiarDeDios` | BELMONTE | GARCIADEPRADO | 84 | 21/84 (25%) | 0.91 | GARCIADEPRADO (21), CALDERON (14), BATRES (12), HURTADODEMENDOZA (6), AMESCUA (5) |
| low | `CALDERON_SuenosHayQueVerdadSon2` | CALDERON | FAJARDOYACEVEDO | 112 | 44/112 (39%) | 0.91 | FAJARDOYACEVEDO (44), GONZALEZDEBARCIA (35), VIDALYSALVADOR (15), GONGORA (9), VARGASMACHUCA (3) |
| low | `CANIZARES_Ponersehabitosinpruebas` | CANIZARES | CASTROYSALAZAR | 66 | 27/66 (41%) | 0.91 | CASTROYSALAZAR (27), GILENRIQUEZ (18), VERATASSIS (7), MORETO (4), CANIZARES (3) |
| low | `GONGORA_ElDoctorCarlino` | GONGORA | PACHECO | 35 | 14/35 (40%) | 0.91 | PACHECO (14), MELO (11), LORENZANA (4), TORRESLORENZODE (3), AVELLANEDADELACUEVA (1) |
| low | `LANINI_TiaYSobrina` | LANINI | QUINONES | 12 | 4/12 (33%) | 0.91 | QUINONES (4), LEIVARAMIREZ (3), SANDOVAL (2), BENAVIDES (1), LEONORCUEVA (1) |
| low | `CALDERON_VerdaderoDiosPan1` | CALDERON | HURTADODEMENDOZA | 60 | 37/60 (62%) | 0.91 | HURTADODEMENDOZA (37), CERVANTES (8), GONGORA (5), VIDALYSALVADOR (3), LOPE (2) |
| low | `CALDERON_GranCenobia` | CALDERON | GONGORA | 140 | 88/140 (63%) | 0.88 | GONGORA (88), CERVANTES (26), SARAVIAYMENDOZA (10), CASTROYSALAZAR (2), CLARAMONTE (2) |
| low | `GONGORA_FirmezasdeIsabelaLas_Hispanic` | GONGORA | CASTILLOSOLORZANO | 80 | 18/80 (22%) | 0.87 | CASTILLOSOLORZANO (18), ENRIQUEZ (14), PAREDES (11), CERVANTES (11), CECILIANACIMIENTO (7) |
| low | `CALDERON_PintorDeshonra_rubrica` | CALDERON | GONGORA | 79 | 50/79 (63%) | 0.86 | GONGORA (50), SARAVIAYMENDOZA (11), HURTADODEMENDOZA (5), VIDALYSALVADOR (4), VARGASMACHUCA (4) |
| low | `ROJASZORRILLA_PapelActorRodamonte` | ROJASZORRILLA | AVELLANEDADELACUEVA | 6 | 2/6 (33%) | 0.85 | AVELLANEDADELACUEVA (2), SANTATERESA (1), REMON (1) |
| low | `LOPE_Viajehombre` | LOPE | VARGAS | 21 | 8/21 (38%) | 0.85 | VARGAS (8), PACHECO (6), LANINI (3), TORRESLORENZODE (2), MULSA (1) |
| low | `GONGORA_DoctorCarlinoEl_Hispanic` | GONGORA | ENRIQUEZ | 35 | 11/35 (31%) | 0.85 | ENRIQUEZ (11), VIDALYSALVADOR (6), COELLO (5), TORRESLORENZODE (4), PAREDES (3) |
| low | `CALDERON_PastorFido_rubricayfirma` | CALDERON | GONGORA | 103 | 27/103 (26%) | 0.85 | GONGORA (27), GONZALEZDEBARCIA (21), FAJARDOYACEVEDO (19), VIDALYSALVADOR (15), MOLINAYMENDOZA (5) |
| low | `DIAMANTE_LANINI_ApostolValencianoSanVicenteFerrer` | DIAMANTE | VIDALYSALVADOR | 101 | 30/101 (30%) | 0.84 | VIDALYSALVADOR (30), MONTALBAN (25), BATRES (16), COELLO (8), VERATASSIS (4) |
| low | `CALDERON_CuraEnfermedad2_BHM` | CALDERON | HURTADODEMENDOZA | 68 | 33/68 (48%) | 0.83 | HURTADODEMENDOZA (33), VIDALYSALVADOR (11), GONGORA (10), LOPE (6), GONZALEZDEBARCIA (3) |
| low | `AMESCUA_MasFelizCautiverio` | AMESCUA | VARGASMACHUCA | 145 | 56/145 (39%) | 0.78 | VARGASMACHUCA (56), VIDALYSALVADOR (26), GONGORA (25), QUEVEDO (19), CASTILLOSOLORZANO (5) |
| low | `CALDERON_CuraYEnfermedad3` | CALDERON | MARCHANTE | 92 | 33/92 (36%) | 0.77 | MARCHANTE (33), SANDOVAL (30), VERATASSIS (10), VIDALYSALVADOR (3), AVELLANEDA (3) |
| low | `CALDERON_PastorFido_loa` | CALDERON | SANDOVAL | 10 | 3/10 (30%) | 0.76 | SANDOVAL (3), LOPEZDECASTRO (2), CERVANTES (2), AVELLANEDA (1), LORENZANA (1) |
| low | `AVELLANEDA_SargentoGanchillos` | AVELLANEDA | ANDOSILLA | 8 | 2/8 (25%) | 0.75 | ANDOSILLA (2), LEIVARAMIREZ (2), GARCIADEPRADO (1), SANDOVAL (1) |
| low | `CALDERON_NinaDeGomezArias` | CALDERON | VERATASSIS | 170 | 50/170 (29%) | 0.74 | VERATASSIS (50), MARCHANTE (45), SARAVIAYMENDOZA (20), VIDALYSALVADOR (19), GONGORA (7) |
| low | `MATOSFRAGOSO_DIAMANTE_GILENRIQUEZ_VaqueroEmperador` | MATOSFRAGOSO | CASTROYSALAZAR | 123 | 38/123 (31%) | 0.74 | CASTROYSALAZAR (38), VERATASSIS (30), VIDALYSALVADOR (26), GARCIAMARCOS (9), CALLE (4) |
| low | `MONTALBAN_GitanaDeMenfis` | MONTALBAN | VERATASSIS | 152 | 50/152 (33%) | 0.73 | VERATASSIS (50), GARCIADEPRADO (21), GONGORA (15), MONTALBAN (13), CASTILLOSOLORZANO (10) |
| low | `QUEVEDO_certificadoescribano` | QUEVEDO | SARAVIAYMENDOZA | 2 | 1/2 (50%) | 0.73 | SARAVIAYMENDOZA (1), PSEUDOHURTADODEMENDOZA (1) |
| low | `LOPE_HijosdeMaria_Parma` | LOPE | CERVANTES | 14 | 3/14 (21%) | 0.71 | CERVANTES (3), CORDERO (3), CUEVAYSILVA (2), HURTADODEMENDOZA (2), ENRIQUEZ (1) |
| low | `CALDERON_SerpienteDeMetal` | CALDERON | FAJARDOYACEVEDO | 114 | 36/114 (32%) | 0.70 | FAJARDOYACEVEDO (36), GONZALEZDEBARCIA (31), GONGORA (23), ROMEROROQUE (12), VIDALYSALVADOR (5) |
| low | `CALDERON_CorderoDeIsaias2` | CALDERON | GONGORA | 73 | 30/73 (41%) | 0.69 | GONGORA (30), VIDALYSALVADOR (9), CANIZARES (6), GARCIADEPRADO (6), GONZALEZDEBARCIA (4) |
| low | `HURTADODEMENDOZA_Entremes` | HURTADODEMENDOZA | CORDERO | 7 | 3/7 (43%) | 0.69 | CORDERO (3), GARCIAMARCOS (2), MELO (1), PAREDES (1) |
| low | `Calderon_RabiaLa` | CALDERON | QUINONES | 16 | 5/16 (31%) | 0.68 | QUINONES (5), CERVANTES (2), BATRES (2) |
| low | `CANIZARES_PleitodeHernanCortesconPanfilo` | CANIZARES | GILENRIQUEZ | 66 | 23/66 (35%) | 0.64 | GILENRIQUEZ (23), GONGORA (13), CASTROYSALAZAR (9), CANIZARES (5), ROJASZORRILLA (3) |
| low | `CALDERON_VILLAMAYOR_NAJERA_EcoyNarciso` | CALDERON | LICENCIADOROJAS | 97 | 64/97 (66%) | 0.62 | LICENCIADOROJAS (64), CERVANTES (28), LOPEZDECARDENA (3), ROJASVILLANDRANDO (1) |
| low | `MENESES_AlcaldeYElBorricoDelBarbero` | MENESES | ENRIQUEZ | 12 | 6/12 (50%) | 0.60 | ENRIQUEZ (6), VIDALYSALVADOR (2), QUINONES (2), ONAVIEDMAYTORRES (1) |
| low | `GALLEGOS_ValorBeldadYAficion` | GALLEGOS | GARCIADEPRADO | 41 | 8/41 (20%) | 0.60 | GARCIADEPRADO (8), VIDALYSALVADOR (7), GILENRIQUEZ (6), REMON (5), CASTROYSALAZAR (3) |
| low | `QUEVEDO_autografopoesia` | QUEVEDO | CARVAJAL | 3 | 1/3 (33%) | 0.60 | CARVAJAL (1), QUINONES (1), HURTADODEMENDOZA (1) |
| low | `BANCESCANDAMO_GranQuimicoDelMundo` | BANCESCANDAMO | MULSA | 45 | 16/45 (36%) | 0.56 | MULSA (16), TAMAYO (6), HURTADODEMENDOZA (5), SANTATERESA (4), VALDIVIELSO (4) |
| low | `HURTADODEMENDOZA_ValoryelingeniooQuererporsoloquererEl` | HURTADODEMENDOZA | BENAVIDES | 263 | 105/263 (40%) | 0.56 | BENAVIDES (105), CERVANTES (41), VARGASMACHUCA (36), ROMEROROQUE (28), SANDOVAL (22) |
| low | `MONTALBAN_SanAntonioPadua_BNP` | MONTALBAN | GALLEGOS | 9 | 7/9 (78%) | 0.55 | GALLEGOS (7), JUANDESOTO (1) |
| low | `CALDERON_Alimentos_SerpientedeMetal_PBA` | CALDERON | VIDALYSALVADOR | 290 | 112/290 (39%) | 0.53 | VIDALYSALVADOR (112), VARGASMACHUCA (77), GONGORA (39), PAREDES (11), GONZALEZDEBARCIA (5) |
| low | `CALDERON_CasaConDosPuertas` | CALDERON | GONGORA | 176 | 98/176 (56%) | 0.53 | GONGORA (98), SARAVIAYMENDOZA (19), VIDALYSALVADOR (16), GONZALEZDEBARCIA (8), CERVANTES (7) |
| low | `ZORRILLA_GranPatioDePalacio` | ROJASZORRILLA | CORDERO | 58 | 22/58 (38%) | 0.53 | CORDERO (22), ENRIQUEZ (13), COELLO (4), GONGORA (3), FAJARDOYACEVEDO (2) |
| low | `CANIZARES_AcisYGalatea` | CANIZARES | SANDOVAL | 35 | 18/35 (51%) | 0.53 | SANDOVAL (18), ENRIQUEZ (5), GILENRIQUEZ (5), MEDINA (2), CERVANTES (2) |
| low | `CALDERON_ArbolDelMejorFruto1` | CALDERON | GONZALEZDEBARCIA | 93 | 31/93 (33%) | 0.53 | GONZALEZDEBARCIA (31), VIDALYSALVADOR (23), GONGORA (16), FAJARDOYACEVEDO (15), VARGASMACHUCA (3) |
| low | `CALDERON_Serpiente_Alimentos` | CALDERON | VIDALYSALVADOR | 291 | 121/291 (42%) | 0.52 | VIDALYSALVADOR (121), VARGASMACHUCA (81), GONGORA (40), PAREDES (6), ENRIQUEZ (4) |
| low | `CALDERON_Iglesiasiatada` | CALDERON | CERVANTES | 74 | 48/74 (65%) | 0.51 | CERVANTES (48), LICENCIADOROJAS (25) |
| low | `MONTALBAN_TeagenesyClariquea` | MONTALBAN | GALLEGOS | 30 | 18/30 (60%) | 0.50 | GALLEGOS (18), LOPE (5), VELEZ (1), CASTILLOSOLORZANO (1), HERNANDEZPADILLA (1) |
| low | `MONTALBAN_DespreciarLoQueSeQuiere` | MONTALBAN | GALLEGOS | 25 | 9/25 (36%) | 0.49 | GALLEGOS (9), LOPE (4), SAAVEDRAFAJARDO (2), SANTATERESA (2), JUANDESOTO (2) |
| low | `Calderon_VisionesdelamuerteLas` | CALDERON | LEIVARAMIREZ | 16 | 2/16 (12%) | 0.48 | LEIVARAMIREZ (2), ALARCON (2), CERVANTES (1), VIDALYSALVADOR (1), CAXESI (1) |
| low | `MONTALBAN_ComoAmanteYComoHonrada` | MONTALBAN | GALLEGOS | 23 | 22/23 (96%) | 0.48 | GALLEGOS (22) |
| low | `CALDERON_MaestrazgoTuson_BHM` | CALDERON | VIDALYSALVADOR | 63 | 21/63 (33%) | 0.48 | VIDALYSALVADOR (21), HURTADODEMENDOZA (15), AMESCUA (6), GONZALEZDEBARCIA (5), LOPE (5) |
| low | `CALDERON_PleitoMatrimonial` | CALDERON | LEONORCUEVA | 124 | 63/124 (51%) | 0.48 | LEONORCUEVA (63), AVELLANEDA (28), QUINONES (12), SANDOVAL (7), DIAMANTE (1) |
| low | `COELLO_ROJAS_VELEZ_CatalanSerrallonga` | COELLO | VIDALYSALVADOR | 168 | 89/168 (53%) | 0.47 | VIDALYSALVADOR (89), SARAVIAYMENDOZA (46), VARGASMACHUCA (23), GONGORA (1), GARCIADEPRADO (1) |
| low | `HURTADODEMENDOZA_VERATASSIS_MasMereceQuienMasAma` | HURTADODEMENDOZA | AMESCUA | 184 | 83/184 (45%) | 0.47 | AMESCUA (83), CONTRERAS (36), MULSA (25), GRACIAN (9), CERVANTES (8) |
| low | `CALDERON_ArcaDeDiosCautiva2` | CALDERON | GONGORA | 59 | 27/59 (46%) | 0.45 | GONGORA (27), VIDALYSALVADOR (6), CANIZARES (5), HURTADODEMENDOZA (4), GARCIADEPRADO (4) |
| low | `CALDERON_Laberintomundo` | CALDERON | MEDINA | 52 | 17/52 (33%) | 0.44 | MEDINA (17), SANDOVAL (8), LICENCIADOROJAS (8), BENAVIDES (6), CECILIANACIMIENTO (5) |
| low | `CALDERON_VILLAMAYOR_NAJERA_EcoyNarciso2aParte` | CALDERON | LICENCIADOROJAS | 74 | 44/74 (60%) | 0.44 | LICENCIADOROJAS (44), CERVANTES (28), LOPEZDECARDENA (2) |
| low | `MONTALBAN_AmorLealtadyAmistad` | MONTALBAN | GALLEGOS | 14 | 7/14 (50%) | 0.43 | GALLEGOS (7), HURTADODEMENDOZA (2), BENAVIDES (1), JUANDESOTO (1), SAAVEDRAFAJARDO (1) |
| low | `CALDERON_FortunaDios_loa` | CALDERON | CERVANTES | 14 | 5/14 (36%) | 0.42 | CERVANTES (5), AVELLANEDA (3), LEONORCUEVA (3), LOPEZDECASTRO (2), MELO (1) |
| low | `CALDERON_BandaYLaFlor` | CALDERON | VARGASMACHUCA | 168 | 46/168 (27%) | 0.42 | VARGASMACHUCA (46), GONGORA (43), CERVANTES (16), GONZALEZDEBARCIA (13), HURTADODEMENDOZA (12) |
| low | `MONTALBAN_ValienteMasDichoso` | MONTALBAN | GALLEGOS | 36 | 21/36 (58%) | 0.41 | GALLEGOS (21), SAAVEDRAFAJARDO (3), LOPE (3), MIRACLESSOTOMAYOR (3), AGUADOELVIEJO (1) |
| low | `CALDERON_DarloTodoYNoDarNada` | CALDERON | VERATASSIS | 158 | 51/158 (32%) | 0.41 | VERATASSIS (51), GONGORA (51), MARCHANTE (24), VIDALYSALVADOR (10), SARAVIAYMENDOZA (9) |
| low | `GONGORA_autografofalso` | GONGORA | VALDIVIELSO | 2 | 2/2 (100%) | 0.39 | VALDIVIELSO (2) |
| low | `CALDERON_PastorFidoTBP` | CALDERON | AVELLANEDA | 243 | 69/243 (28%) | 0.39 | AVELLANEDA (69), LOPEZDECARDENA (50), LICENCIADOROJAS (48), VALDIVIELSO (15), LEONORCUEVA (12) |
| low | `QUEVEDO_codicilio` | QUEVEDO | ENRIQUEZ | 2 | 1/2 (50%) | 0.39 | ENRIQUEZ (1), AVELLANEDADELACUEVA (1) |
| low | `CALDERON_EscondidoYLaTapada` | CALDERON | VARGASMACHUCA | 232 | 54/232 (23%) | 0.38 | VARGASMACHUCA (54), GONZALEZDEBARCIA (44), HURTADODEMENDOZA (42), VIDALYSALVADOR (21), GODINEZMANRIQUE (17) |
| low | `LOPE_CastelvinesYMonteses` | LOPE | ANDOSILLA | 134 | 32/134 (24%) | 0.37 | ANDOSILLA (32), LEONORCUEVA (31), GALLEGOS (15), MENESES (13), LEIVARAMIREZ (11) |
| low | `CALDERON_AcasoYElError3` | CALDERON | AVELLANEDA | 45 | 18/45 (40%) | 0.36 | AVELLANEDA (18), SANTATERESA (13), LEONORCUEVA (7), SANDOVAL (4), QUINONES (1) |
| low | `LOPE_PoemaDeFelixLopeDeVegaCarpio` | LOPE | CERVANTES | 4 | 2/4 (50%) | 0.34 | CERVANTES (2), BANCESCANDAMO (1), ENRIQUEZ (1) |
| low | `MONTALBAN_GananciaPorLaMano` | MONTALBAN | GALLEGOS | 30 | 16/30 (53%) | 0.33 | GALLEGOS (16), LOPE (5), SAAVEDRAFAJARDO (2), SANTATERESA (2), JUANDESOTO (1) |
| low | `CALDERON_Venenoytriaca_loa` | CALDERON | CERVANTES | 11 | 4/11 (36%) | 0.32 | CERVANTES (4), AVELLANEDA (3), MELO (2), TORRESLORENZODE (1), LOPEZDECASTRO (1) |
| low | `ZABALETA_GUEVARA_Otrodemoniotenemos` | ZABALETA | LORENZANA | 98 | 18/98 (18%) | 0.31 | LORENZANA (18), VARGAS (14), ENRIQUEZ (12), CERVANTES (7), GONGORA (7) |
| low | `MONTALBAN_SenecadeEspana` | MONTALBAN | LOPE | 15 | 8/15 (53%) | 0.29 | LOPE (8), GALLEGOS (3), SANTATERESA (2), HURTADODEMENDOZA (1), ROJASVILLANDRANDO (1) |
| low | `MONTALBAN_ValienteNazareno` | MONTALBAN | LOPE | 27 | 11/27 (41%) | 0.29 | LOPE (11), GALLEGOS (6), SANTATERESA (2), MIRACLESSOTOMAYOR (2), HERNANDEZPADILLA (2) |
| low | `GONGORA_Carta1_Autografo` | GONGORA | CERVANTES | 1 | 1/1 (100%) | 0.29 | CERVANTES (1) |
| low | `CALDERON_Alimentoshombre` | CALDERON | MEDINA | 93 | 38/93 (41%) | 0.28 | MEDINA (38), CECILIANACIMIENTO (12), BENAVIDES (11), CERVANTES (9), SANDOVAL (7) |
| low | `MONTALBAN_FloriseldeNiquea` | MONTALBAN | LOPE | 38 | 12/38 (32%) | 0.28 | LOPE (12), GALLEGOS (12), SANTATERESA (8), SAAVEDRAFAJARDO (1), MIRACLESSOTOMAYOR (1) |
| low | `VELEZ_Melindrosa` | VELEZ | HURTADODEMENDOZA | 32 | 8/32 (25%) | 0.27 | HURTADODEMENDOZA (8), GRACIAN (5), CUEVAYSILVA (4), MULSA (3), VALDIVIELSO (3) |
| low | `CALDERON_JoseMujeres_Autografo` | CALDERON | HURTADODEMENDOZA | 118 | 27/118 (23%) | 0.26 | HURTADODEMENDOZA (27), GARCIADEPRADO (26), QUINONES (20), ROSETENINO (10), MONTALBAN (5) |
| low | `QUEVEDO_trasladotitulo` | QUEVEDO | ENRIQUEZ | 7 | 4/7 (57%) | 0.24 | ENRIQUEZ (4), CERVANTES (2), HURTADODEMENDOZA (1) |
| low | `ROJASZORRILLA_PatronaDeMadrid` | ROJASZORRILLA | CERVANTES | 86 | 22/86 (26%) | 0.21 | CERVANTES (22), CASTILLOSOLORZANO (11), MORETO (10), GONGORA (9), LEIVARAMIREZ (9) |
| low | `CALDERON_Misteriosdelamisa_loa` | CALDERON | LOPEZDECASTRO | 12 | 4/12 (33%) | 0.21 | LOPEZDECASTRO (4), CERVANTES (2), SANDOVAL (2), MELO (2), LEONORCUEVA (1) |
| low | `LOPE_autografo_archivohistoriconacional` | LOPE | VELEZ | 2 | 1/2 (50%) | 0.17 | VELEZ (1), ROJASZORRILLA (1) |
| low | `CALDERON_Laberintomundo_loa` | CALDERON | SANDOVAL | 13 | 4/13 (31%) | 0.16 | SANDOVAL (4), LOPEZDECASTRO (3), CERVANTES (3), CASTROYSALAZAR (1), LORENZANA (1) |
| low | `MONTALBAN_DeshonraHonrosa` | MONTALBAN | LOPE | 5 | 2/5 (40%) | 0.13 | LOPE (2), GALLEGOS (1), SAAVEDRAFAJARDO (1) |
| low | `LOPE_Escolasticacelosa` | LOPE | QUEVEDO | 1 | 1/1 (100%) | 0.09 | QUEVEDO (1) |
| low | `CALDERON_autografo` | CALDERON | DIAMANTE | 2 | 1/2 (50%) | 0.08 | DIAMANTE (1) |
| low | `LOPE_carta_archivohistorico` | LOPE | HURTADODEMENDOZA | 1 | 1/1 (100%) | 0.03 | HURTADODEMENDOZA (1) |

## 3. Anonymous attributions

Manuscripts whose filename indicates anonymous or mixed-author origin (ANONIMO, DESCONOCIDO, Autoresvarios, Variasmanos, etc.). The model proposed an attribution to one of the 100 trained scribes. High-tier rows are the most defensible candidate attributions.

**552 manuscripts** (high: 21, medium: 125, low: 406)

| Tier | Manuscript | Model says | Pages | Agreement | Margin | Top-5 |
|---|---|---|---:|---:|---:|---|
| high | `MHouse_NochedesanJuanCOLOR` | LORENZANA | 17 | 16/17 (94%) | 86.32 | LORENZANA (16), VARGASMACHUCA (1) |
| high | `MHouse_HonraporlamujerCOLOR` | LORENZANA | 21 | 19/21 (90%) | 76.94 | LORENZANA (19), ROMEROROQUE (1) |
| high | `Anonimo_Librodebailes` | LOPEZDELCAMPO | 187 | 154/187 (82%) | 71.87 | LOPEZDELCAMPO (154), BATRES (1) |
| high | `DESCONOCIDO_FamosotratoToledo_Parma` | CECILIANACIMIENTO | 38 | 33/38 (87%) | 31.39 | CECILIANACIMIENTO (33), BELMONTE (1), LOPE (1) |
| high | `Anonimo_RescatedelalmaAutosacramentaly` | AVELLANEDA | 219 | 208/219 (95%) | 23.94 | AVELLANEDA (208), CECILIANACIMIENTO (2), SANTATERESA (1), BARRIONUEVO (1), VIDALYSALVADOR (1) |
| high | `DESCONOCIDO_ClaraEstrellaDeAsis` | AVELLANEDA | 53 | 53/53 (100%) | 23.30 | AVELLANEDA (53) |
| high | `Anonimo_MojigangaElalcaldedePozuelopar` | VIDALYSALVADOR | 107 | 98/107 (92%) | 19.22 | VIDALYSALVADOR (98), CASTILLOSOLORZANO (2), MOLINAYMENDOZA (1), VARGASMACHUCA (1), CECILIANACIMIENTO (1) |
| high | `DESCONOCIDO_CarbonerosFrancia` | BELMONTE | 33 | 30/33 (91%) | 17.51 | BELMONTE (30), SANDOVAL (3) |
| high | `Desconocido_PolifemoCirce_acto` | PSEUDOHURTADODEMENDOZA | 38 | 37/38 (97%) | 16.39 | PSEUDOHURTADODEMENDOZA (37) |
| high | `DESCONOCIDO_AmoresDelPrincipeDeTiro` | SANDOVAL | 52 | 43/52 (83%) | 15.96 | SANDOVAL (43), BELMONTE (7) |
| high | `ANONIMO_DonAlonsoPerezdeGuzman` | LICENCIADOROJAS | 30 | 24/30 (80%) | 13.78 | LICENCIADOROJAS (24), CERVANTES (1), AVELLANEDA (1), GONGORA (1) |
| high | `Anonimo_PericoeldeUtreraoTresnoviosenu` | CARVAJAL | 20 | 16/20 (80%) | 12.79 | CARVAJAL (16), CERVANTES (1) |
| high | `MHouse_SanBasilioCOLOR` | CASTROYSALAZAR | 46 | 39/46 (85%) | 12.06 | CASTROYSALAZAR (39), BOLEAYALVARADO (4), LLOBREGATYESTEVE (1), GONZALEZDETORRES (1), CANIZARES (1) |
| high | `DESCONOCIDO_TeatroBreve` | VIDALYSALVADOR | 149 | 128/149 (86%) | 11.50 | VIDALYSALVADOR (128), GONZALEZDEBARCIA (7), PAREDES (7), MELO (3), LANINI (2) |
| high | `Anonimo_Lagaleraenecos` | MELO | 228 | 191/228 (84%) | 11.45 | MELO (191), PAREDES (26), AVELLANEDADELACUEVA (3), TORRESLORENZODE (1), CASTROYSALAZAR (1) |
| high | `DESCONOCIDO_SanPedroNolasco` | GONZALEZDEBARCIA | 41 | 40/41 (98%) | 11.37 | GONZALEZDEBARCIA (40), VIDALYSALVADOR (1) |
| high | `Autoresvarios_Codicedeautosviejos` | AVELLANEDA | 445 | 407/445 (92%) | 11.20 | AVELLANEDA (407), CUEVAYSILVA (21), LICENCIADOROJAS (9), LOPEZDECARDENA (2), BANCESCANDAMO (2) |
| high | `MHouse_SolenelnuevomundoCOLOR` | SANDOVAL | 79 | 74/79 (94%) | 10.58 | SANDOVAL (74), VERATASSIS (2), GILENRIQUEZ (2), CASTROYSALAZAR (1) |
| high | `DESCONOCIDO_VerdadYElTiempo` | VIDALYSALVADOR | 38 | 37/38 (97%) | 10.48 | VIDALYSALVADOR (37), GONZALEZDEBARCIA (1) |
| high | `DESCONOCIDO_Loa_estaciones_British` | CASTROYSALAZAR | 16 | 15/16 (94%) | 10.40 | CASTROYSALAZAR (15), GONZALEZDETORRES (1) |
| high | `ANONIMO_TeatroMenor` | VIDALYSALVADOR | 100 | 81/100 (81%) | 10.33 | VIDALYSALVADOR (81), PAREDES (7), GONZALEZDEBARCIA (5), MELO (3), LANINI (2) |
| medium | `Anonimo_PronosticosdeAlejandreLos` | SANDOVAL | 28 | 15/28 (54%) | 35.50 | SANDOVAL (15), VERATASSIS (1), AVELLANEDA (1), MEDINA (1), BARREDA (1) |
| medium | `Anonimo_BrahuleroyMaribragas` | MOLINAYMENDOZA | 9 | 6/9 (67%) | 30.77 | MOLINAYMENDOZA (6), CERVANTES (1) |
| medium | `Anonimo_HechosdelCidymuertedelreydFern` | CUEVAYSILVA | 17 | 9/17 (53%) | 27.13 | CUEVAYSILVA (9), TAMAYO (1) |
| medium | `Anonimo_Triunfoyerrordeloscelosyelamor` | CASTROYSALAZAR | 33 | 19/33 (58%) | 26.40 | CASTROYSALAZAR (19), VERATASSIS (1), PAREDES (1), VIDALYSALVADOR (1) |
| medium | `Anonimo_FuentenuevadelaReddeSanLuisLa` | CANIZARES | 8 | 4/8 (50%) | 25.35 | CANIZARES (4), GONZALEZDEBARCIA (1) |
| medium | `Anonimo_EneasdelaVirgenyprimerreydeNav` | CASTROYSALAZAR | 61 | 47/61 (77%) | 24.88 | CASTROYSALAZAR (47), SANDOVAL (4), CERVANTES (1), ROMEROROQUE (1), GONZALEZDEBARCIA (1) |
| medium | `Anonimo_VidadeJuanGuarinymilagrosdeNue` | CUEVAYSILVA | 18 | 12/18 (67%) | 23.54 | CUEVAYSILVA (12), GARCIAMARCOS (1) |
| medium | `Anonimo_CarnestolendasdeBarcelonaLas` | CASTROYSALAZAR | 36 | 27/36 (75%) | 20.54 | CASTROYSALAZAR (27), CARVAJAL (2), LOPEZDECASTRO (2), LICENCIADOROJAS (1) |
| medium | `Anonimo_ProgneyFilomena` | CUEVAYSILVA | 13 | 7/13 (54%) | 20.21 | CUEVAYSILVA (7), VIDALYSALVADOR (1) |
| medium | `Anonimo_MariaMagdalena` | AVELLANEDA | 78 | 56/78 (72%) | 15.05 | AVELLANEDA (56), BARRIONUEVO (11), CECILIANACIMIENTO (4), PAREDES (1) |
| medium | `ANONIMO_Moromartirysantos_Novena` | FAJARDOYACEVEDO | 74 | 40/74 (54%) | 14.82 | FAJARDOYACEVEDO (40), TORRESLORENZODE (11), CASTROYSALAZAR (8), ROMEROROQUE (5), VIDALYSALVADOR (2) |
| medium | `Anonimo_Loaenalabanzadeltrabajo` | QUINONES | 6 | 3/6 (50%) | 14.31 | QUINONES (3) |
| medium | `Anonimo_IndiciosylanopestedelpuertoLos` | MOLINAYMENDOZA | 8 | 4/8 (50%) | 13.56 | MOLINAYMENDOZA (4) |
| medium | `Anonimo_Rescatarsufortuna` | GARCIAMARCOS | 78 | 51/78 (65%) | 13.22 | GARCIAMARCOS (51), FAJARDOYACEVEDO (8), ROMEROROQUE (8), LICENCIADOROJAS (1), CALLE (1) |
| medium | `ANONIMO_AnilloGigesyreyLidia_Novena` | SANDOVAL | 73 | 58/73 (80%) | 13.04 | SANDOVAL (58), LANINI (3), LICENCIADOROJAS (3), GONGORA (1), FAJARDOYACEVEDO (1) |
| medium | `DESCONOCIDO_ObispoDonGonzalo` | CUEVAYSILVA | 42 | 30/42 (71%) | 12.93 | CUEVAYSILVA (30), GOMEZACOSTA (5), RUIZALCEO (3), TAMAYO (1), CASTILLOSOLORZANO (1) |
| medium | `Anonimo_ObstinadoSapricioyelrevenidoNi` | MESA | 68 | 51/68 (75%) | 12.58 | MESA (51), RUIZALCEO (3), ANDOSILLA (2), CARVAJAL (1), LEONORCUEVA (1) |
| medium | `DESCONOCIDO_NuevaCanonizadaSantaLucia` | GILENRIQUEZ | 51 | 29/51 (57%) | 12.55 | GILENRIQUEZ (29), CANIZARES (11), BOLEAYALVARADO (3), CASTROYSALAZAR (2), LANINI (2) |
| medium | `Anonimo_FamosaTeodoraalejandrinaypenit` | TORRESLORENZODE | 32 | 18/32 (56%) | 12.29 | TORRESLORENZODE (18), SANDOVAL (6), AVELLANEDA (1), ROMEROROQUE (1) |
| medium | `Anonimo_SabinoEl` | LEIVARAMIREZ | 10 | 6/10 (60%) | 12.02 | LEIVARAMIREZ (6), BANCESCANDAMO (1) |
| medium | `MHouse_ValordeMaltaCOLOR` | CASTROYSALAZAR | 45 | 35/45 (78%) | 11.99 | CASTROYSALAZAR (35), LORENZANA (9), BOLEAYALVARADO (1) |
| medium | `MHouse_FuenteovejunaCOLOR` | GILENRIQUEZ | 20 | 14/20 (70%) | 11.76 | GILENRIQUEZ (14), CANIZARES (5) |
| medium | `Anonimo_TiranoreyCorbantoCoribantoEl` | LICENCIADOROJAS | 28 | 17/28 (61%) | 11.28 | LICENCIADOROJAS (17), CUEVAYSILVA (1), SANDOVAL (1), CARVAJAL (1) |
| medium | `Anonimo_MundonovoEl` | MOLINAYMENDOZA | 11 | 6/11 (55%) | 10.90 | MOLINAYMENDOZA (6), ROMEROROQUE (1), GARCIAMARCOS (1) |
| medium | `Anonimo_Nobastaenamorlofino` | CASTROYSALAZAR | 58 | 30/58 (52%) | 10.76 | CASTROYSALAZAR (30), SANDOVAL (17), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), VERATASSIS (1) |
| medium | `Desconocido_HijocunaSevilla` | PACHECO | 47 | 32/47 (68%) | 10.62 | PACHECO (32), MEDINA (8), TORRESLORENZODE (7) |
| medium | `Anonimo_EspanolaenMilanLa` | GARCIAMARCOS | 77 | 53/77 (69%) | 10.60 | GARCIAMARCOS (53), PAREDES (10), SANDOVAL (1), MOLINAYMENDOZA (1), BELMONTE (1) |
| medium | `DESCONOCIDO_Gravarte` | MEDINA | 12 | 9/12 (75%) | 10.09 | MEDINA (9), BELMONTE (2), TORRESLORENZODE (1) |
| medium | `MHouse_OrdenyredencionCOLOR` | CASTROYSALAZAR | 49 | 28/49 (57%) | 10.07 | CASTROYSALAZAR (28), LORENZANA (18), BOLEAYALVARADO (2), LLOBREGATYESTEVE (1) |
| medium | `ANONIMO_MejorRosadeLimaLa` | VIDALYSALVADOR | 55 | 41/55 (74%) | 9.97 | VIDALYSALVADOR (41), PAREDES (13), VERATASSIS (1) |
| medium | `Anonimo_IsladelasedymartiriodeSanPedro` | CLARAMONTE | 55 | 31/55 (56%) | 9.94 | CLARAMONTE (31), ANDOSILLA (4), VILLEGASDELACRUZ (2), LEONORCUEVA (1), GONZALEZDEBARCIA (1) |
| medium | `Anonimo_GeniosLos` | CANIZARES | 8 | 5/8 (62%) | 9.74 | CANIZARES (5), FAJARDOYACEVEDO (1) |
| medium | `DESCONOCIDO_AmorPerseguidoTriunfa` | VIDALYSALVADOR | 108 | 92/108 (85%) | 9.74 | VIDALYSALVADOR (92), BELMONTE (3), GONZALEZDEBARCIA (2), LICENCIADOROJAS (1), SARAVIAYMENDOZA (1) |
| medium | `Anonimo_Clerigoycasadoauntiempo` | MOLINAYMENDOZA | 75 | 39/75 (52%) | 9.70 | MOLINAYMENDOZA (39), BELMONTE (22), CASTILLOSOLORZANO (1) |
| medium | `Anonimo_RosarioperseguidoEl` | GARCIAMARCOS | 55 | 36/55 (66%) | 9.69 | GARCIAMARCOS (36), PAREDES (4), CASTROYSALAZAR (2), LICENCIADOROJAS (1), SANDOVAL (1) |
| medium | `Anonimo_CautivadeValladolidLa` | QUEVEDO | 42 | 25/42 (60%) | 9.58 | QUEVEDO (25), ENRIQUEZ (1), ONAVIEDMAYTORRES (1) |
| medium | `Anonimo_ContiendadeCesaryPompeyoLa` | LANINI | 24 | 12/24 (50%) | 9.52 | LANINI (12), GILENRIQUEZ (7) |
| medium | `DESCONOCIDO_NapolesLiberada` | CERVANTES | 55 | 45/55 (82%) | 9.25 | CERVANTES (45), QUEVEDO (7), ENRIQUEZ (2), SANDOVAL (1) |
| medium | `Anonimo_PeluqueroEl` | RUANO | 11 | 7/11 (64%) | 9.07 | RUANO (7), LEONORCUEVA (1), GONZALEZDEBARCIA (1) |
| medium | `ANONIMO_ClerigoycasadoBritish` | GILENRIQUEZ | 119 | 92/119 (77%) | 9.05 | GILENRIQUEZ (92), CANIZARES (18), VERATASSIS (5), CASTROYSALAZAR (3), CERVANTES (1) |
| medium | `Anonimo_EstrelladelMadronalydevocionde` | FAJARDOYACEVEDO | 60 | 49/60 (82%) | 8.99 | FAJARDOYACEVEDO (49), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), LEONORCUEVA (1), PAREDES (1) |
| medium | `Desconocido_SantoAngelo` | CUEVAYSILVA | 23 | 23/23 (100%) | 8.96 | CUEVAYSILVA (23) |
| medium | `DESCONOCIDO_BastaIntentarlo` | CASTROYSALAZAR | 54 | 47/54 (87%) | 8.77 | CASTROYSALAZAR (47), BOLEAYALVARADO (5), SARAVIAYMENDOZA (1), LORENZANA (1) |
| medium | `DESCONOCIDO_HebreodeRomaEl` | CALDERON | 65 | 35/65 (54%) | 8.77 | CALDERON (35), LOPEZDELCAMPO (20), DIAMANTE (3), ENRIQUEZ (2), QUINONES (2) |
| medium | `Anonimo_RescatedeMelisendraEl` | CONTRERAS | 364 | 184/364 (50%) | 8.69 | CONTRERAS (184), CECILIANACIMIENTO (85), CUEVAYSILVA (35), GOMEZACOSTA (17), LOPEZDELCAMPO (8) |
| medium | `DESCONOCIDO_Loaalegoricadelarifa` | VIDALYSALVADOR | 15 | 14/15 (93%) | 8.38 | VIDALYSALVADOR (14) |
| medium | `MHouse_ParaisodeLauraCOLOR` | MELO | 35 | 32/35 (91%) | 8.36 | MELO (32), GONZALEZDETORRES (1), LOPEZDECASTRO (1), VARGASMACHUCA (1) |
| medium | `MHouse_NohaybiensinajenodanoCOLOR` | LORENZANA | 63 | 39/63 (62%) | 8.16 | LORENZANA (39), TORRESLORENZODE (6), VARGAS (4), MELO (3), GARCIAMARCOS (3) |
| medium | `DESCONOCIDO_SegundaMagdalena` | GILENRIQUEZ | 65 | 38/65 (58%) | 8.05 | GILENRIQUEZ (38), CASTROYSALAZAR (21), MELO (3), SANDOVAL (2), MEDINA (1) |
| medium | `ANONIMO_AtlantedelaIglesia` | SANDOVAL | 75 | 71/75 (95%) | 7.85 | SANDOVAL (71), AVELLANEDA (3) |
| medium | `Anonimo_EsperanzacumplidaLa` | COELLO | 47 | 35/47 (74%) | 7.82 | COELLO (35), VARGASMACHUCA (1), PAREDES (1) |
| medium | `ANONIMO_AustriaenJerusalen_Novena` | GILENRIQUEZ | 54 | 31/54 (57%) | 7.76 | GILENRIQUEZ (31), CASTROYSALAZAR (21), SANDOVAL (1), VERATASSIS (1) |
| medium | `MHouse_AmarporveramarCOLOR` | CLARAMONTE | 54 | 34/54 (63%) | 7.48 | CLARAMONTE (34), CARVAJAL (12), LORENZANA (3), REMON (2), ROMEROROQUE (1) |
| medium | `DESCONOCIDO_AsedioYSitioDePeniscola` | CONTRERAS | 48 | 25/48 (52%) | 7.41 | CONTRERAS (25), CECILIANACIMIENTO (9), LOPEZDELCAMPO (2), BANCESCANDAMO (1), MARCHANTE (1) |
| medium | `DESCONOCIDO_PiedadVenceAlDestino` | SANDOVAL | 4 | 3/4 (75%) | 7.15 | SANDOVAL (3), MELO (1) |
| medium | `DESCONOCIDO_EntremesMochuelo` | CARVAJAL | 4 | 3/4 (75%) | 7.10 | CARVAJAL (3), CONTRERAS (1) |
| medium | `ANONIMO_Entremes` | VIDALYSALVADOR | 13 | 12/13 (92%) | 7.03 | VIDALYSALVADOR (12), CASTROYSALAZAR (1) |
| medium | `Anonimo_RamilleteraLa` | SANDOVAL | 12 | 6/12 (50%) | 6.92 | SANDOVAL (6), GONZALEZDEBARCIA (1), PSEUDOHURTADODEMENDOZA (1) |
| medium | `Anonimo_SegundoJobEl` | VIDALYSALVADOR | 68 | 53/68 (78%) | 6.75 | VIDALYSALVADOR (53), PAREDES (5), MELO (1), GARCIAMARCOS (1) |
| medium | `MHouse_Navas_Autografo_COLOR` | LOPE | 55 | 46/55 (84%) | 6.65 | LOPE (46), GONGORA (1), BELMONTE (1), QUEVEDO (1), CAXESI (1) |
| medium | `Anonimo_BurladoburladorEl` | TORRESLORENZODE | 61 | 40/61 (66%) | 6.57 | TORRESLORENZODE (40), SANDOVAL (3), ROJASZORRILLA (2), BARRIONUEVO (2), PACHECO (1) |
| medium | `Desconocido_ConMusica_acto1` | BOLEAYALVARADO | 18 | 16/18 (89%) | 6.51 | BOLEAYALVARADO (16), CANIZARES (2) |
| medium | `Anonimo_MayorluzdeItaliaSantaClaraLa` | CANIZARES | 60 | 38/60 (63%) | 6.48 | CANIZARES (38), MOLINAYMENDOZA (13), CASTROYSALAZAR (3), LORENZANA (1), LOPEZDECASTRO (1) |
| medium | `Anonimo_CapitanadeamorLa` | GARCIAMARCOS | 8 | 4/8 (50%) | 6.47 | GARCIAMARCOS (4), BANCESCANDAMO (1) |
| medium | `ANONIMO_Cadatontoconsutema` | VIDALYSALVADOR | 22 | 22/22 (100%) | 6.45 | VIDALYSALVADOR (22) |
| medium | `DESCONOCIDO_SoberbiacastigadaeneltriunfodeJudithLas` | GARCIADEPRADO | 45 | 33/45 (73%) | 6.44 | GARCIADEPRADO (33), VIDALYSALVADOR (6), CERVANTES (2), CECILIANACIMIENTO (2) |
| medium | `Anonimo_Enelmayorpeligroseconocelaamis` | LOPE | 28 | 18/28 (64%) | 6.33 | LOPE (18), QUEVEDO (5), LICENCIADOROJAS (1) |
| medium | `Anonimo_Devociondelasanimasymayordomos` | FAJARDOYACEVEDO | 59 | 32/59 (54%) | 6.32 | FAJARDOYACEVEDO (32), RUIZALCEO (8), GARCIAMARCOS (6), MEDINA (3), DAVILAYPALOMARES (2) |
| medium | `DESCONOCIDO_PasmoDeInglaterra` | GILENRIQUEZ | 55 | 45/55 (82%) | 6.25 | GILENRIQUEZ (45), VERATASSIS (4), SANDOVAL (3), CASTROYSALAZAR (1), MELO (1) |
| medium | `DESCONOCIDO_ViciosDeComodo` | SANDOVAL | 32 | 22/32 (69%) | 5.90 | SANDOVAL (22), CALLE (3), TORRESLORENZODE (2), MEDINA (1), BELMONTE (1) |
| medium | `DESCONOCIDO_ElDivinoAlcides` | CASTROYSALAZAR | 13 | 9/13 (69%) | 5.77 | CASTROYSALAZAR (9), SANTATERESA (1), PAREDES (1), VARGASMACHUCA (1), MOLINAYMENDOZA (1) |
| medium | `DESCONOCIDO_FarsaDeLaConstanza` | QUEVEDO | 48 | 27/48 (56%) | 5.74 | QUEVEDO (27), CECILIANACIMIENTO (13), BARRIONUEVO (4), LEONORCUEVA (2), MARCHANTE (1) |
| medium | `MHouse_AlpasardelarroyoCOLOR` | LICENCIADOROJAS | 72 | 42/72 (58%) | 5.70 | LICENCIADOROJAS (42), LORENZANA (17), SANDOVAL (4), GILENRIQUEZ (3), LEONORCUEVA (2) |
| medium | `ANONIMO_MartiresdeCarlet` | LORENZANA | 21 | 13/21 (62%) | 5.53 | LORENZANA (13), PACHECO (5), BARRIONUEVO (2), CERVANTES (1) |
| medium | `DESCONOCIDO_EntremesPerote` | CARVAJAL | 4 | 3/4 (75%) | 5.51 | CARVAJAL (3), CONTRERAS (1) |
| medium | `Anonimo_SoldadovillanoEl` | PAREDES | 14 | 7/14 (50%) | 5.49 | PAREDES (7) |
| medium | `Anonimo_RobodelainfantaLeonidaEl` | MESA | 69 | 36/69 (52%) | 5.48 | MESA (36), RUIZALCEO (13), TORRESLORENZODE (7), ROMEROROQUE (3), GONZALEZDEBARCIA (1) |
| medium | `Anonimo_NacimientodelHijodeDiosEl` | LANINI | 42 | 24/42 (57%) | 5.40 | LANINI (24), VERATASSIS (4), BARRIONUEVO (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| medium | `Anonimo_Pecadorconvertidoporelangeldes` | CALDERON | 59 | 35/59 (59%) | 5.32 | CALDERON (35), GILENRIQUEZ (7), VERATASSIS (3), SARAVIAYMENDOZA (2), VIDALYSALVADOR (2) |
| medium | `Anonimo_Hazbienynomiresaquien` | BELMONTE | 65 | 33/65 (51%) | 5.32 | BELMONTE (33), CLARAMONTE (12), GALLEGOS (5), PACHECO (1), BARREDA (1) |
| medium | `Anonimo_NacimientodelhijodeDiosylanega` | SANDOVAL | 28 | 19/28 (68%) | 5.21 | SANDOVAL (19), LICENCIADOROJAS (1), GALLEGOS (1), CARVAJAL (1) |
| medium | `DESCONOCIDO_LoQueValeElDarPorDios` | GONGORA | 63 | 57/63 (90%) | 5.20 | GONGORA (57), VARGASMACHUCA (2), VIDALYSALVADOR (1), SANDOVAL (1), SANTATERESA (1) |
| medium | `DESCONOCIDO_EntreinocenciayMaldad` | SANDOVAL | 57 | 37/57 (65%) | 5.16 | SANDOVAL (37), GILENRIQUEZ (19), CASTROYSALAZAR (1) |
| medium | `DESCONOCIDO_Coloquiodelasletrasydelasarmas` | CECILIANACIMIENTO | 22 | 13/22 (59%) | 5.08 | CECILIANACIMIENTO (13), VIDALYSALVADOR (5), AVELLANEDA (2) |
| medium | `ANONIMO_Tembleque` | VARGASMACHUCA | 5 | 4/5 (80%) | 5.03 | VARGASMACHUCA (4), VIDALYSALVADOR (1) |
| medium | `DESCONOCIDO_LosValientes` | FAJARDOYACEVEDO | 13 | 7/13 (54%) | 5.02 | FAJARDOYACEVEDO (7), GONZALEZDEBARCIA (1), GONZALEZDETORRES (1), ROMEROROQUE (1) |
| medium | `DESCONOCIDO_FalsificacionCervantes` | CERVANTES | 1 | 1/1 (100%) | 4.97 | CERVANTES (1) |
| medium | `ANONIMO_DiscretaMentirosa` | SANDOVAL | 92 | 57/92 (62%) | 4.92 | SANDOVAL (57), LANINI (8), VERATASSIS (7), CASTROYSALAZAR (5), AVELLANEDA (3) |
| medium | `Desconocido_LocurasOrlando` | SANDOVAL | 31 | 18/31 (58%) | 4.91 | SANDOVAL (18), MEDINA (4), TORRESLORENZODE (3), AVELLANEDA (1), FAJARDOYACEVEDO (1) |
| medium | `DESCONOCIDO_PrevenidoEl` | CASTILLOSOLORZANO | 11 | 8/11 (73%) | 4.88 | CASTILLOSOLORZANO (8), CERVANTES (2), CONTRERAS (1) |
| medium | `Anonimo_OrigendelosCesaresdeRomaEl` | GARCIAMARCOS | 96 | 65/96 (68%) | 4.80 | GARCIAMARCOS (65), LEIVARAMIREZ (11), MOLINAYMENDOZA (4), SANDOVAL (2), CASTILLOSOLORZANO (2) |
| medium | `Desconocido_Troyaabrasada_acto1` | CASTROYSALAZAR | 15 | 11/15 (73%) | 4.78 | CASTROYSALAZAR (11), AVELLANEDA (2), VERATASSIS (1), LOPEZDECARDENA (1) |
| medium | `Anonimo_ReyportruequeEl` | GARCIAMARCOS | 68 | 60/68 (88%) | 4.78 | GARCIAMARCOS (60), LICENCIADOROJAS (1), RUIZALCEO (1) |
| medium | `DESCONOCIDO_Hermandadmassantayfina` | GONZALEZDETORRES | 19 | 11/19 (58%) | 4.72 | GONZALEZDETORRES (11), PACHECO (6), ROSETENINO (1), LANINI (1) |
| medium | `Anonimo_DosfinezasdeamorLas` | LANINI | 68 | 37/68 (54%) | 4.61 | LANINI (37), GARCIAMARCOS (8), PAREDES (4), MOLINAYMENDOZA (4), REMON (2) |
| medium | `DESCONOCIDO_AsombroDeJerez` | SANDOVAL | 60 | 50/60 (83%) | 4.60 | SANDOVAL (50), GONGORA (4), GILENRIQUEZ (2), LEONORCUEVA (1), CASTROYSALAZAR (1) |
| medium | `Anonimo_LetrasLas` | SANDOVAL | 10 | 6/10 (60%) | 4.59 | SANDOVAL (6), CASTILLOSOLORZANO (1) |
| medium | `DESCONOCIDO_Infortunios` | ENRIQUEZ | 56 | 34/56 (61%) | 4.54 | ENRIQUEZ (34), BELMONTE (10), BATRES (2), VILLEGASDELACRUZ (2), QUEVEDO (2) |
| medium | `DESCONOCIDO_VueltadeEgipto` | REMON | 13 | 10/13 (77%) | 4.33 | REMON (10), LICENCIADOROJAS (2), LORENZANA (1) |
| medium | `DESCONOCIDO_DivinoPoluxEl` | CALDERON | 34 | 17/34 (50%) | 4.27 | CALDERON (17), GARCIADEPRADO (9), AMESCUA (3), VIDALYSALVADOR (1), VELEZ (1) |
| medium | `ANONIMO_Introduccionparaelfindefiesta` | MARCHANTE | 5 | 3/5 (60%) | 4.26 | MARCHANTE (3), GILENRIQUEZ (1), VIDALYSALVADOR (1) |
| medium | `DESCONOCIDO_NuevoEspejoEnLaCorte` | TORRESLORENZODE | 49 | 41/49 (84%) | 4.16 | TORRESLORENZODE (41), CARVAJAL (2), LORENZANA (2), GILENRIQUEZ (2), SANDOVAL (1) |
| medium | `DESCONOCIDO_QuieroYNoSabenQueQuiero` | MELO | 88 | 74/88 (84%) | 4.10 | MELO (74), VARGASMACHUCA (7), CERVANTES (5), HURTADODEMENDOZA (1) |
| medium | `Anonimo_Hacerdelamorvenganza` | CARVAJAL | 56 | 34/56 (61%) | 3.85 | CARVAJAL (34), MORETO (3), CAXESI (3), LORENZANA (3), CLARAMONTE (2) |
| medium | `DESCONOCIDO_MejorperladeOrienteLa` | MARCHANTE | 70 | 36/70 (51%) | 3.73 | MARCHANTE (36), CASTROYSALAZAR (20), VIDALYSALVADOR (8), SANDOVAL (3), CASTILLOSOLORZANO (1) |
| medium | `Anonimo_MayortriunfoensimismoEl` | VALDIVIELSO | 68 | 38/68 (56%) | 3.64 | VALDIVIELSO (38), QUINONES (8), MONTALBAN (7), GONGORA (3), CONTRERAS (3) |
| medium | `MHouse_AntonioRocaCOLOR` | AVELLANEDADELACUEVA | 37 | 23/37 (62%) | 3.61 | AVELLANEDADELACUEVA (23), GILENRIQUEZ (4), TORRESLORENZODE (2), GONGORA (2), SANTATERESA (1) |
| medium | `DESCONOCIDO_GrutaDeLosAcasos` | SANDOVAL | 58 | 48/58 (83%) | 3.55 | SANDOVAL (48), GILENRIQUEZ (8), VERATASSIS (2) |
| medium | `Anonimo_NuevoJoseenFranciaEl` | ENRIQUEZ | 81 | 57/81 (70%) | 3.50 | ENRIQUEZ (57), SANDOVAL (5), TIRSO (5), CUEVAYSILVA (3), BELMONTE (2) |
| medium | `DESCONOCIDO_SiempreLaSuerteEsContraria` | CASTROYSALAZAR | 52 | 28/52 (54%) | 3.48 | CASTROYSALAZAR (28), GILENRIQUEZ (14), LORENZANA (7), VERATASSIS (1), LANINI (1) |
| medium | `Anonimo_Nohaycontralarazonfuerza` | MELO | 79 | 42/79 (53%) | 3.44 | MELO (42), GARCIAMARCOS (16), SANDOVAL (6), CASTROYSALAZAR (5), MOLINAYMENDOZA (4) |
| medium | `DESCONOCIDO_RosaPoliciano` | CASTROYSALAZAR | 62 | 43/62 (69%) | 3.44 | CASTROYSALAZAR (43), GONZALEZDETORRES (11), LORENZANA (4), CANIZARES (3), PACHECO (1) |
| medium | `DESCONOCIDO_AutosacramentalparaelBorje` | DIAMANTE | 5 | 3/5 (60%) | 3.41 | DIAMANTE (3), CONTRERAS (1), LEONORCUEVA (1) |
| medium | `ANONIMO_Amigoamanteleal_Novena` | ALARCON | 56 | 32/56 (57%) | 3.27 | ALARCON (32), BOLEAYALVARADO (9), GILENRIQUEZ (4), VIDALYSALVADOR (3), TORRESLORENZODE (3) |
| medium | `DESCONOCIDO_Barbas` | VIDALYSALVADOR | 18 | 13/18 (72%) | 3.25 | VIDALYSALVADOR (13), ENRIQUEZ (2), MELO (2), VARGASMACHUCA (1) |
| medium | `ANONIMO_El_encanto_del_olvido_Novena` | SANDOVAL | 69 | 41/69 (59%) | 3.25 | SANDOVAL (41), MELO (9), MEDINA (8), AVELLANEDA (5), DAVILAYPALOMARES (2) |
| medium | `ANONIMO_Si_una_vez_llega_a_querer_Novena` | SANDOVAL | 69 | 41/69 (59%) | 3.25 | SANDOVAL (41), MELO (9), MEDINA (8), AVELLANEDA (5), DAVILAYPALOMARES (2) |
| medium | `DESCONOCIDO_Forastero` | ROJASZORRILLA | 6 | 4/6 (67%) | 3.23 | ROJASZORRILLA (4), CALDERON (2) |
| medium | `Anonimo_MalainclinacionoElhijomalincli` | BELMONTE | 64 | 33/64 (52%) | 3.20 | BELMONTE (33), ROJASZORRILLA (11), QUEVEDO (4), CALDERON (4), LEIVARAMIREZ (3) |
| medium | `DESCONOCIDO_EntremesSinTituloSonPrincipalesInterlocutoresAguedaYUnSacristan` | BELMONTE | 6 | 3/6 (50%) | 3.18 | BELMONTE (3), GONZALEZDEBARCIA (1), REMON (1), CLARAMONTE (1) |
| medium | `Anonimo_Infelicesdichososentrarporcria` | SANDOVAL | 51 | 31/51 (61%) | 3.09 | SANDOVAL (31), GALLEGOS (8), ROMEROROQUE (5), BOLEAYALVARADO (1), CERVANTES (1) |
| medium | `DESCONOCIDO_SanRoque` | QUEVEDO | 26 | 17/26 (65%) | 3.08 | QUEVEDO (17), BELMONTE (2), LEIVARAMIREZ (2), LOPE (1), GILENRIQUEZ (1) |
| medium | `ANONIMO_Maestresala` | CECILIANACIMIENTO | 6 | 5/6 (83%) | 3.03 | CECILIANACIMIENTO (5), MARCHANTE (1) |
| medium | `MHouse_ProtectoresdeEspanaCOLOR` | GONZALEZDETORRES | 26 | 22/26 (85%) | 3.03 | GONZALEZDETORRES (22), VARGASMACHUCA (3), CECILIANACIMIENTO (1) |
| medium | `DESCONOCIDO_ProcesoContraIsabelRodriguez` | CERVANTES | 965 | 660/965 (68%) | 3.02 | CERVANTES (660), HURTADODEMENDOZA (127), CUEVAYSILVA (35), ENRIQUEZ (33), VARGASMACHUCA (27) |
| low | `Anonimo_NarroEl` | LOPEZJACINTO | 16 | 5/16 (31%) | 35.91 | LOPEZJACINTO (5), JIMENEZSEDENO (1) |
| low | `DESCONOCIDO_PeroHernandez` | SALAZARYTORRES | 9 | 3/9 (33%) | 29.11 | SALAZARYTORRES (3), ROMEROROQUE (2), MULSA (1) |
| low | `Anonimo_UnhijoquenegoasupadreEntremese` | SANTATERESA | 6 | 2/6 (33%) | 24.51 | SANTATERESA (2), BANCESCANDAMO (1), GALLEGOS (1) |
| low | `Anonimo_MojigangaparafiestadeSevilla` | ROSETENINO | 17 | 7/17 (41%) | 18.69 | ROSETENINO (7), HURTADODEMENDOZA (1), ANDOSILLA (1) |
| low | `Anonimo_MuelaLa` | LOPEZDELCAMPO | 15 | 6/15 (40%) | 18.56 | LOPEZDELCAMPO (6), LICENCIADOROJAS (1) |
| low | `DESCONOCIDO_LoaComediaSanIsidro` | DIAMANTE | 24 | 3/24 (12%) | 17.96 | DIAMANTE (3), TORRESLORENZODE (1) |
| low | `ANONIMO_Presentaciontemplo_Novena` | LANINI | 44 | 20/44 (46%) | 14.34 | LANINI (20), LEIVARAMIREZ (17), GILENRIQUEZ (2), GARCIADEPRADO (2), AVELLANEDADELACUEVA (1) |
| low | `ANONIMO_AsistenteSevilla_Novena` | CASTROYSALAZAR | 86 | 31/86 (36%) | 14.01 | CASTROYSALAZAR (31), GILENRIQUEZ (24), MEDINA (17), LEONORCUEVA (6), DAVILAYPALOMARES (6) |
| low | `ANONIMO_Lasfloresbaile` | CANIZARES | 13 | 5/13 (38%) | 13.86 | CANIZARES (5), GONZALEZDEBARCIA (1), CERVANTES (1) |
| low | `Desconocido_AUnTiempoReyYVasallo_acto2y3` | BELMONTE | 64 | 26/64 (41%) | 13.76 | BELMONTE (26), MORETO (13), LEIVARAMIREZ (11), CALLE (11), VARGAS (1) |
| low | `Anonimo_EscandalodeGreciacontralassant` | MOLINAYMENDOZA | 33 | 10/33 (30%) | 12.81 | MOLINAYMENDOZA (10), CASTROYSALAZAR (8), HOZYMOTA (2), LLOBREGATYESTEVE (2), GONZALEZDEBARCIA (1) |
| low | `Anonimo_PuercodesanAntonEl` | SANDOVAL | 16 | 3/16 (19%) | 11.26 | SANDOVAL (3), AMESCUA (1), MELO (1) |
| low | `Anonimo_LatinesLos` | GONZALEZDEBARCIA | 14 | 3/14 (21%) | 11.13 | GONZALEZDEBARCIA (3), MOLINAYMENDOZA (2), LICENCIADOROJAS (1) |
| low | `Anonimo_Enelmartirioeldescansoyeneldes` | CASTROYSALAZAR | 49 | 11/49 (22%) | 10.94 | CASTROYSALAZAR (11), PAREDES (9), LANINI (9), SANDOVAL (7), GARCIAMARCOS (2) |
| low | `Anonimo_ConstanteOrintiaLa` | TORRESLORENZODE | 44 | 10/44 (23%) | 10.37 | TORRESLORENZODE (10), CAXESI (9), BARRIONUEVO (6), MEDINA (3), CASTILLOSOLORZANO (2) |
| low | `ANONIMO_Papelesvarios` | LANINI | 402 | 69/402 (17%) | 10.20 | LANINI (69), CASTROYSALAZAR (62), MELO (34), MOLINAYMENDOZA (29), LEONORCUEVA (21) |
| low | `Anonimo_GranatenienseysoleclipsadoSanD` | MEDINA | 37 | 13/37 (35%) | 10.19 | MEDINA (13), TORRESLORENZODE (6), RUIZALCEO (4), CUEVAYSILVA (3), SANDOVAL (2) |
| low | `DESCONOCIDO_TurnoyEneas` | CECILIANACIMIENTO | 45 | 20/45 (44%) | 10.19 | CECILIANACIMIENTO (20), CASTILLOSOLORZANO (11), ENRIQUEZ (5), PAREDES (2), VARGASMACHUCA (2) |
| low | `MHouse_HumildadsoberbiaCOLOR` | LORENZANA | 23 | 11/23 (48%) | 9.69 | LORENZANA (11), PACHECO (6), CANIZARES (4), GILENRIQUEZ (2) |
| low | `Anonimo_NinoEl` | CASTROYSALAZAR | 14 | 2/14 (14%) | 9.43 | CASTROYSALAZAR (2), MELO (1), PAREDES (1) |
| low | `Anonimo_Venenodelossentidos` | SANDOVAL | 8 | 3/8 (38%) | 9.35 | SANDOVAL (3), GONZALEZDEBARCIA (1), PSEUDOHURTADODEMENDOZA (1) |
| low | `Anonimo_Entremesentreunmuchachollamado` | CUEVAYSILVA | 7 | 3/7 (43%) | 9.34 | CUEVAYSILVA (3), AMESCUA (1) |
| low | `DESCONOCIDO_AntonPanderoGilSonajas` | SANDOVAL | 18 | 5/18 (28%) | 9.34 | SANDOVAL (5), LICENCIADOROJAS (1), LANINI (1) |
| low | `Anonimo_SanRoque` | SANDOVAL | 24 | 8/24 (33%) | 9.27 | SANDOVAL (8), VARGASMACHUCA (3), MELO (2), FAJARDOYACEVEDO (1), RUANO (1) |
| low | `Anonimo_Escenacomicaquerepresentaeltie` | CECILIANACIMIENTO | 174 | 47/174 (27%) | 9.24 | CECILIANACIMIENTO (47), LANINI (25), BANCESCANDAMO (21), BARRIONUEVO (18), LOPEZDELCAMPO (12) |
| low | `Anonimo_Comediaalodivinosobrelaenvidia` | BELMONTE | 361 | 69/361 (19%) | 8.81 | BELMONTE (69), SANDOVAL (67), QUEVEDO (47), ENRIQUEZ (29), ROJASVILLANDRANDO (20) |
| low | `Anonimo_LoaparalaVirgendePenaSacra` | FAJARDOYACEVEDO | 16 | 5/16 (31%) | 8.68 | FAJARDOYACEVEDO (5), LICENCIADOROJAS (1), ANDOSILLA (1) |
| low | `Anonimo_NuncaelbiensillegallegatardeAu` | RUIZALCEO | 36 | 10/36 (28%) | 8.66 | RUIZALCEO (10), QUINONES (7), GARCIAMARCOS (3), SANDOVAL (3), MESA (2) |
| low | `Anonimo_NegaciondelaposadaaSanJoseyelj` | PAREDES | 34 | 13/34 (38%) | 8.43 | PAREDES (13), COELLO (10), GONZALEZDEBARCIA (1) |
| low | `Anonimo_SufridoEl` | VIDALYSALVADOR | 135 | 46/135 (34%) | 8.30 | VIDALYSALVADOR (46), SANDOVAL (35), VERATASSIS (14), PAREDES (11), GARCIAMARCOS (11) |
| low | `Anonimo_DiosesporellealLos` | CAXESI | 307 | 36/307 (12%) | 8.23 | CAXESI (36), ENRIQUEZ (31), BARRIONUEVO (26), CUEVAYSILVA (25), CONTRERAS (24) |
| low | `Anonimo_SacristanembusteroEl` | MARCHANTE | 16 | 4/16 (25%) | 7.96 | MARCHANTE (4), LOPEZDELCAMPO (1), CANIZARES (1), LEONORCUEVA (1) |
| low | `Anonimo_ParnasoEl` | CANIZARES | 10 | 3/10 (30%) | 7.89 | CANIZARES (3), MOLINAYMENDOZA (2), CASTILLOSOLORZANO (1), REMON (1) |
| low | `Anonimo_SimonMagocastigado` | BARRIONUEVO | 57 | 25/57 (44%) | 7.46 | BARRIONUEVO (25), MEDINA (8), REMON (3), LICENCIADOROJAS (3) |
| low | `ANONIMO_Dialogodelasciencias` | LOPE | 25 | 10/25 (40%) | 6.90 | LOPE (10), CECILIANACIMIENTO (8), VIDALYSALVADOR (3), ROJASVILLANDRANDO (1) |
| low | `Anonimo_ReydebastosEl` | MARCHANTE | 16 | 3/16 (19%) | 6.68 | MARCHANTE (3), SANDOVAL (2), LEONORCUEVA (2) |
| low | `Anonimo_PremiodelavirtudCastigoenlamen` | BELMONTE | 31 | 8/31 (26%) | 6.59 | BELMONTE (8), LOPEZDELCAMPO (8), ROJASZORRILLA (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `Anonimo_LinternaynochesdeinviernoLa` | SANDOVAL | 15 | 4/15 (27%) | 6.57 | SANDOVAL (4), CASTILLOSOLORZANO (1), CASTROYSALAZAR (1), MORETO (1) |
| low | `Anonimo_Triunfosdelamorenpanellirioyla` | PAREDES | 51 | 22/51 (43%) | 6.55 | PAREDES (22), VIDALYSALVADOR (19), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `Anonimo_GloriosoSanIsidrodeMadridEl` | CLARAMONTE | 32 | 14/32 (44%) | 6.43 | CLARAMONTE (14), MESA (7), LICENCIADOROJAS (1), QUINONES (1) |
| low | `Anonimo_NochedeSanPedroLa` | FAJARDOYACEVEDO | 14 | 4/14 (29%) | 6.39 | FAJARDOYACEVEDO (4), ROMEROROQUE (1) |
| low | `DESCONOCIDO_AsuncionDeNuestraSenora` | QUINONES | 12 | 4/12 (33%) | 6.27 | QUINONES (4), TORRESLORENZODE (1), VILLEGASDELACRUZ (1), ENRIQUEZ (1) |
| low | `Anonimo_FamosacomediadeladivinaesposaL` | MEDINA | 52 | 22/52 (42%) | 6.20 | MEDINA (22), SANDOVAL (13), TORRESLORENZODE (4), LICENCIADOROJAS (1), LEONORCUEVA (1) |
| low | `Anonimo_NochedetorosenMadridLa` | VIDALYSALVADOR | 16 | 6/16 (38%) | 6.18 | VIDALYSALVADOR (6), BANCESCANDAMO (1) |
| low | `Anonimo_LunadeFlorenciaLa` | RUIZALCEO | 32 | 9/32 (28%) | 6.17 | RUIZALCEO (9), ROMEROROQUE (6), GARCIAMARCOS (5), TORRESLORENZODE (2), FAJARDOYACEVEDO (1) |
| low | `Anonimo_DegollaciondesanJuanLa` | CECILIANACIMIENTO | 452 | 85/452 (19%) | 6.10 | CECILIANACIMIENTO (85), AVELLANEDA (38), CONTRERAS (30), VARGASMACHUCA (22), ENRIQUEZ (21) |
| low | `Anonimo_JuegodevuelapajaritosEl` | SANDOVAL | 10 | 4/10 (40%) | 6.09 | SANDOVAL (4), LEONORCUEVA (1), VARGASMACHUCA (1), BELMONTE (1) |
| low | `DESCONOCIDO_ElEnganoEnLaVictoriaYSitioDeYelves` | MELO | 7 | 3/7 (43%) | 6.04 | MELO (3), ROMEROROQUE (2), CASTROYSALAZAR (2) |
| low | `Anonimo_MejorfrutodelrobleyVirgendeVal` | LANINI | 40 | 10/40 (25%) | 6.04 | LANINI (10), TORRESLORENZODE (8), BANCESCANDAMO (5), PAREDES (3), GONZALEZDEBARCIA (1) |
| low | `DESCONOCIDO_VasodeEleccion_Parma` | QUINONES | 63 | 20/63 (32%) | 6.01 | QUINONES (20), MONTALBAN (15), CONTRERAS (9), REMON (6), VILLEGASDELACRUZ (4) |
| low | `Anonimo_Saineterecitadoenmusica` | MELO | 13 | 3/13 (23%) | 5.99 | MELO (3), ROMEROROQUE (2), LICENCIADOROJAS (1) |
| low | `Anonimo_MilagrosoespanolEl` | SANDOVAL | 34 | 9/34 (26%) | 5.99 | SANDOVAL (9), LOPEZDECASTRO (8), GOMEZACOSTA (4), TORRESLORENZODE (3), BENAVIDES (2) |
| low | `DESCONOCIDO_CuerdoDelirioAmor` | CASTROYSALAZAR | 44 | 19/44 (43%) | 5.97 | CASTROYSALAZAR (19), MELO (17), MEDINA (4), LOPEZDECASTRO (3), GILENRIQUEZ (1) |
| low | `Anonimo_DichadelretraidoLa` | ANDOSILLA | 68 | 19/68 (28%) | 5.78 | ANDOSILLA (19), GALLEGOS (17), LEIVARAMIREZ (6), MOLINAYMENDOZA (6), BELMONTE (2) |
| low | `Anonimo_Introduccionaunbaileyjuego` | CANIZARES | 12 | 4/12 (33%) | 5.75 | CANIZARES (4), CERVANTES (1), LEIVARAMIREZ (1), LEONORCUEVA (1) |
| low | `Anonimo_FeriadelbuengustoLa` | CASTROYSALAZAR | 8 | 3/8 (38%) | 5.75 | CASTROYSALAZAR (3), GONZALEZDEBARCIA (1), CANIZARES (1) |
| low | `Anonimo_PleitodelmochueloEl` | PAREDES | 14 | 5/14 (36%) | 5.66 | PAREDES (5), VARGAS (1) |
| low | `Anonimo_DivinaesposaLa` | QUEVEDO | 29 | 8/29 (28%) | 5.60 | QUEVEDO (8), ROMEROROQUE (6), LOPE (2), LICENCIADOROJAS (1), BENAVIDES (1) |
| low | `Anonimo_SabanonesLos` | VIDALYSALVADOR | 16 | 4/16 (25%) | 5.59 | VIDALYSALVADOR (4), PAREDES (2), LICENCIADOROJAS (1), LOPEZJACINTO (1) |
| low | `Anonimo_Empenoydesempenodelsantisimosa` | ROJASZORRILLA | 33 | 13/33 (39%) | 5.57 | ROJASZORRILLA (13), BELMONTE (10), PACHECO (1), ROMEROROQUE (1), LEIVARAMIREZ (1) |
| low | `Anonimo_BurladelpellejoLa` | SANDOVAL | 13 | 2/13 (15%) | 5.35 | SANDOVAL (2), ROMEROROQUE (2) |
| low | `MHouse_CuerdolocoCOLOR` | LOPE | 68 | 33/68 (48%) | 5.33 | LOPE (33), CLARAMONTE (4), VELEZ (3), ROMEROROQUE (3), BELMONTE (3) |
| low | `DESCONOCIDO_Cuevasalvajes` | BELMONTE | 26 | 8/26 (31%) | 5.24 | BELMONTE (8), TORRESLORENZODE (8), FBQUIROS (6), ROSETENINO (2), CASTILLOSOLORZANO (1) |
| low | `Anonimo_LoaacasoparalacomediaTodoestas` | CONTRERAS | 47 | 16/47 (34%) | 5.12 | CONTRERAS (16), CARVAJAL (10), LOPEZDELCAMPO (3), CAXESI (3), QUINONES (2) |
| low | `ANONIMO_NuestraSenoraFuencisla` | LORENZANA | 36 | 16/36 (44%) | 5.09 | LORENZANA (16), BELMONTE (7), GILENRIQUEZ (4), REMON (3), LICENCIADOROJAS (1) |
| low | `Anonimo_Zenonia` | VARGAS | 228 | 75/228 (33%) | 5.08 | VARGAS (75), RUIZALCEO (38), MULSA (30), CUEVAYSILVA (25), GARCIAMARCOS (9) |
| low | `Anonimo_PadrinodesuafrentaEl` | PAREDES | 74 | 32/74 (43%) | 5.06 | PAREDES (32), MELO (14), ONAVIEDMAYTORRES (7), CASTROYSALAZAR (5), SANDOVAL (4) |
| low | `Anonimo_ValientesLos` | CERVANTES | 14 | 2/14 (14%) | 5.00 | CERVANTES (2), LORENZANA (2), CARVAJAL (2), LICENCIADOROJAS (1) |
| low | `Anonimo_JuanHidalgo` | CANIZARES | 10 | 4/10 (40%) | 4.99 | CANIZARES (4), QUINONES (2), ROMEROROQUE (1), LEONORCUEVA (1) |
| low | `Anonimo_EnsaladillaLa` | LORENZANA | 12 | 2/12 (17%) | 4.96 | LORENZANA (2), MATOSFRAGOSO (1) |
| low | `Anonimo_Coloquiodelaprisionlibreyliber` | MEDINA | 46 | 16/46 (35%) | 4.92 | MEDINA (16), SANDOVAL (14), FAJARDOYACEVEDO (4), MELO (3), CERVANTES (1) |
| low | `Anonimo_Bailesintitulo` | AVELLANEDA | 1000 | 117/1000 (12%) | 4.92 | AVELLANEDA (117), CECILIANACIMIENTO (111), VIDALYSALVADOR (98), GOMEZACOSTA (73), VERATASSIS (58) |
| low | `Anonimo_CastigoensucautelaEl` | BELMONTE | 61 | 23/61 (38%) | 4.85 | BELMONTE (23), CLARAMONTE (8), GALLEGOS (6), VELEZ (4), MOLINAYMENDOZA (3) |
| low | `MHouse_VillanaGetafeCOLOR` | LICENCIADOROJAS | 33 | 8/33 (24%) | 4.82 | LICENCIADOROJAS (8), CAXESI (8), CARVAJAL (7), LORENZANA (3), GOMEZACOSTA (2) |
| low | `Anonimo_BeataLa` | CASTROYSALAZAR | 10 | 4/10 (40%) | 4.79 | CASTROYSALAZAR (4), LEONORCUEVA (1), CASTILLOSOLORZANO (1), SANDOVAL (1), VIDALYSALVADOR (1) |
| low | `Anonimo_SanJuanensuApocalipsis` | CASTROYSALAZAR | 61 | 21/61 (34%) | 4.71 | CASTROYSALAZAR (21), SANDOVAL (14), VIDALYSALVADOR (6), PAREDES (5), LANINI (2) |
| low | `DESCONOCIDO_QueHabraQueNoVenzaAmor` | CASTROYSALAZAR | 41 | 10/41 (24%) | 4.66 | CASTROYSALAZAR (10), GILENRIQUEZ (7), MELO (6), ROMEROROQUE (6), SANDOVAL (2) |
| low | `MHouse_CastigosinvenganzaCOLOR` | CARVAJAL | 70 | 17/70 (24%) | 4.60 | CARVAJAL (17), SANDOVAL (14), MELO (12), VERATASSIS (8), AVELLANEDA (8) |
| low | `Anonimo_CastigoenlaarroganciaEl` | GARCIAMARCOS | 46 | 19/46 (41%) | 4.58 | GARCIAMARCOS (19), CALLE (10), FAJARDOYACEVEDO (7), GONZALEZDEBARCIA (1) |
| low | `Anonimo_NinodelaRollonaEl` | HOZYMOTA | 246 | 65/246 (26%) | 4.47 | HOZYMOTA (65), MOLINAYMENDOZA (47), CASTILLOSOLORZANO (42), CASTROYSALAZAR (23), BOLEAYALVARADO (23) |
| low | `Anonimo_ReinapenitenteLa` | CARVAJAL | 52 | 15/52 (29%) | 4.43 | CARVAJAL (15), VILLEGASJUANBAUTISTA (7), GALLEGOS (5), AGUADOELVIEJO (4), MULSA (4) |
| low | `Anonimo_PrimerllantodelalbaodeElninoDi` | CECILIANACIMIENTO | 228 | 84/228 (37%) | 4.39 | CECILIANACIMIENTO (84), LANINI (36), AVELLANEDA (27), ONAVIEDMAYTORRES (17), PAREDES (10) |
| low | `Anonimo_MorirencruzdalavidaoVidadeDima` | ROMEROROQUE | 46 | 21/46 (46%) | 4.37 | ROMEROROQUE (21), VARGASMACHUCA (10), MELO (2), RUANO (2), BANCESCANDAMO (1) |
| low | `Desconocido_obrasdramaticas_Palacio` | RUIZALCEO | 27 | 10/27 (37%) | 4.37 | RUIZALCEO (10), GOMEZACOSTA (5), CUEVAYSILVA (2), MEDINA (2), PACHECO (2) |
| low | `Anonimo_PrimersoldeToledoSanEugenioEl` | VIDALYSALVADOR | 73 | 20/73 (27%) | 4.30 | VIDALYSALVADOR (20), CASTROYSALAZAR (13), MARCHANTE (9), GONGORA (8), VERATASSIS (7) |
| low | `ANONIMO_Adonis` | GILENRIQUEZ | 11 | 5/11 (46%) | 4.21 | GILENRIQUEZ (5), LICENCIADOROJAS (2), VERATASSIS (2), CARVAJAL (1), TORRESLORENZODE (1) |
| low | `Anonimo_EspadadelsegundoAdanLa` | LANINI | 378 | 53/378 (14%) | 4.19 | LANINI (53), CASTROYSALAZAR (46), MOLINAYMENDOZA (38), VERATASSIS (32), SANDOVAL (28) |
| low | `ANONIMO_AcademiaBurlescaBnF` | MELO | 80 | 36/80 (45%) | 4.19 | MELO (36), LOPEZDECASTRO (24), LANINI (16), SANDOVAL (3), AVELLANEDA (1) |
| low | `Anonimo_RecaidadelalmaLa` | TORRESLORENZODE | 38 | 13/38 (34%) | 4.18 | TORRESLORENZODE (13), SANDOVAL (12), CUEVAYSILVA (1), JIMENEZSEDENO (1), ROMEROROQUE (1) |
| low | `DESCONOCIDO_AmorAprisionado` | MOLINAYMENDOZA | 9 | 4/9 (44%) | 4.18 | MOLINAYMENDOZA (4), BANCESCANDAMO (1), GONZALEZDEBARCIA (1) |
| low | `Anonimo_NigromanticoEl` | PAREDES | 16 | 4/16 (25%) | 4.11 | PAREDES (4), GONZALEZDEBARCIA (1), JIMENEZSEDENO (1) |
| low | `DESCONOCIDO_LealtadPerseguidaEnvidiaCruel` | SANDOVAL | 91 | 40/91 (44%) | 4.09 | SANDOVAL (40), VERATASSIS (31), GILENRIQUEZ (18), GONZALEZDETORRES (1), LANINI (1) |
| low | `Anonimo_AventurasdeGreciaLas` | SANDOVAL | 86 | 32/86 (37%) | 4.08 | SANDOVAL (32), FAJARDOYACEVEDO (15), ROMEROROQUE (6), TORRESLORENZODE (6), PAREDES (5) |
| low | `Anonimo_TutilimundiEntremesEl` | PAREDES | 16 | 5/16 (31%) | 4.08 | PAREDES (5), GONZALEZDEBARCIA (3), LOPEZJACINTO (1) |
| low | `ANONIMO_MasPeregrinoEspejo` | VERATASSIS | 78 | 38/78 (49%) | 4.07 | VERATASSIS (38), SANDOVAL (32), GILENRIQUEZ (8) |
| low | `Anonimo_MayaLa` | SANDOVAL | 12 | 3/12 (25%) | 4.06 | SANDOVAL (3), VERATASSIS (2), GONZALEZDEBARCIA (1), GARCIAMARCOS (1), LANINI (1) |
| low | `Anonimo_PorfiadosLos` | SANDOVAL | 16 | 2/16 (12%) | 4.06 | SANDOVAL (2), CUENCAYARGUELLO (1), AGUADOELVIEJO (1), MORETO (1) |
| low | `DESCONOCIDO_JoasreydeJuda` | CASTILLOSOLORZANO | 19 | 7/19 (37%) | 4.04 | CASTILLOSOLORZANO (7), CERVANTES (4), CECILIANACIMIENTO (4), BANCESCANDAMO (1), CONTRERAS (1) |
| low | `Anonimo_Vientocontraviento` | VARGAS | 254 | 58/254 (23%) | 4.01 | VARGAS (58), PAREDES (40), AVELLANEDA (26), SALAZARYTORRES (23), LICENCIADOROJAS (21) |
| low | `Anonimo_NinosfingidosEntremesLos` | LEONORCUEVA | 16 | 6/16 (38%) | 4.00 | LEONORCUEVA (6), FAJARDOYACEVEDO (1) |
| low | `DESCONOCIDO_TeatroBreve2` | MELO | 148 | 71/148 (48%) | 3.98 | MELO (71), VARGASMACHUCA (42), VIDALYSALVADOR (30), ENRIQUEZ (1), GONZALEZDEBARCIA (1) |
| low | `Desconocido_PrincipePerseguido_acto2_Autografo` | MORETO | 27 | 9/27 (33%) | 3.93 | MORETO (9), LEIVARAMIREZ (6), ROJASZORRILLA (4), HOZYMOTA (2), CORDERO (2) |
| low | `Anonimo_CampodelaverdadEl` | GOMEZACOSTA | 57 | 7/57 (12%) | 3.92 | GOMEZACOSTA (7), BOLEAYALVARADO (6), RUIZALCEO (5), MOLINAYMENDOZA (4), LANINI (3) |
| low | `Anonimo_LoaparalafiestadeNuestraSenora` | LICENCIADOROJAS | 19 | 7/19 (37%) | 3.91 | LICENCIADOROJAS (7), TORRESLORENZODE (3), CUEVAYSILVA (1) |
| low | `Anonimo_EspadanegraLa` | VERATASSIS | 8 | 3/8 (38%) | 3.80 | VERATASSIS (3), CASTILLOSOLORZANO (1), LEIVARAMIREZ (1), SANDOVAL (1) |
| low | `Anonimo_Delaabarcaalacorona` | LEIVARAMIREZ | 75 | 31/75 (41%) | 3.79 | LEIVARAMIREZ (31), CASTILLOSOLORZANO (23), VIDALYSALVADOR (4), ENRIQUEZ (3), GARCIADEPRADO (2) |
| low | `Anonimo_HermosuraLa` | CASTROYSALAZAR | 10 | 3/10 (30%) | 3.77 | CASTROYSALAZAR (3), CERVANTES (1), MOLINAYMENDOZA (1) |
| low | `Anonimo_GuardainfanteEl` | CECILIANACIMIENTO | 452 | 132/452 (29%) | 3.76 | CECILIANACIMIENTO (132), PAREDES (88), VARGASMACHUCA (55), VIDALYSALVADOR (37), AVELLANEDADELACUEVA (14) |
| low | `Anonimo_SanFranciscoAutosacramental` | ROSETENINO | 28 | 9/28 (32%) | 3.73 | ROSETENINO (9), BELMONTE (6), MIRACLESSOTOMAYOR (5), LICENCIADOROJAS (1), LOPEZDECASTRO (1) |
| low | `Anonimo_SombraLa` | ROMEROROQUE | 13 | 2/13 (15%) | 3.69 | ROMEROROQUE (2), RUANO (1), GONZALEZDEBARCIA (1) |
| low | `Anonimo_InclinacionespanolaLa` | BELMONTE | 62 | 16/62 (26%) | 3.67 | BELMONTE (16), SANDOVAL (14), ANDOSILLA (11), MESA (3), LEIVARAMIREZ (3) |
| low | `Anonimo_Restauraciondelasimagenesporla` | MEDINA | 76 | 14/76 (18%) | 3.59 | MEDINA (14), MESA (13), ANDOSILLA (12), QUINONES (7), VARGAS (6) |
| low | `DESCONOCIDO_GrandezasDelCapitan` | BELMONTE | 28 | 9/28 (32%) | 3.56 | BELMONTE (9), ENRIQUEZ (7), SANDOVAL (5), TORRESLORENZODE (5), BENAVIDES (1) |
| low | `MHouse_PeribanezCOLOR` | CARVAJAL | 43 | 13/43 (30%) | 3.55 | CARVAJAL (13), LORENZANA (10), ROMEROROQUE (6), ROJASZORRILLA (3), TORRESLORENZODE (2) |
| low | `Anonimo_RepelonEl` | CASTROYSALAZAR | 16 | 3/16 (19%) | 3.54 | CASTROYSALAZAR (3), GONGORA (3), CARVAJAL (1), SANDOVAL (1) |
| low | `Anonimo_AventurasdelalmaLas` | MOLINAYMENDOZA | 32 | 7/32 (22%) | 3.52 | MOLINAYMENDOZA (7), BELMONTE (5), GARCIAMARCOS (3), GILENRIQUEZ (3), BANCESCANDAMO (1) |
| low | `Anonimo_Nohayinstantesinengano` | LANINI | 77 | 28/77 (36%) | 3.51 | LANINI (28), GILENRIQUEZ (15), VERATASSIS (10), TORRESLORENZODE (4), CASTROYSALAZAR (3) |
| low | `DESCONOCIDO_Colmenas` | CAXESI | 19 | 9/19 (47%) | 3.48 | CAXESI (9), ALARCON (4), HOZYMOTA (3), GARCIADEPRADO (2), CARVAJAL (1) |
| low | `Anonimo_Loasacramentaldeunvillano` | ROMEROROQUE | 6 | 2/6 (33%) | 3.48 | ROMEROROQUE (2), GONZALEZDEBARCIA (1), MELO (1) |
| low | `Anonimo_PlatodeGenovaEl` | MULSA | 41 | 10/41 (24%) | 3.47 | MULSA (10), MENESES (4), CAXESI (3), TAMAYO (2), GARCIADEPRADO (2) |
| low | `Anonimo_LevantamientodelilustreTeofilo` | MESA | 62 | 18/62 (29%) | 3.46 | MESA (18), SALAZARYTORRES (14), CARVAJAL (8), RUIZALCEO (4), PACHECO (1) |
| low | `Anonimo_LoquepasaenMadrid` | VIDALYSALVADOR | 20 | 3/20 (15%) | 3.43 | VIDALYSALVADOR (3), MOLINAYMENDOZA (3), LICENCIADOROJAS (1), HURTADODEMENDOZA (1), QUINONES (1) |
| low | `Anonimo_ParidaLa` | SANDOVAL | 16 | 3/16 (19%) | 3.40 | SANDOVAL (3), VIDALYSALVADOR (1), MARCHANTE (1), CASTROYSALAZAR (1), GONZALEZDEBARCIA (1) |
| low | `Anonimo_HungarofamosoysegundoSanEsteba` | LEIVARAMIREZ | 56 | 18/56 (32%) | 3.39 | LEIVARAMIREZ (18), TORRESLORENZODE (9), JUANDESOTO (4), RUIZALCEO (2), CARVAJAL (2) |
| low | `Anonimo_VidadesanAtanasiofrailelegodel` | ALARCON | 21 | 7/21 (33%) | 3.39 | ALARCON (7), CASTILLOSOLORZANO (5), CARVAJAL (2), JUANDESOTO (1) |
| low | `Anonimo_HidalgoEl` | CASTILLOSOLORZANO | 21 | 6/21 (29%) | 3.34 | CASTILLOSOLORZANO (6), ALARCON (2), LICENCIADOROJAS (1), PSEUDOHURTADODEMENDOZA (1), GARCIADEPRADO (1) |
| low | `Anonimo_PaciodeChristoNostreSenorAutoe` | FAJARDOYACEVEDO | 98 | 14/98 (14%) | 3.32 | FAJARDOYACEVEDO (14), QUINONES (14), SANDOVAL (13), RUANO (11), BELMONTE (7) |
| low | `DESCONOCIDO_TriunfoHumildad_Parma` | LOPEZDECARDENA | 49 | 23/49 (47%) | 3.28 | LOPEZDECARDENA (23), AVELLANEDA (22), CUEVAYSILVA (2), MESA (2) |
| low | `Anonimo_PapanatasLos` | FAJARDOYACEVEDO | 18 | 5/18 (28%) | 3.28 | FAJARDOYACEVEDO (5), VARGASMACHUCA (2), LICENCIADOROJAS (1) |
| low | `CARTASvariasmanos_TorreyServil_Autografo` | MELO | 13 | 3/13 (23%) | 3.27 | MELO (3), AGUADOELVIEJO (2), AMESCUA (1), CONTRERAS (1), CANIZARES (1) |
| low | `Anonimo_EntremesnuevoparafiestadeCorpu` | GILENRIQUEZ | 16 | 7/16 (44%) | 3.22 | GILENRIQUEZ (7), ROMEROROQUE (1), GONZALEZDEBARCIA (1), MOLINAYMENDOZA (1), CASTROYSALAZAR (1) |
| low | `Anonimo_NochedecarnestolendasDelacriti` | FAJARDOYACEVEDO | 14 | 2/14 (14%) | 3.22 | FAJARDOYACEVEDO (2), PAREDES (1), AVELLANEDADELACUEVA (1) |
| low | `Anonimo_Devociondelasanimasdelpurgator` | CARVAJAL | 56 | 18/56 (32%) | 3.16 | CARVAJAL (18), CASTILLOSOLORZANO (17), ROMEROROQUE (4), CAXESI (4), MULSA (2) |
| low | `DESCONOCIDO_AngelDeLasEscuelas` | GRACIAN | 40 | 9/40 (22%) | 3.09 | GRACIAN (9), SALAZARYTORRES (8), SANTATERESA (6), LICENCIADOROJAS (5), GONZALEZDEBARCIA (1) |
| low | `Anonimo_NuestraSenoradelaVargadelavill` | ENRIQUEZ | 21 | 7/21 (33%) | 3.05 | ENRIQUEZ (7), BELMONTE (3), CARVAJAL (1), ROMEROROQUE (1) |
| low | `Anonimo_RenunciaciondelreyWambayfundac` | ANDOSILLA | 63 | 28/63 (44%) | 3.03 | ANDOSILLA (28), MESA (17), TAMAYO (12), BELMONTE (1) |
| low | `DESCONOCIDO_GranSaladina` | CARVAJAL | 50 | 19/50 (38%) | 3.03 | CARVAJAL (19), ROMEROROQUE (11), ENRIQUEZ (7), CASTILLOSOLORZANO (6), GARCIADEPRADO (3) |
| low | `Anonimo_LoquepasaenmitaddeCuaresmaalpa` | SANDOVAL | 17 | 3/17 (18%) | 3.02 | SANDOVAL (3), TAMAYO (3), GONGORA (1), PAREDES (1) |
| low | `DESCONOCIDO_MemoriaDelAutorCordoba` | SANTATERESA | 23 | 6/23 (26%) | 3.01 | SANTATERESA (6), CLARAMONTE (1), CERVANTES (1), VERATASSIS (1), SANDOVAL (1) |
| low | `Anonimo_VidaypersecucionesdeSanEstacio` | MESA | 21 | 8/21 (38%) | 3.00 | MESA (8), CUEVAYSILVA (4), CARVAJAL (1), BELMONTE (1), CASTILLOSOLORZANO (1) |
| low | `DESCONOCIDO_RepartimientoDelPan_Auto` | CUEVAYSILVA | 12 | 8/12 (67%) | 2.98 | CUEVAYSILVA (8), LOPEZDECASTRO (2), LICENCIADOROJAS (1), PACHECO (1) |
| low | `DESCONOCIDO_SelveAvventurose` | GONZALEZDETORRES | 119 | 59/119 (50%) | 2.98 | GONZALEZDETORRES (59), VARGAS (26), CERVANTES (19), MELO (6), MULSA (6) |
| low | `DESCONOCIDO_SenoraInesLa` | MELO | 13 | 10/13 (77%) | 2.97 | MELO (10), AVELLANEDA (2), BARREDA (1) |
| low | `ANONIMO_AventurasverdaderasdelsegundodonQuijoteLas` | MARCHANTE | 37 | 13/37 (35%) | 2.97 | MARCHANTE (13), VIDALYSALVADOR (10), QUEVEDO (8), GILENRIQUEZ (5), HOZYMOTA (1) |
| low | `Anonimo_PeticionLa` | PAREDES | 14 | 3/14 (21%) | 2.95 | PAREDES (3), LEONORCUEVA (1), MOLINAYMENDOZA (1) |
| low | `Anonimo_RebuznoEl` | GONZALEZDEBARCIA | 9 | 2/9 (22%) | 2.95 | GONZALEZDEBARCIA (2), MOLINAYMENDOZA (2), AMESCUA (1), VIDALYSALVADOR (1) |
| low | `Anonimo_AventurasdelcaballerodonPascua` | FAJARDOYACEVEDO | 24 | 6/24 (25%) | 2.95 | FAJARDOYACEVEDO (6), MELO (2), CANIZARES (2), LICENCIADOROJAS (1), HURTADODEMENDOZA (1) |
| low | `DESCONOCIDO_MayorTriunfoDeAmor` | VIDALYSALVADOR | 24 | 18/24 (75%) | 2.95 | VIDALYSALVADOR (18), VARGASMACHUCA (5) |
| low | `DESCONOCIDO_LaPlazaMayor` | MOLINAYMENDOZA | 14 | 4/14 (29%) | 2.92 | MOLINAYMENDOZA (4), CANIZARES (3), GONZALEZDEBARCIA (1), MELO (1), CASTROYSALAZAR (1) |
| low | `Anonimo_CautivosLos` | SANDOVAL | 20 | 5/20 (25%) | 2.91 | SANDOVAL (5), BELMONTE (5), MEDINA (3), LORENZANA (1), GONZALEZDEBARCIA (1) |
| low | `Anonimo_Tratodelaldea` | ROMEROROQUE | 40 | 14/40 (35%) | 2.91 | ROMEROROQUE (14), SANDOVAL (6), GONZALEZDEBARCIA (2), BANCESCANDAMO (2), CONTRERAS (2) |
| low | `DESCONOCIDO_GranPastorialDeArcadia` | LOPEZDECASTRO | 32 | 13/32 (41%) | 2.90 | LOPEZDECASTRO (13), CASTILLOSOLORZANO (4), CALLE (4), BENAVIDES (3), VARGASMACHUCA (3) |
| low | `DESCONOCIDO_Triunfodelaelocuencia` | BANCESCANDAMO | 25 | 12/25 (48%) | 2.90 | BANCESCANDAMO (12), ENRIQUEZ (5), CASTILLOSOLORZANO (4), CORDERO (2), CERVANTES (2) |
| low | `DESCONOCIDO_Cruelmartiriodelcobre` | HURTADODEMENDOZA | 1 | 1/1 (100%) | 2.86 | HURTADODEMENDOZA (1) |
| low | `Anonimo_RudapoliticaLa` | GARCIAMARCOS | 203 | 32/203 (16%) | 2.84 | GARCIAMARCOS (32), FAJARDOYACEVEDO (25), ANDOSILLA (22), QUINONES (20), ROMEROROQUE (19) |
| low | `Anonimo_LuceroserafinEl` | GALLEGOS | 34 | 21/34 (62%) | 2.81 | GALLEGOS (21), QUEVEDO (2), LICENCIADOROJAS (1), SAAVEDRAFAJARDO (1), LOPEZDECASTRO (1) |
| low | `DESCONOCIDO_MemoriaDeDiversosAutos` | HURTADODEMENDOZA | 65 | 47/65 (72%) | 2.79 | HURTADODEMENDOZA (47), AVELLANEDA (4), CERVANTES (2), GARCIADEPRADO (2), CECILIANACIMIENTO (2) |
| low | `DESCONOCIDO_OpusculosVarios` | VIDALYSALVADOR | 421 | 102/421 (24%) | 2.78 | VIDALYSALVADOR (102), VARGASMACHUCA (74), GARCIADEPRADO (34), GONZALEZDEBARCIA (33), LEONORCUEVA (28) |
| low | `DESCONOCIDO_ArdienteEspada` | MESA | 55 | 29/55 (53%) | 2.78 | MESA (29), MULSA (8), VARGAS (2), ROJASVILLANDRANDO (2), ENRIQUEZ (1) |
| low | `Anonimo_FirmezadelaIglesiaAutoLa` | BELMONTE | 44 | 16/44 (36%) | 2.77 | BELMONTE (16), LOPEZDELCAMPO (5), COELLO (4), ALARCON (3), LEIVARAMIREZ (2) |
| low | `Anonimo_Imperioprodigiosoypazensuleyfu` | BELMONTE | 58 | 23/58 (40%) | 2.77 | BELMONTE (23), ROJASZORRILLA (10), CANIZARES (4), VELEZ (4), ANDOSILLA (3) |
| low | `Anonimo_Entremessintitulo` | BELMONTE | 8 | 5/8 (62%) | 2.74 | BELMONTE (5), BANCESCANDAMO (1) |
| low | `ANONIMO_CercodeAlmeriayconquistaEl` | CALDERON | 48 | 14/48 (29%) | 2.72 | CALDERON (14), LEIVARAMIREZ (12), BATRES (10), PAREDES (3), BELMONTE (2) |
| low | `DESCONOCIDO_VasodeeleccionEl` | LICENCIADOROJAS | 60 | 42/60 (70%) | 2.71 | LICENCIADOROJAS (42), ENRIQUEZ (6), AVELLANEDA (5), LEIVARAMIREZ (3), QUINONES (2) |
| low | `DESCONOCIDO_AstrosYFlores` | CALDERON | 6 | 4/6 (67%) | 2.71 | CALDERON (4), VIDALYSALVADOR (1), HURTADODEMENDOZA (1) |
| low | `Anonimo_Contrariosparecidosodesdichave` | PAREDES | 86 | 24/86 (28%) | 2.71 | PAREDES (24), GARCIAMARCOS (19), TAMAYO (18), FAJARDOYACEVEDO (7), VARGAS (2) |
| low | `DESCONOCIDO_LoQueVaDeCetroACetro` | LEONORCUEVA | 67 | 57/67 (85%) | 2.70 | LEONORCUEVA (57), SANDOVAL (5), QUEVEDO (2), CERVANTES (2), VERATASSIS (1) |
| low | `Anonimo_SilvoEntremesEl` | VIDALYSALVADOR | 10 | 1/10 (10%) | 2.68 | VIDALYSALVADOR (1), GONZALEZDEBARCIA (1) |
| low | `Anonimo_MojigangaparaelSitiodelBuenRet` | FAJARDOYACEVEDO | 8 | 2/8 (25%) | 2.68 | FAJARDOYACEVEDO (2), LEONORCUEVA (1), GRACIAN (1), VARGASMACHUCA (1), ROMEROROQUE (1) |
| low | `Anonimo_SangradorEl` | GONZALEZDEBARCIA | 8 | 6/8 (75%) | 2.68 | GONZALEZDEBARCIA (6) |
| low | `DESCONOCIDO_Labellasayaguesa` | CASTILLOSOLORZANO | 34 | 14/34 (41%) | 2.67 | CASTILLOSOLORZANO (14), JIMENEZSEDENO (4), CALDERON (3), CALLE (3), GARCIADEPRADO (3) |
| low | `ANONIMO_LosciegosBritish` | SANDOVAL | 11 | 9/11 (82%) | 2.65 | SANDOVAL (9), MELO (1), VERATASSIS (1) |
| low | `DESCONOCIDO_AnardaYSilvio` | TORRESLORENZODE | 6 | 2/6 (33%) | 2.64 | TORRESLORENZODE (2), CERVANTES (1), CASTILLOSOLORZANO (1) |
| low | `Anonimo_LoaparaelautosacramentaldeMisticayrealBabilonia` | SANDOVAL | 9 | 3/9 (33%) | 2.63 | SANDOVAL (3), CASTROYSALAZAR (1), FAJARDOYACEVEDO (1), MOLINAYMENDOZA (1) |
| low | `Anonimo_TreslasfinezasdelmayoramanteyE` | MELO | 24 | 8/24 (33%) | 2.62 | MELO (8), ROMEROROQUE (5), GARCIAMARCOS (4), PSEUDOHURTADODEMENDOZA (1) |
| low | `Anonimo_TriunfodelSantisimoSacramentoE` | COELLO | 32 | 13/32 (41%) | 2.60 | COELLO (13), MULSA (2), CARVAJAL (2), CALDERON (2), LICENCIADOROJAS (1) |
| low | `DESCONOCIDO_Amornovencepoderniengano` | VERATASSIS | 180 | 100/180 (56%) | 2.58 | VERATASSIS (100), GONGORA (55), SANDOVAL (6), CALLE (5), CANIZARES (4) |
| low | `MHouse_PrimeroreydelmundoCOLOR` | SANDOVAL | 54 | 16/54 (30%) | 2.58 | SANDOVAL (16), TORRESLORENZODE (14), CASTROYSALAZAR (12), MELO (3), VARGASMACHUCA (2) |
| low | `DESCONOCIDO_Propositos` | ENRIQUEZ | 48 | 15/48 (31%) | 2.57 | ENRIQUEZ (15), CAXESI (12), CASTILLOSOLORZANO (5), LEIVARAMIREZ (3), TORRESLORENZODE (2) |
| low | `Anonimo_MulatodeHuescarEl` | ANDOSILLA | 12 | 2/12 (17%) | 2.56 | ANDOSILLA (2), LICENCIADOROJAS (1), QUINONES (1), LOPEZJACINTO (1) |
| low | `Anonimo_Entremessintitulocuyosinterloc` | BELMONTE | 8 | 3/8 (38%) | 2.56 | BELMONTE (3), CERVANTES (1), SANDOVAL (1) |
| low | `Anonimo_ConversiondesanDionisioolaconv` | QUEVEDO | 23 | 10/23 (44%) | 2.56 | QUEVEDO (10), LOPE (3), MESA (2), LEONORCUEVA (1), BELMONTE (1) |
| low | `MHouse_LoqueesuncocheCOLOR` | GILENRIQUEZ | 53 | 20/53 (38%) | 2.55 | GILENRIQUEZ (20), CASTROYSALAZAR (19), TORRESLORENZODE (5), CANIZARES (5), LORENZANA (2) |
| low | `Desconocida_MartirdeMadrid_restoscopista_Autografo` | CASTILLOSOLORZANO | 10 | 4/10 (40%) | 2.54 | CASTILLOSOLORZANO (4), CERVANTES (2), GARCIADEPRADO (1), AMESCUA (1) |
| low | `DESCONOCIDO_HungaroFamoso` | AVELLANEDA | 36 | 7/36 (19%) | 2.54 | AVELLANEDA (7), REMON (6), CERVANTES (6), CARVAJAL (5), CECILIANACIMIENTO (5) |
| low | `DESCONOCIDO_AlbaYSol` | MELO | 58 | 53/58 (91%) | 2.50 | MELO (53), GONZALEZDETORRES (1), SANDOVAL (1), LOPEZDECASTRO (1), CASTROYSALAZAR (1) |
| low | `DESCONOCIDO_EnmudecerEsAmar` | GILENRIQUEZ | 40 | 14/40 (35%) | 2.50 | GILENRIQUEZ (14), LANINI (12), TORRESLORENZODE (11), LORENZANA (1), SANDOVAL (1) |
| low | `Anonimo_TraicionagradecidaLa` | SANDOVAL | 60 | 23/60 (38%) | 2.45 | SANDOVAL (23), QUINONES (19), RUIZALCEO (2), LICENCIADOROJAS (1), RUANO (1) |
| low | `DESCONOCIDO_EscenaComica2` | VIDALYSALVADOR | 36 | 28/36 (78%) | 2.45 | VIDALYSALVADOR (28), AVELLANEDA (4), VERATASSIS (2), VALDIVIELSO (1) |
| low | `ANONIMO_ZarabullequeColombina` | TORRESLORENZODE | 5 | 3/5 (60%) | 2.44 | TORRESLORENZODE (3), SANDOVAL (1), BELMONTE (1) |
| low | `Anonimo_Cuandounadamatienediezgalanesy` | ROMEROROQUE | 17 | 3/17 (18%) | 2.43 | ROMEROROQUE (3), FAJARDOYACEVEDO (3), LICENCIADOROJAS (1), GARCIAMARCOS (1), PAREDES (1) |
| low | `Anonimo_MayorazgodelcieloEl` | LEIVARAMIREZ | 28 | 8/28 (29%) | 2.43 | LEIVARAMIREZ (8), BELMONTE (3), VARGAS (3), GONZALEZDEBARCIA (1), JUANDESOTO (1) |
| low | `ANONIMO_DialogoBritish` | ONAVIEDMAYTORRES | 9 | 8/9 (89%) | 2.41 | ONAVIEDMAYTORRES (8), GONZALEZDETORRES (1) |
| low | `Anonimo_SucesiondelpecadoAutosacrament` | QUEVEDO | 26 | 7/26 (27%) | 2.41 | QUEVEDO (7), BATRES (4), LOPE (3), CALDERON (2), BELMONTE (2) |
| low | `DESCONOCIDO_VariosPapelesDePoesiasADiferentesAsuntos` | VIDALYSALVADOR | 543 | 133/543 (24%) | 2.39 | VIDALYSALVADOR (133), AVELLANEDA (71), MONTALBAN (55), VERATASSIS (54), HURTADODEMENDOZA (35) |
| low | `DESCONOCIDO_Amor` | MELO | 10 | 5/10 (50%) | 2.38 | MELO (5), CASTILLOSOLORZANO (1), LOPEZJACINTO (1) |
| low | `Anonimo_Iryquedarse` | RUIZALCEO | 72 | 27/72 (38%) | 2.38 | RUIZALCEO (27), LEIVARAMIREZ (10), GARCIAMARCOS (10), ROMEROROQUE (7), CASTILLOSOLORZANO (2) |
| low | `DESCONOCIDO_FundaciondeAtenasLa` | CASTILLOSOLORZANO | 33 | 20/33 (61%) | 2.35 | CASTILLOSOLORZANO (20), GODINEZMANRIQUE (6), LOPEZJACINTO (3), MORETO (2), CALDERON (1) |
| low | `Anonimo_MayormagicoeldiabloEl` | LICENCIADOROJAS | 53 | 31/53 (58%) | 2.34 | LICENCIADOROJAS (31), LANINI (9), MEDINA (4), TORRESLORENZODE (1), VARGAS (1) |
| low | `ANONIMO_CercoOrihuela` | CAXESI | 37 | 11/37 (30%) | 2.34 | CAXESI (11), LEIVARAMIREZ (4), CARVAJAL (4), QUEVEDO (4), REMON (3) |
| low | `Anonimo_NuestraSenoradelRosarioytesoro` | GALLEGOS | 34 | 14/34 (41%) | 2.33 | GALLEGOS (14), CLARAMONTE (5), AGUADOELVIEJO (4), LICENCIADOROJAS (1), CANIZARES (1) |
| low | `DESCONOCIDO_FortalezaDelJudaismo` | VARGASMACHUCA | 331 | 170/331 (51%) | 2.32 | VARGASMACHUCA (170), ENRIQUEZ (123), CERVANTES (24), LORENZANA (6), LICENCIADOROJAS (2) |
| low | `MHouse_DelprometeralcumplirCOLOR` | CARVAJAL | 64 | 24/64 (38%) | 2.31 | CARVAJAL (24), VARGAS (18), MULSA (11), TORRESLORENZODE (3), LORENZANA (3) |
| low | `Desconocido_VaqueroEmperador_acto3_Autografo` | SANDOVAL | 46 | 25/46 (54%) | 2.30 | SANDOVAL (25), GILENRIQUEZ (10), VERATASSIS (3), MORETO (3), ROJASZORRILLA (2) |
| low | `Anonimo_SoldadoamercedComediaPrimerays` | GALLEGOS | 44 | 12/44 (27%) | 2.29 | GALLEGOS (12), FAJARDOYACEVEDO (9), HURTADODEMENDOZA (7), CLARAMONTE (4), MOLINAYMENDOZA (1) |
| low | `Anonimo_FeriadelbotijeroLa` | BELMONTE | 62 | 17/62 (27%) | 2.29 | BELMONTE (17), AMESCUA (17), AGUADOELVIEJO (5), MONTALBAN (3), ROJASZORRILLA (3) |
| low | `ANONIMO_LacostureraBritish` | VERATASSIS | 109 | 74/109 (68%) | 2.27 | VERATASSIS (74), LEONORCUEVA (25), GILENRIQUEZ (4), GONGORA (2), CERVANTES (2) |
| low | `Anonimo_Loquepasaentreduenasdoncellasp` | GARCIAMARCOS | 67 | 26/67 (39%) | 2.24 | GARCIAMARCOS (26), ROMEROROQUE (23), MELO (4), PAREDES (3), CASTILLOSOLORZANO (2) |
| low | `Anonimo_Barbaabarbahonrasecata` | GALLEGOS | 58 | 34/58 (59%) | 2.24 | GALLEGOS (34), CLARAMONTE (12), HURTADODEMENDOZA (2), ROMEROROQUE (1) |
| low | `Anonimo_MamolaLa` | CONTRERAS | 14 | 2/14 (14%) | 2.24 | CONTRERAS (2), LICENCIADOROJAS (1), QUINONES (1), CARVAJAL (1) |
| low | `Anonimo_ZurdillodelacostaEl` | BATRES | 69 | 21/69 (30%) | 2.23 | BATRES (21), QUINONES (20), AGUADOELVIEJO (7), ANDOSILLA (4), MULSA (3) |
| low | `DESCONOCIDO_VariasCuriosidades` | VARGASMACHUCA | 377 | 96/377 (26%) | 2.23 | VARGASMACHUCA (96), AVELLANEDA (60), VERATASSIS (53), SANDOVAL (33), PAREDES (19) |
| low | `ANONIMO_ContravirtudnohaydesdichaBritish` | ONAVIEDMAYTORRES | 69 | 36/69 (52%) | 2.21 | ONAVIEDMAYTORRES (36), ROMEROROQUE (13), MELO (6), LEONORCUEVA (4), CERVANTES (3) |
| low | `DESCONOCIDO_LoaNuevaDeNuestraSenora` | ENRIQUEZ | 12 | 5/12 (42%) | 2.21 | ENRIQUEZ (5), CASTILLOSOLORZANO (2), AMESCUA (1), TORRESLORENZODE (1), BELMONTE (1) |
| low | `Anonimo_FindefiestaparalacomediadeLosa` | CASTROYSALAZAR | 7 | 2/7 (29%) | 2.21 | CASTROYSALAZAR (2), GONZALEZDEBARCIA (1), VARGASMACHUCA (1), ROMEROROQUE (1), LICENCIADOROJAS (1) |
| low | `Anonimo_RobodeElenaEl` | GARCIAMARCOS | 84 | 22/84 (26%) | 2.21 | GARCIAMARCOS (22), LOPEZJACINTO (20), CUENCAYARGUELLO (8), QUINONES (6), LORENZANA (4) |
| low | `Anonimo_CaballerodelacruzbermejanEl` | ROMEROROQUE | 30 | 11/30 (37%) | 2.19 | ROMEROROQUE (11), FAJARDOYACEVEDO (5), ALARCON (4), AVELLANEDADELACUEVA (1) |
| low | `Anonimo_FantasmadelagallegaLa` | GILENRIQUEZ | 18 | 4/18 (22%) | 2.17 | GILENRIQUEZ (4), SANDOVAL (3), LICENCIADOROJAS (1), SAAVEDRAFAJARDO (1), BELMONTE (1) |
| low | `Anonimo_ConjuraciondeCatilinaLa` | ROJASVILLANDRANDO | 50 | 15/50 (30%) | 2.15 | ROJASVILLANDRANDO (15), TORRESLORENZODE (11), SALAZARYTORRES (8), TAMAYO (2), CERVANTES (1) |
| low | `Desconocido_AfricanoNeron_acto1yrestosacto3` | GILENRIQUEZ | 47 | 15/47 (32%) | 2.14 | GILENRIQUEZ (15), CANIZARES (12), ROJASZORRILLA (5), DIAMANTE (4), VIDALYSALVADOR (3) |
| low | `DESCONOCIDO_BaileDeRepente` | VIDALYSALVADOR | 36 | 35/36 (97%) | 2.14 | VIDALYSALVADOR (35), LOPEZDELCAMPO (1) |
| low | `ANONIMO_DesenganodeamorEl` | GARCIADEPRADO | 9 | 6/9 (67%) | 2.13 | GARCIADEPRADO (6), VIDALYSALVADOR (1), CERVANTES (1), CARVAJAL (1) |
| low | `DESCONOCIDO_Pilirrica` | VIDALYSALVADOR | 30 | 8/30 (27%) | 2.12 | VIDALYSALVADOR (8), PAREDES (3), QUINONES (2), GARCIADEPRADO (2), DIAMANTE (2) |
| low | `Anonimo_PapagayoEntremesEl` | HOZYMOTA | 14 | 3/14 (21%) | 2.12 | HOZYMOTA (3), LICENCIADOROJAS (1), MOLINAYMENDOZA (1), GARCIADEPRADO (1) |
| low | `Anonimo_TontomaliciosoEl` | SANDOVAL | 11 | 2/11 (18%) | 2.12 | SANDOVAL (2), MOLINAYMENDOZA (2), LEIVARAMIREZ (1), LEONORCUEVA (1) |
| low | `DESCONOCIDO_EstragoEnLaFineza` | VIDALYSALVADOR | 30 | 14/30 (47%) | 2.11 | VIDALYSALVADOR (14), REMON (6), BELMONTE (6), QUEVEDO (3), GILENRIQUEZ (1) |
| low | `Desconocido_Amistadinfelice` | VERATASSIS | 185 | 163/185 (88%) | 2.10 | VERATASSIS (163), GONGORA (6), CASTILLOSOLORZANO (2), VIDALYSALVADOR (1) |
| low | `Anonimo_EsclavodesuhijoEl` | LOPEZDECASTRO | 39 | 22/39 (56%) | 2.06 | LOPEZDECASTRO (22), GOMEZACOSTA (6), LICENCIADOROJAS (1), ROJASVILLANDRANDO (1), RUIZALCEO (1) |
| low | `Anonimo_JuntadelosmedicosLa` | GALLEGOS | 16 | 4/16 (25%) | 2.05 | GALLEGOS (4), CARVAJAL (1), SANDOVAL (1) |
| low | `Anonimo_LoasEntremesLas` | LEONORCUEVA | 18 | 4/18 (22%) | 2.05 | LEONORCUEVA (4), MELO (2), QUINONES (1), TAMAYO (1) |
| low | `DESCONOCIDO_PrincipedonCarlos` | CASTILLOSOLORZANO | 224 | 155/224 (69%) | 2.04 | CASTILLOSOLORZANO (155), CERVANTES (34), CONTRERAS (10), SANTATERESA (3), LEONORCUEVA (3) |
| low | `Anonimo_ValienteJuandeHerediaEl` | ANDOSILLA | 71 | 23/71 (32%) | 2.00 | ANDOSILLA (23), QUINONES (12), LEIVARAMIREZ (8), MOLINAYMENDOZA (7), FAJARDOYACEVEDO (6) |
| low | `Anonimo_SacamuelasEl` | MOLINAYMENDOZA | 14 | 3/14 (21%) | 1.99 | MOLINAYMENDOZA (3), CASTROYSALAZAR (1), CANIZARES (1) |
| low | `Anonimo_MejorblasondeMejicoSanFelipede` | AVELLANEDA | 143 | 88/143 (62%) | 1.97 | AVELLANEDA (88), MELO (17), MEDINA (12), LICENCIADOROJAS (12), LEONORCUEVA (3) |
| low | `Anonimo_PresumidoEl` | FAJARDOYACEVEDO | 14 | 3/14 (21%) | 1.97 | FAJARDOYACEVEDO (3), LICENCIADOROJAS (1), SANDOVAL (1), PAREDES (1), MOLINAYMENDOZA (1) |
| low | `Anonimo_Darbienpormaloelrespetoalsacer` | LICENCIADOROJAS | 52 | 19/52 (36%) | 1.95 | LICENCIADOROJAS (19), FAJARDOYACEVEDO (13), MEDINA (9), CARVAJAL (2), ROMEROROQUE (2) |
| low | `MHouse_PremiodelbienhablarCOLOR` | VARGAS | 62 | 29/62 (47%) | 1.94 | VARGAS (29), MULSA (18), CARVAJAL (10), ROJASVILLANDRANDO (3), MELO (1) |
| low | `DESCONOCIDO_RicoAvariento` | ROJASZORRILLA | 21 | 6/21 (29%) | 1.94 | ROJASZORRILLA (6), LORENZANA (4), BELMONTE (3), REMON (3), CAXESI (1) |
| low | `ANONIMO_AmormejormedicamentocasamientoBritish` | SANDOVAL | 66 | 22/66 (33%) | 1.93 | SANDOVAL (22), CASTROYSALAZAR (19), VERATASSIS (11), MELO (7), GILENRIQUEZ (6) |
| low | `DESCONOCIDO_BurlaDeLosCuencos_Entremes` | LICENCIADOROJAS | 12 | 4/12 (33%) | 1.91 | LICENCIADOROJAS (4), AVELLANEDA (4), LOPEZDECARDENA (2), VALDIVIELSO (1), BARRIONUEVO (1) |
| low | `Anonimo_LadronaLa` | PAREDES | 16 | 4/16 (25%) | 1.91 | PAREDES (4), GONZALEZDEBARCIA (2) |
| low | `ANONIMO_VengarseDarseCelos` | VIDALYSALVADOR | 68 | 22/68 (32%) | 1.89 | VIDALYSALVADOR (22), PAREDES (13), LANINI (9), CASTILLOSOLORZANO (6), MORETO (4) |
| low | `DESCONOCIDO_PrincipeSergio` | SANDOVAL | 75 | 24/75 (32%) | 1.89 | SANDOVAL (24), MELO (17), AVELLANEDA (11), VARGASMACHUCA (6), CARVAJAL (6) |
| low | `Anonimo_Sutilmaranadelosdosfielesypare` | AVELLANEDA | 24 | 8/24 (33%) | 1.88 | AVELLANEDA (8), MEDINA (4), LICENCIADOROJAS (3), CARVAJAL (1), TAMAYO (1) |
| low | `DESCONOCIDO_QuienMasAma` | VIDALYSALVADOR | 4 | 2/4 (50%) | 1.88 | VIDALYSALVADOR (2), MARCHANTE (1), BELMONTE (1) |
| low | `ANONIMO_SaineteBritish` | VERATASSIS | 36 | 31/36 (86%) | 1.87 | VERATASSIS (31), GONGORA (3), LICENCIADOROJAS (1), LEONORCUEVA (1) |
| low | `Anonimo_NoestabadeDios` | HURTADODEMENDOZA | 66 | 30/66 (46%) | 1.87 | HURTADODEMENDOZA (30), QUINONES (25), CECILIANACIMIENTO (2), AMESCUA (2), VIDALYSALVADOR (1) |
| low | `Anonimo_BuenladronymuertedeCristoNuest` | BATRES | 47 | 24/47 (51%) | 1.86 | BATRES (24), LEIVARAMIREZ (9), ROMEROROQUE (2), GALLEGOS (2), MENESES (2) |
| low | `Anonimo_Enmujereshayvenganzayensuvenga` | HOZYMOTA | 47 | 21/47 (45%) | 1.85 | HOZYMOTA (21), ROMEROROQUE (4), TORRESLORENZODE (3), CASTILLOSOLORZANO (3), CAXESI (2) |
| low | `MHouse_CelosdelduqueCOLOR` | CARVAJAL | 38 | 11/38 (29%) | 1.85 | CARVAJAL (11), VILLEGASDELACRUZ (11), ROMEROROQUE (4), CASTILLOSOLORZANO (4), LORENZANA (3) |
| low | `Anonimo_LoafamosadeSanJuanBautista` | BELMONTE | 8 | 2/8 (25%) | 1.81 | BELMONTE (2), GONZALEZDEBARCIA (1), ROJASZORRILLA (1), GALLEGOS (1) |
| low | `Anonimo_SitioyexpugnaciondeBudaEl` | VALDIVIELSO | 95 | 32/95 (34%) | 1.80 | VALDIVIELSO (32), VERATASSIS (10), MONTALBAN (10), MORETO (6), ROSETENINO (6) |
| low | `Anonimo_MarienmantadaLa` | TORRESLORENZODE | 74 | 37/74 (50%) | 1.80 | TORRESLORENZODE (37), MESA (17), COELLO (3), VILLEGASDELACRUZ (3), LOPEZJACINTO (1) |
| low | `ANONIMO_BellaSayaguesa` | BELMONTE | 53 | 14/53 (26%) | 1.80 | BELMONTE (14), PAREDES (10), TORRESLORENZODE (9), VIDALYSALVADOR (9), CASTROYSALAZAR (8) |
| low | `DESCONOCIDO_AmorOlleroDeAlarcon` | VERATASSIS | 12 | 5/12 (42%) | 1.79 | VERATASSIS (5), ROMEROROQUE (1), FAJARDOYACEVEDO (1), CANIZARES (1) |
| low | `Anonimo_NuestraSenoradelRosariooeltira` | ROMEROROQUE | 29 | 6/29 (21%) | 1.77 | ROMEROROQUE (6), SANDOVAL (5), CASTILLOSOLORZANO (3), GONZALEZDEBARCIA (1), FAJARDOYACEVEDO (1) |
| low | `Anonimo_PorfiadoEl` | HURTADODEMENDOZA | 12 | 3/12 (25%) | 1.77 | HURTADODEMENDOZA (3), FAJARDOYACEVEDO (2), LICENCIADOROJAS (1) |
| low | `Anonimo_InteresbandoleroEl` | SANDOVAL | 10 | 4/10 (40%) | 1.76 | SANDOVAL (4), CASTILLOSOLORZANO (1), GONZALEZDEBARCIA (1), QUEVEDO (1) |
| low | `DESCONOCIDO_DelSantisimoSacramento` | CERVANTES | 33 | 17/33 (52%) | 1.75 | CERVANTES (17), VILLEGASDELACRUZ (8), VARGASMACHUCA (2), CORDERO (1), TAMAYO (1) |
| low | `ANONIMO_LechugasLas` | VARGASMACHUCA | 7 | 6/7 (86%) | 1.74 | VARGASMACHUCA (6), CECILIANACIMIENTO (1) |
| low | `DESCONOCIDO_EscenaComica1` | VIDALYSALVADOR | 32 | 26/32 (81%) | 1.72 | VIDALYSALVADOR (26), ENRIQUEZ (2), QUEVEDO (2), VARGASMACHUCA (1) |
| low | `Variasmanos_MejorAmigoMuerto_foliossueltos_Autografo` | CALDERON | 25 | 9/25 (36%) | 1.71 | CALDERON (9), MENESES (4), VARGASMACHUCA (1), BATRES (1), MONTALBAN (1) |
| low | `DESCONOCIDO_ConsejoDeInquisicion1670` | QUEVEDO | 260 | 73/260 (28%) | 1.70 | QUEVEDO (73), ENRIQUEZ (41), GARCIADEPRADO (25), HURTADODEMENDOZA (23), AVELLANEDA (16) |
| low | `ANONIMO_FragmentosAltamira42` | CECILIANACIMIENTO | 8 | 7/8 (88%) | 1.70 | CECILIANACIMIENTO (7), LEONORCUEVA (1) |
| low | `Anonimo_RufianesLos` | CANIZARES | 16 | 2/16 (12%) | 1.70 | CANIZARES (2), CONTRERAS (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), SAAVEDRAFAJARDO (1) |
| low | `MHouse_CautivoporsudamaCOLOR` | TORRESLORENZODE | 64 | 17/64 (27%) | 1.69 | TORRESLORENZODE (17), ENRIQUEZ (15), VARGAS (10), VERATASSIS (6), SANDOVAL (5) |
| low | `DESCONOCIDO_PachecosYPalomeques` | CANIZARES | 55 | 18/55 (33%) | 1.69 | CANIZARES (18), HOZYMOTA (15), GILENRIQUEZ (5), CAXESI (4), CARVAJAL (4) |
| low | `Anonimo_JardinencantadoEl` | GILENRIQUEZ | 14 | 4/14 (29%) | 1.68 | GILENRIQUEZ (4), GONZALEZDEBARCIA (2), MOLINAYMENDOZA (2), SANDOVAL (2), LEONORCUEVA (1) |
| low | `DESCONOCIDO_TontoDeLasBatuecas` | CASTILLOSOLORZANO | 18 | 6/18 (33%) | 1.68 | CASTILLOSOLORZANO (6), GARCIAMARCOS (4), PAREDES (3), VIDALYSALVADOR (2), LOPEZJACINTO (1) |
| low | `DESCONOCIDO_TresMayoresProdigios` | LANINI | 54 | 25/54 (46%) | 1.66 | LANINI (25), MORETO (12), MULSA (9), GARCIAMARCOS (2), TORRESLORENZODE (2) |
| low | `Anonimo_TutilimundiEl` | LEIVARAMIREZ | 16 | 3/16 (19%) | 1.65 | LEIVARAMIREZ (3), ALARCON (3) |
| low | `Anonimo_LucesdelEvangelioSanSimonyJuda` | VERATASSIS | 62 | 27/62 (44%) | 1.64 | VERATASSIS (27), VIDALYSALVADOR (13), VALDIVIELSO (8), AVELLANEDA (3), LICENCIADOROJAS (1) |
| low | `Anonimo_VictoriadeFuenterrabiaLa` | JIMENEZSEDENO | 72 | 7/72 (10%) | 1.64 | JIMENEZSEDENO (7), CALDERON (5), CALLE (5), GILENRIQUEZ (3), ANDOSILLA (3) |
| low | `DESCONOCIDO_EnsenarseASerBuenRey` | HOZYMOTA | 43 | 23/43 (54%) | 1.61 | HOZYMOTA (23), CANIZARES (10), CAXESI (4), LICENCIADOROJAS (1), AVELLANEDADELACUEVA (1) |
| low | `DESCONOCIDO_Cancionero` | ENRIQUEZ | 387 | 162/387 (42%) | 1.60 | ENRIQUEZ (162), CERVANTES (84), QUINONES (44), CONTRERAS (24), MULSA (11) |
| low | `DESCONOCIDO_Teatrodecolegio` | GONZALEZDEBARCIA | 4 | 2/4 (50%) | 1.60 | GONZALEZDEBARCIA (2), CONTRERAS (1), CERVANTES (1) |
| low | `DESCONOCIDO_TesoroescondidoEl` | CALLE | 77 | 36/77 (47%) | 1.58 | CALLE (36), GONZALEZDETORRES (6), GONZALEZDEBARCIA (6), GARCIAMARCOS (5), SARAVIAYMENDOZA (5) |
| low | `DESCONOCIDO_MasHeroicaRomana` | GONGORA | 126 | 57/126 (45%) | 1.56 | GONGORA (57), VIDALYSALVADOR (20), GILENRIQUEZ (16), CANIZARES (9), GARCIADEPRADO (6) |
| low | `Anonimo_CaballerodeOlmedooLaviudaporca` | ROJASVILLANDRANDO | 71 | 21/71 (30%) | 1.55 | ROJASVILLANDRANDO (21), TAMAYO (8), VILLEGASDELACRUZ (6), TORRESLORENZODE (5), GALLEGOS (4) |
| low | `DESCONOCIDO_MayorTriunfoDeAmor1` | VARGASMACHUCA | 158 | 71/158 (45%) | 1.54 | VARGASMACHUCA (71), VIDALYSALVADOR (70), MELO (3), GONGORA (2), JIMENEZSEDENO (1) |
| low | `ANONIMO_FragmentosAltamira40` | GONZALEZDEBARCIA | 7 | 5/7 (71%) | 1.52 | GONZALEZDEBARCIA (5), CERVANTES (1), CASTILLOSOLORZANO (1) |
| low | `Anonimo_Vencerconhumildadelambiciondel` | CASTILLOSOLORZANO | 35 | 7/35 (20%) | 1.50 | CASTILLOSOLORZANO (7), MEDINA (6), ROMEROROQUE (5), JUANDESOTO (5), CARVAJAL (2) |
| low | `Anonimo_CautivadeventurosayperseguidaR` | ROJASVILLANDRANDO | 66 | 18/66 (27%) | 1.50 | ROJASVILLANDRANDO (18), BATRES (15), ENRIQUEZ (12), CASTILLOSOLORZANO (3), GONZALEZDEBARCIA (2) |
| low | `DESCONOCIDO_PetimetreBurlado` | VERATASSIS | 54 | 27/54 (50%) | 1.49 | VERATASSIS (27), SANDOVAL (12), LOPEZDECARDENA (5), MEDINA (4), LICENCIADOROJAS (2) |
| low | `Anonimo_ManadelcieloEl` | HURTADODEMENDOZA | 30 | 12/30 (40%) | 1.48 | HURTADODEMENDOZA (12), GONGORA (8), LICENCIADOROJAS (1) |
| low | `MHouse_NohaycienciacontraelamorCOLOR` | CARVAJAL | 61 | 20/61 (33%) | 1.47 | CARVAJAL (20), SANDOVAL (12), VARGAS (10), MULSA (7), VERATASSIS (2) |
| low | `Anonimo_EntremesquesehizoenelautodeQui` | FAJARDOYACEVEDO | 18 | 3/18 (17%) | 1.46 | FAJARDOYACEVEDO (3), AVELLANEDADELACUEVA (2), JUANDESOTO (2), LOPEZJACINTO (1), ALARCON (1) |
| low | `DESCONOCIDO_Primerapartecomediasviejas` | VIDALYSALVADOR | 3 | 2/3 (67%) | 1.45 | VIDALYSALVADOR (2), AVELLANEDA (1) |
| low | `DESCONOCIDO_NuestrasenoradelaPobeda` | GARCIADEPRADO | 68 | 25/68 (37%) | 1.45 | GARCIADEPRADO (25), CERVANTES (19), CALDERON (7), HURTADODEMENDOZA (6), GONGORA (6) |
| low | `Anonimo_IndianoincreduloEl` | BOLEAYALVARADO | 16 | 3/16 (19%) | 1.45 | BOLEAYALVARADO (3), ANDOSILLA (2), CARVAJAL (1), QUINONES (1), CANIZARES (1) |
| low | `Anonimo_FenixElJuanRana` | LEIVARAMIREZ | 10 | 3/10 (30%) | 1.44 | LEIVARAMIREZ (3), FAJARDOYACEVEDO (2), GONZALEZDEBARCIA (1), ANDOSILLA (1), MENESES (1) |
| low | `Anonimo_DonAsmodeooElpoetaastrologo` | TORRESLORENZODE | 10 | 3/10 (30%) | 1.42 | TORRESLORENZODE (3), GONZALEZDEBARCIA (1), LANINI (1), CASTROYSALAZAR (1), MORETO (1) |
| low | `Anonimo_Florinda` | HOZYMOTA | 12 | 1/12 (8%) | 1.41 | HOZYMOTA (1), MATOSFRAGOSO (1), MORETO (1), BATRES (1) |
| low | `Anonimo_GallegasLas` | GONZALEZDEBARCIA | 10 | 3/10 (30%) | 1.40 | GONZALEZDEBARCIA (3), FAJARDOYACEVEDO (2), CERVANTES (1), ROMEROROQUE (1), LEONORCUEVA (1) |
| low | `ANONIMO_VerdadyeltiempoLa` | AVELLANEDADELACUEVA | 3 | 1/3 (33%) | 1.40 | AVELLANEDADELACUEVA (1), CONTRERAS (1), DIAMANTE (1) |
| low | `Anonimo_LicenciadoMoclinEl` | GARCIADEPRADO | 12 | 2/12 (17%) | 1.40 | GARCIADEPRADO (2), LICENCIADOROJAS (1), CASTILLOSOLORZANO (1), ALARCON (1) |
| low | `DESCONOCIDO_EmpenoHaceLaOfensa` | CASTILLOSOLORZANO | 20 | 6/20 (30%) | 1.40 | CASTILLOSOLORZANO (6), GOMEZACOSTA (4), VARGASMACHUCA (4), ROMEROROQUE (2), PAREDES (1) |
| low | `DESCONOCIDO_Arcabuceado` | DIAMANTE | 12 | 3/12 (25%) | 1.37 | DIAMANTE (3), ANDOSILLA (2), AMESCUA (1), FAJARDOYACEVEDO (1) |
| low | `DESCONOCIDO_AAveriguadosCelosNoHayPrudencia` | ENRIQUEZ | 61 | 18/61 (30%) | 1.34 | ENRIQUEZ (18), TORRESLORENZODE (11), ALARCON (4), COELLO (3), LEIVARAMIREZ (3) |
| low | `DESCONOCIDO_LoaparaLasvictoriasdeamor` | HURTADODEMENDOZA | 46 | 17/46 (37%) | 1.34 | HURTADODEMENDOZA (17), GONZALEZDEBARCIA (10), MULSA (9) |
| low | `DESCONOCIDO_TragediaSantaCaterinaAlejandria` | BENAVIDES | 53 | 30/53 (57%) | 1.33 | BENAVIDES (30), VARGASMACHUCA (9), AVELLANEDA (8), SANDOVAL (2), MELO (2) |
| low | `DESCONOCIDO_JardinDeEspana` | AVELLANEDA | 11 | 7/11 (64%) | 1.31 | AVELLANEDA (7), VERATASSIS (1), LICENCIADOROJAS (1), VIDALYSALVADOR (1), LEONORCUEVA (1) |
| low | `DESCONOCIDO_AnardaYPascual` | VERATASSIS | 8 | 2/8 (25%) | 1.31 | VERATASSIS (2), LEONORCUEVA (1), CASTILLOSOLORZANO (1), MONTALBAN (1), CANIZARES (1) |
| low | `DESCONOCIDO_PescadorDeCana` | CECILIANACIMIENTO | 10 | 3/10 (30%) | 1.31 | CECILIANACIMIENTO (3), MARCHANTE (2), VALDIVIELSO (1), GOMEZACOSTA (1), LOPEZDECASTRO (1) |
| low | `Anonimo_VenturasinbuscarlaLa` | ROMEROROQUE | 29 | 9/29 (31%) | 1.29 | ROMEROROQUE (9), CANIZARES (5), CASTROYSALAZAR (4), GONZALEZDEBARCIA (1), CAXESI (1) |
| low | `Anonimo_LazarillosLos` | SANDOVAL | 9 | 3/9 (33%) | 1.27 | SANDOVAL (3), ROMEROROQUE (1), FAJARDOYACEVEDO (1) |
| low | `Anonimo_TriunfosdeamorydesdenDaphneyAp` | MELO | 42 | 11/42 (26%) | 1.27 | MELO (11), GONZALEZDEBARCIA (10), CANIZARES (7), RUANO (5), GRACIAN (2) |
| low | `Anonimo_LucerodelsolSanJuanBautistaEl` | AGUADOELVIEJO | 109 | 62/109 (57%) | 1.27 | AGUADOELVIEJO (62), MESA (10), MIRACLESSOTOMAYOR (9), VARGAS (3), MULSA (3) |
| low | `DESCONOCIDO_Commission` | MIRACLESSOTOMAYOR | 31 | 26/31 (84%) | 1.26 | MIRACLESSOTOMAYOR (26), GONZALEZDEBARCIA (1), HURTADODEMENDOZA (1), SANTATERESA (1), AMESCUA (1) |
| low | `Anonimo_LocosLos` | TORRESLORENZODE | 15 | 4/15 (27%) | 1.24 | TORRESLORENZODE (4), PAREDES (2), LICENCIADOROJAS (1), ROMEROROQUE (1) |
| low | `Anonimo_ConquistadeToledoLa` | VIDALYSALVADOR | 52 | 19/52 (36%) | 1.23 | VIDALYSALVADOR (19), MOLINAYMENDOZA (6), GONZALEZDEBARCIA (5), CASTILLOSOLORZANO (2), HOZYMOTA (2) |
| low | `DESCONOCIDO_AmorSastre` | FAJARDOYACEVEDO | 12 | 4/12 (33%) | 1.23 | FAJARDOYACEVEDO (4), SANDOVAL (1), VIDALYSALVADOR (1), MOLINAYMENDOZA (1), HURTADODEMENDOZA (1) |
| low | `DESCONOCIDO_ListFromAutoDeFe` | LEONORCUEVA | 6 | 5/6 (83%) | 1.23 | LEONORCUEVA (5), CERVANTES (1) |
| low | `DESCONOCIDO_TresPrimerosMisterios` | GONGORA | 52 | 23/52 (44%) | 1.22 | GONGORA (23), QUEVEDO (10), CASTROYSALAZAR (6), SANDOVAL (5), GILENRIQUEZ (4) |
| low | `DESCONOCIDO_MatarsePorNoMorirse` | GONGORA | 39 | 13/39 (33%) | 1.21 | GONGORA (13), QUEVEDO (10), CANIZARES (4), AVELLANEDADELACUEVA (3), ENRIQUEZ (2) |
| low | `Anonimo_LicenciadoestupendoEl` | LOPEZDECASTRO | 20 | 6/20 (30%) | 1.20 | LOPEZDECASTRO (6), CASTILLOSOLORZANO (2), LICENCIADOROJAS (1), GONZALEZDETORRES (1) |
| low | `DESCONOCIDO_Roncesvalles` | JUANDESOTO | 42 | 15/42 (36%) | 1.20 | JUANDESOTO (15), TORRESLORENZODE (13), CASTILLOSOLORZANO (4), GONZALEZDETORRES (4), GOMEZACOSTA (2) |
| low | `Anonimo_CorredordenoviosEl` | CANIZARES | 17 | 2/17 (12%) | 1.18 | CANIZARES (2), GONZALEZDEBARCIA (1), CASTILLOSOLORZANO (1), FAJARDOYACEVEDO (1), GARCIADEPRADO (1) |
| low | `Anonimo_MojigangaparafiestadeCorpusdee` | MOLINAYMENDOZA | 10 | 7/10 (70%) | 1.15 | MOLINAYMENDOZA (7), BANCESCANDAMO (1), BELMONTE (1), SANDOVAL (1) |
| low | `DESCONOCIDO_ConsejoDeInquisicion1596-1597` | VARGASMACHUCA | 60 | 12/60 (20%) | 1.15 | VARGASMACHUCA (12), HURTADODEMENDOZA (7), GARCIADEPRADO (4), CECILIANACIMIENTO (4), GONGORA (3) |
| low | `DESCONOCIDO_ManuscritosMiscelaneos` | AVELLANEDA | 4 | 1/4 (25%) | 1.14 | AVELLANEDA (1), QUINONES (1), CUEVAYSILVA (1), CERVANTES (1) |
| low | `Desconocido_jornadaburlesca` | MELO | 559 | 326/559 (58%) | 1.14 | MELO (326), VARGASMACHUCA (85), QUEVEDO (20), CASTROYSALAZAR (15), VIDALYSALVADOR (12) |
| low | `MHouse_MasvalefingirqueamarCOLOR` | MEDINA | 66 | 16/66 (24%) | 1.14 | MEDINA (16), VARGAS (12), SANDOVAL (9), VERATASSIS (8), MELO (7) |
| low | `DESCONOCIDO_LettereDiDiversiPrincipi` | HURTADODEMENDOZA | 113 | 55/113 (49%) | 1.12 | HURTADODEMENDOZA (55), CERVANTES (24), VARGASMACHUCA (21), GONGORA (2), ANDOSILLA (1) |
| low | `Anonimo_SalteadorventurosooAutodenuest` | LOPEZDECASTRO | 38 | 8/38 (21%) | 1.12 | LOPEZDECASTRO (8), VILLEGASJUANBAUTISTA (5), ONAVIEDMAYTORRES (4), ROMEROROQUE (3), VILLEGASDELACRUZ (3) |
| low | `DESCONOCIDO_AlOficialGeringado` | MORETO | 28 | 11/28 (39%) | 1.11 | MORETO (11), CARVAJAL (7), CASTILLOSOLORZANO (5), LORENZANA (2), CERVANTES (2) |
| low | `Anonimo_MazalquivirEl` | GOMEZACOSTA | 14 | 2/14 (14%) | 1.09 | GOMEZACOSTA (2), BOLEAYALVARADO (1), CAXESI (1) |
| low | `Anonimo_PapagayoEl` | FAJARDOYACEVEDO | 16 | 2/16 (12%) | 1.09 | FAJARDOYACEVEDO (2), CASTILLOSOLORZANO (1), LEIVARAMIREZ (1), MOLINAYMENDOZA (1), GARCIADEPRADO (1) |
| low | `DESCONOCIDO_Cirodescubierto` | CERVANTES | 50 | 35/50 (70%) | 1.08 | CERVANTES (35), LICENCIADOROJAS (7), CECILIANACIMIENTO (3), VIDALYSALVADOR (2), LOPEZDELCAMPO (1) |
| low | `Anonimo_MayortriunfodeVenusEl` | GARCIADEPRADO | 61 | 28/61 (46%) | 1.08 | GARCIADEPRADO (28), VIDALYSALVADOR (8), CASTILLOSOLORZANO (4), GONZALEZDEBARCIA (3), ENRIQUEZ (3) |
| low | `DESCONOCIDO_ConsejoDeInquisicion1662` | ANDOSILLA | 2 | 1/2 (50%) | 1.08 | ANDOSILLA (1), CASTILLOSOLORZANO (1) |
| low | `DESCONOCIDO_AsunciondeNuestraSenora2` | QUINONES | 56 | 27/56 (48%) | 1.07 | QUINONES (27), SANTATERESA (4), AVELLANEDADELACUEVA (4), COELLO (2), VARGASMACHUCA (2) |
| low | `DESCONOCIDO_HastaEnAmarHayFortuna` | CERVANTES | 88 | 35/88 (40%) | 1.06 | CERVANTES (35), TORRESLORENZODE (13), SANDOVAL (12), AVELLANEDA (11), LANINI (4) |
| low | `Anonimo_NopuedeserComediaentresjornada` | VERATASSIS | 33 | 18/33 (55%) | 1.06 | VERATASSIS (18), CERVANTES (4), ENRIQUEZ (3), LICENCIADOROJAS (1), CLARAMONTE (1) |
| low | `Anonimo_TajadasLas` | GONZALEZDEBARCIA | 15 | 3/15 (20%) | 1.05 | GONZALEZDEBARCIA (3), VARGAS (2), ROMEROROQUE (1) |
| low | `Anonimo_PleitodelasduenasyescuderosEl` | FAJARDOYACEVEDO | 16 | 4/16 (25%) | 1.03 | FAJARDOYACEVEDO (4), GALLEGOS (2), CASTILLOSOLORZANO (1), ALARCON (1) |
| low | `DESCONOCIDO_ElTestamentoDeLosLadrones` | SALAZARYTORRES | 9 | 2/9 (22%) | 1.03 | SALAZARYTORRES (2), LICENCIADOROJAS (2), CERVANTES (1), MEDINA (1), BOLEAYALVARADO (1) |
| low | `ANONIMO_DesertorBritish` | GONGORA | 69 | 50/69 (72%) | 1.01 | GONGORA (50), VERATASSIS (12), CERVANTES (3), VARGASMACHUCA (1), LICENCIADOROJAS (1) |
| low | `Anonimo_ComediasintitulosobreSanRamonN` | CONTRERAS | 17 | 7/17 (41%) | 1.00 | CONTRERAS (7), CORDERO (4), ROJASVILLANDRANDO (2), COELLO (1), CAXESI (1) |
| low | `DESCONOCIDO_AbrahamDelYermo` | BELMONTE | 51 | 7/51 (14%) | 1.00 | BELMONTE (7), BATRES (7), ROMEROROQUE (6), CASTILLOSOLORZANO (5), CAXESI (4) |
| low | `Anonimo_MejorhijodeMadridSanDamasoEl` | CANIZARES | 58 | 26/58 (45%) | 0.99 | CANIZARES (26), GONGORA (10), CASTROYSALAZAR (4), GONZALEZDEBARCIA (4), BOLEAYALVARADO (2) |
| low | `Anonimo_MatachinesLos` | ENRIQUEZ | 27 | 3/27 (11%) | 0.97 | ENRIQUEZ (3), LANINI (2), CARVAJAL (1), AMESCUA (1), PAREDES (1) |
| low | `DESCONOCIDO_MalContenta` | VIDALYSALVADOR | 12 | 3/12 (25%) | 0.97 | VIDALYSALVADOR (3), COELLO (1), BATRES (1), LOPEZDELCAMPO (1), MATOSFRAGOSO (1) |
| low | `Anonimo_MudanzasLas` | MENESES | 29 | 5/29 (17%) | 0.95 | MENESES (5), LEIVARAMIREZ (2), MONTALBAN (1), CONTRERAS (1), LEONORCUEVA (1) |
| low | `Anonimo_LoaasusenoriaelsenorcondedeGon` | LEONORCUEVA | 6 | 1/6 (17%) | 0.93 | LEONORCUEVA (1), GONGORA (1), ROMEROROQUE (1), CASTILLOSOLORZANO (1) |
| low | `Anonimo_Ventayventeroenunapieza` | MORETO | 10 | 2/10 (20%) | 0.92 | MORETO (2), MENESES (2), TAMAYO (1) |
| low | `DESCONOCIDO_DialogoentreEspanaynobleza` | CARVAJAL | 5 | 2/5 (40%) | 0.89 | CARVAJAL (2), MATOSFRAGOSO (1), TORRESLORENZODE (1), VIDALYSALVADOR (1) |
| low | `MHouse_PerdidasdelquejuegaCOLOR` | SANDOVAL | 63 | 19/63 (30%) | 0.89 | SANDOVAL (19), VARGAS (19), CARVAJAL (9), MONTALBAN (4), VERATASSIS (3) |
| low | `Anonimo_SacristanyelpuercoEl` | GALLEGOS | 16 | 3/16 (19%) | 0.89 | GALLEGOS (3), CANIZARES (2), QUINONES (1) |
| low | `Anonimo_Tercerosparaelcieloydevocionde` | AVELLANEDA | 33 | 8/33 (24%) | 0.88 | AVELLANEDA (8), CUEVAYSILVA (5), MEDINA (4), CORDERO (2), CECILIANACIMIENTO (1) |
| low | `DESCONOCIDO_ComediaSinTitulo_PalacioRealMadrid` | PACHECO | 69 | 36/69 (52%) | 0.87 | PACHECO (36), MIRACLESSOTOMAYOR (19), MEDINA (7), CUEVAYSILVA (5), LOPEZDECASTRO (2) |
| low | `ANONIMO_AmorlovencetodoBritish` | CARVAJAL | 61 | 41/61 (67%) | 0.86 | CARVAJAL (41), CERVANTES (10), GARCIADEPRADO (4), AVELLANEDADELACUEVA (3), ROMEROROQUE (1) |
| low | `DESCONOCIDO_Entreacto` | CORDERO | 2 | 1/2 (50%) | 0.85 | CORDERO (1), CASTILLOSOLORZANO (1) |
| low | `Anonimo_SoldadoyGilaEl` | CASTILLOSOLORZANO | 10 | 2/10 (20%) | 0.85 | CASTILLOSOLORZANO (2), MOLINAYMENDOZA (2), CANIZARES (1), GILENRIQUEZ (1) |
| low | `Anonimo_Justiciaaluso` | FAJARDOYACEVEDO | 10 | 2/10 (20%) | 0.83 | FAJARDOYACEVEDO (2), MOLINAYMENDOZA (1), LORENZANA (1) |
| low | `Anonimo_PlazamayorporNavidadLa` | CASTROYSALAZAR | 12 | 3/12 (25%) | 0.83 | CASTROYSALAZAR (3), LEONORCUEVA (1), LOPEZJACINTO (1), MOLINAYMENDOZA (1), MELO (1) |
| low | `DESCONOCIDO_JuanBragado` | QUINONES | 12 | 5/12 (42%) | 0.82 | QUINONES (5), BATRES (2), ENRIQUEZ (2), VIDALYSALVADOR (1), CONTRERAS (1) |
| low | `Anonimo_Mojigangafamosa` | LEIVARAMIREZ | 14 | 3/14 (21%) | 0.82 | LEIVARAMIREZ (3), CARVAJAL (1), CLARAMONTE (1) |
| low | `Anonimo_SilvoEl` | LICENCIADOROJAS | 12 | 1/12 (8%) | 0.81 | LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), ROMEROROQUE (1), GALLEGOS (1), LOPEZDECASTRO (1) |
| low | `Anonimo_EnganodelavictoriaysitiodeYelv` | CORDERO | 16 | 3/16 (19%) | 0.80 | CORDERO (3), JIMENEZSEDENO (1), MELO (1) |
| low | `Anonimo_MarcosdeSevillaLos` | BELMONTE | 13 | 1/13 (8%) | 0.80 | BELMONTE (1), ANDOSILLA (1), MESA (1), QUINONES (1) |
| low | `Desconocido_CatalanSerrallonga_acto2_Autografo` | QUINONES | 36 | 11/36 (31%) | 0.80 | QUINONES (11), BATRES (6), ENRIQUEZ (5), GARCIADEPRADO (5), CALDERON (2) |
| low | `Anonimo_PeriquilloeldeMadrid` | GARCIAMARCOS | 15 | 4/15 (27%) | 0.80 | GARCIAMARCOS (4), FAJARDOYACEVEDO (1), JIMENEZSEDENO (1) |
| low | `Anonimo_LoaparaempezarenLisboa` | CERVANTES | 8 | 1/8 (12%) | 0.80 | CERVANTES (1), BELMONTE (1), FAJARDOYACEVEDO (1), BATRES (1) |
| low | `DESCONOCIDO_CriticoDeModa` | QUEVEDO | 15 | 7/15 (47%) | 0.79 | QUEVEDO (7), LEIVARAMIREZ (7) |
| low | `Anonimo_FiliyDanteo` | PAREDES | 7 | 2/7 (29%) | 0.75 | PAREDES (2), CASTILLOSOLORZANO (1), VIDALYSALVADOR (1), LANINI (1) |
| low | `DESCONOCIDO_CualEsElMayorTesoro` | QUINONES | 27 | 10/27 (37%) | 0.73 | QUINONES (10), HURTADODEMENDOZA (6), MIRACLESSOTOMAYOR (2), ROMEROROQUE (2), ANDOSILLA (2) |
| low | `Anonimo_Orozcoenamorado` | CONTRERAS | 20 | 2/20 (10%) | 0.73 | CONTRERAS (2), SARAVIAYMENDOZA (2), VARGASMACHUCA (1), GONGORA (1), CORDERO (1) |
| low | `DESCONOCIDO_ElPeso` | CANIZARES | 8 | 2/8 (25%) | 0.71 | CANIZARES (2), SANDOVAL (2), GONZALEZDEBARCIA (1), GILENRIQUEZ (1), BELMONTE (1) |
| low | `DESCONOCIDO_MuzicaNarciso_nosolicitado` | JIMENEZSEDENO | 12 | 5/12 (42%) | 0.69 | JIMENEZSEDENO (5), LANINI (2), MOLINAYMENDOZA (2), AVELLANEDA (1), PAREDES (1) |
| low | `Anonimo_RondaLa` | MONTALBAN | 15 | 3/15 (20%) | 0.69 | MONTALBAN (3), DIAMANTE (1), ROJASZORRILLA (1), BELMONTE (1) |
| low | `Anonimo_OposicionLa` | GONZALEZDEBARCIA | 14 | 5/14 (36%) | 0.64 | GONZALEZDEBARCIA (5), FAJARDOYACEVEDO (4), VIDALYSALVADOR (1) |
| low | `DESCONOCIDO_SenoraMariPerez` | QUEVEDO | 75 | 41/75 (55%) | 0.64 | QUEVEDO (41), SANDOVAL (19), GILENRIQUEZ (4), CERVANTES (3), GONGORA (3) |
| low | `DESCONOCIDO_CarreteroDeLaMancha` | MEDINA | 40 | 11/40 (28%) | 0.62 | MEDINA (11), AVELLANEDADELACUEVA (8), REMON (5), SANTATERESA (5), VARGAS (5) |
| low | `Anonimo_TorosLos` | QUINONES | 16 | 3/16 (19%) | 0.62 | QUINONES (3), CERVANTES (1), CUENCAYARGUELLO (1), AGUADOELVIEJO (1), CARVAJAL (1) |
| low | `ANONIMO_Honestainfamada` | VALDIVIELSO | 58 | 14/58 (24%) | 0.62 | VALDIVIELSO (14), ENRIQUEZ (8), GONGORA (7), CECILIANACIMIENTO (6), MARCHANTE (5) |
| low | `DESCONOCIDO_HonorContraElPoder` | SARAVIAYMENDOZA | 155 | 34/155 (22%) | 0.61 | SARAVIAYMENDOZA (34), VIDALYSALVADOR (26), VERATASSIS (20), CERVANTES (14), ENRIQUEZ (13) |
| low | `MHouse_PrivilegiodelasmujeresCOLOR` | VARGAS | 66 | 24/66 (36%) | 0.59 | VARGAS (24), JUANDESOTO (13), MULSA (8), CERVANTES (4), MELO (2) |
| low | `DESCONOCIDO_ElAmorQueElOdio` | CERVANTES | 196 | 67/196 (34%) | 0.58 | CERVANTES (67), VERATASSIS (61), GONGORA (12), CALLE (12), SANDOVAL (10) |
| low | `Anonimo_ForasteroenlaCorteEl` | MULSA | 25 | 6/25 (24%) | 0.56 | MULSA (6), HURTADODEMENDOZA (5), GARCIADEPRADO (4), GONZALEZDEBARCIA (2), VERATASSIS (2) |
| low | `Anonimo_LadrondelsacramentoyelminondeB` | GARCIAMARCOS | 70 | 16/70 (23%) | 0.56 | GARCIAMARCOS (16), CORDERO (13), RUIZALCEO (10), ROMEROROQUE (10), ENRIQUEZ (2) |
| low | `DESCONOCIDO_Pardo` | CASTILLOSOLORZANO | 18 | 9/18 (50%) | 0.56 | CASTILLOSOLORZANO (9), JIMENEZSEDENO (5), VIDALYSALVADOR (1), CERVANTES (1) |
| low | `ANONIMO_FragmentosAltamira33` | VARGASMACHUCA | 4 | 1/4 (25%) | 0.54 | VARGASMACHUCA (1), CERVANTES (1), GODINEZMANRIQUE (1), CASTILLOSOLORZANO (1) |
| low | `DESCONOCIDO_QueSolaEstaLaCorte` | LICENCIADOROJAS | 12 | 1/12 (8%) | 0.50 | LICENCIADOROJAS (1), CASTILLOSOLORZANO (1), FAJARDOYACEVEDO (1), ROMEROROQUE (1), CALLE (1) |
| low | `DESCONOCIDO_DefensadelalmaLa` | CERVANTES | 24 | 13/24 (54%) | 0.49 | CERVANTES (13), CASTILLOSOLORZANO (5), ENRIQUEZ (2), VARGASMACHUCA (1), BANCESCANDAMO (1) |
| low | `DESCONOCIDO_MiscellaneousManuscripts` | AVELLANEDA | 14 | 1/14 (7%) | 0.47 | AVELLANEDA (1), CECILIANACIMIENTO (1), VIDALYSALVADOR (1), LICENCIADOROJAS (1), QUEVEDO (1) |
| low | `DESCONOCIDO_LoaDeUnBorrachoParaLaFiestaDelSantisimoSacramento` | GALLEGOS | 6 | 2/6 (33%) | 0.46 | GALLEGOS (2), HURTADODEMENDOZA (1), QUINONES (1) |
| low | `DESCONOCIDO_SanFranciscoDePaula` | VERATASSIS | 54 | 15/54 (28%) | 0.44 | VERATASSIS (15), SANDOVAL (10), QUEVEDO (8), GONGORA (7), GILENRIQUEZ (6) |
| low | `Anonimo_SacristiadeMocejonLa` | BATRES | 15 | 2/15 (13%) | 0.43 | BATRES (2), CARVAJAL (1), ENRIQUEZ (1), TORRESLORENZODE (1), FAJARDOYACEVEDO (1) |
| low | `DESCONOCIDO_MorirPorCumplir` | VARGASMACHUCA | 193 | 95/193 (49%) | 0.40 | VARGASMACHUCA (95), GONGORA (31), CECILIANACIMIENTO (17), VERATASSIS (10), ONAVIEDMAYTORRES (9) |
| low | `DESCONOCIDO_Estrechos` | QUEVEDO | 13 | 4/13 (31%) | 0.40 | QUEVEDO (4), TORRESLORENZODE (3), LEIVARAMIREZ (2), CERVANTES (1), SANDOVAL (1) |
| low | `DESCONOCIDO_ElZurdilloSegundaParte` | GARCIAMARCOS | 6 | 3/6 (50%) | 0.39 | GARCIAMARCOS (3), ANDOSILLA (1), JIMENEZSEDENO (1), MOLINAYMENDOZA (1) |
| low | `DESCONOCIDO_FalsificacionGongora` | VALDIVIELSO | 2 | 2/2 (100%) | 0.39 | VALDIVIELSO (2) |
| low | `DESCONOCIDO_Peorestaqueestabayenfermarconelremedio` | HURTADODEMENDOZA | 3 | 1/3 (33%) | 0.39 | HURTADODEMENDOZA (1), GARCIADEPRADO (1), CARVAJAL (1) |
| low | `DESCONOCIDO_Loapanegirica` | GONGORA | 9 | 4/9 (44%) | 0.38 | GONGORA (4), VARGASMACHUCA (2), CERVANTES (2), VIDALYSALVADOR (1) |
| low | `DESCONOCIDO_PrincipeIgnorante` | SANDOVAL | 44 | 9/44 (20%) | 0.38 | SANDOVAL (9), GONGORA (9), QUINONES (5), HURTADODEMENDOZA (5), SARAVIAYMENDOZA (3) |
| low | `DESCONOCIDO_EntremesDeLosGorrones` | CERVANTES | 3 | 2/3 (67%) | 0.38 | CERVANTES (2), VARGASMACHUCA (1) |
| low | `ANONIMO_ColoquiodeFenisa` | SARAVIAYMENDOZA | 24 | 8/24 (33%) | 0.37 | SARAVIAYMENDOZA (8), CASTILLOSOLORZANO (6), CERVANTES (5), GODINEZMANRIQUE (1), CASTROYSALAZAR (1) |
| low | `Anonimo_Detenedmequeseva` | GONZALEZDEBARCIA | 7 | 1/7 (14%) | 0.34 | GONZALEZDEBARCIA (1), FAJARDOYACEVEDO (1), BATRES (1), REMON (1) |
| low | `Anonimo_CaminodeCaramanchelEl` | CASTILLOSOLORZANO | 10 | 3/10 (30%) | 0.31 | CASTILLOSOLORZANO (3), SANDOVAL (3), FAJARDOYACEVEDO (1) |
| low | `DESCONOCIDO_VisitaDelNacimiento` | LEIVARAMIREZ | 13 | 5/13 (38%) | 0.30 | LEIVARAMIREZ (5), LEONORCUEVA (1), QUEVEDO (1), GARCIAMARCOS (1), CARVAJAL (1) |
| low | `DESCONOCIDO_HabiaenSevillaunasistente` | ROJASZORRILLA | 1 | 1/1 (100%) | 0.26 | ROJASZORRILLA (1) |
| low | `DESCONOCIDO_BaileDelJuegoDelHombre` | GONGORA | 7 | 4/7 (57%) | 0.25 | GONGORA (4), VARGASMACHUCA (1), MELO (1), SANDOVAL (1) |
| low | `DESCONOCIDO_CartaEjecutoria` | LICENCIADOROJAS | 121 | 62/121 (51%) | 0.22 | LICENCIADOROJAS (62), LEONORCUEVA (30), LORENZANA (3), MEDINA (3), REMON (2) |
| low | `DESCONOCIDO_DraftOfADispatch` | SANTATERESA | 9 | 2/9 (22%) | 0.20 | SANTATERESA (2), CUEVAYSILVA (1), MIRACLESSOTOMAYOR (1), HURTADODEMENDOZA (1), LEONORCUEVA (1) |
| low | `DESCONOCIDO_FinezaDeLosAusentes` | CERVANTES | 36 | 8/36 (22%) | 0.19 | CERVANTES (8), GARCIADEPRADO (7), MENESES (7), BATRES (4), HURTADODEMENDOZA (2) |

## 4. Untrained-author filenames

Manuscripts whose filename names an author that is not one of the 100 trained classes (and is not an anonymous marker). The model's prediction here is necessarily its closest match among trained scribes, since the actual author has no class. Predictions in this section should be treated as least reliable - there is no correct trained class for the model to predict.

If many filename prefixes here should resolve to a trained class (case variants, name variants, etc.), add them to `inference_aliases.yaml` and re-run.

**1472 manuscripts** (high: 93, medium: 380, low: 999)

| Tier | Manuscript | Model says | Pages | Agreement | Margin | Top-5 |
|---|---|---|---:|---:|---:|---|
| high | `BarrionuevodePeraltaJeronimo_BarracodeRiosalidoEl` | BARRIONUEVO | 446 | 438/446 (98%) | 145.20 | BARRIONUEVO (438), AVELLANEDA (2) |
| high | `GomezAcostaFrancisco_Pongalenombreeldiscreto` | GOMEZACOSTA | 36 | 32/36 (89%) | 80.91 | GOMEZACOSTA (32), BANCESCANDAMO (1) |
| high | `CartaSANTATERESA_MariaJose` | SANTATERESA | 2 | 2/2 (100%) | 80.38 | SANTATERESA (2) |
| high | `RoseteNinoPedro_PiramoyTisbe` | ROSETENINO | 59 | 49/59 (83%) | 76.81 | ROSETENINO (49), GILENRIQUEZ (1) |
| high | `DavilayPalomaresMartin_Imposiblesvenceamor` | DAVILAYPALOMARES | 60 | 53/60 (88%) | 65.59 | DAVILAYPALOMARES (53), LEONORCUEVA (1) |
| high | `AndosillayEnriquezDiegoFrancis_NacimientodeCristoEl` | ANDOSILLA | 136 | 132/136 (97%) | 64.75 | ANDOSILLA (132), CAXESI (1) |
| high | `LaniniySagredoPedroFranciscode_GranreyanacoretaSanOnofreEl` | LANINI | 66 | 57/66 (86%) | 62.18 | LANINI (57), SANDOVAL (2), FAJARDOYACEVEDO (1) |
| high | `CARTASGracian_TorreyServil_Autografo` | GRACIAN | 8 | 8/8 (100%) | 57.68 | GRACIAN (8) |
| high | `LlobregatyEsteveFranciscode_Maspesanpajasqueculpas` | LLOBREGATYESTEVE | 62 | 52/62 (84%) | 52.99 | LLOBREGATYESTEVE (52), GONZALEZDEBARCIA (1), VARGASMACHUCA (1) |
| high | `GarciadePradoJoseAntonio_PachecosyPalomeques` | GARCIADEPRADO | 75 | 65/75 (87%) | 52.33 | GARCIADEPRADO (65), GONZALEZDEBARCIA (1), HURTADODEMENDOZA (1) |
| high | `BarredaJuandela_Desobligaramando` | BARREDA | 68 | 58/68 (85%) | 49.05 | BARREDA (58), PSEUDOHURTADODEMENDOZA (1), GONGORA (1) |
| high | `ParedesJuande_Muertovivoylealtadenlatraicion` | PAREDES | 57 | 47/57 (82%) | 47.18 | PAREDES (47), GONZALEZDEBARCIA (1) |
| high | `LaniniySagredoPedroFranciscode_SitioytomadeNamur` | LANINI | 59 | 51/59 (86%) | 45.99 | LANINI (51), VIDALYSALVADOR (2), LICENCIADOROJAS (1), AVELLANEDA (1), CASTILLOSOLORZANO (1) |
| high | `LaniniySagredoPedroFranciscode_MonstruodelaamistadAzucenadeVa` | LANINI | 62 | 55/62 (89%) | 45.12 | LANINI (55), CERVANTES (1) |
| high | `DelaHozyMotaJuanClaudio_EncantodelolvidoLasortijadelol` | HOZYMOTA | 64 | 53/64 (83%) | 41.96 | HOZYMOTA (53), GONZALEZDEBARCIA (1), LEIVARAMIREZ (1) |
| high | `JuanBautistadeVillegas_LucidoroaragonesIIIjornada` | TORRESLORENZODE | 18 | 15/18 (83%) | 41.47 | TORRESLORENZODE (15), AMESCUA (1) |
| high | `JIMENEZ_AuroraDelSolDivino_Autografo_2` | JIMENEZSEDENO | 59 | 49/59 (83%) | 38.67 | JIMENEZSEDENO (49), LEONORCUEVA (1), VIDALYSALVADOR (1) |
| high | `SebastianRodriguezdeVillavicio_SortijadeFlorenciaLa` | CASTROYSALAZAR | 68 | 57/68 (84%) | 36.54 | CASTROYSALAZAR (57), HURTADODEMENDOZA (1), BARREDA (1) |
| high | `TamayoBartolomede_SanBartolomeprincipedelaIndiad` | TAMAYO | 74 | 65/74 (88%) | 36.30 | TAMAYO (65), CLARAMONTE (1), GONZALEZDEBARCIA (1) |
| high | `GonzalezdeBarciaCarballidoyZun_SacodelagrancasadeMecaEl` | GONZALEZDEBARCIA | 48 | 42/48 (88%) | 35.89 | GONZALEZDEBARCIA (42), LORENZANA (1), HOZYMOTA (1) |
| high | `GonzalezdeBarciaCarballidoyZun_EsclavitudensupatriaoLosesclav` | GONZALEZDEBARCIA | 56 | 49/56 (88%) | 35.65 | GONZALEZDEBARCIA (49), BANCESCANDAMO (1), GARCIADEPRADO (1), CONTRERAS (1) |
| high | `ONA_ArbolesAnimados_Autografo` | ONAVIEDMAYTORRES | 7 | 7/7 (100%) | 33.47 | ONAVIEDMAYTORRES (7) |
| high | `RomeroRoqueFrancisco_CondesdeMontalboLos` | ROMEROROQUE | 55 | 45/55 (82%) | 33.27 | ROMEROROQUE (45), GONZALEZDEBARCIA (1), LEONORCUEVA (1) |
| high | `Verycreergrancomedia` | CASTROYSALAZAR | 73 | 60/73 (82%) | 33.24 | CASTROYSALAZAR (60), VIDALYSALVADOR (3), GONZALEZDEBARCIA (1) |
| high | `QuirosFranciscoBernardode_Cazadoresytoreadores` | FBQUIROS | 10 | 9/10 (90%) | 32.81 | FBQUIROS (9), VIDALYSALVADOR (1) |
| high | `FajardoyAcevedoAntonio_EstrelladeEuropayfenixdeAfrica` | FAJARDOYACEVEDO | 71 | 61/71 (86%) | 30.20 | FAJARDOYACEVEDO (61), LICENCIADOROJAS (1), GONGORA (1) |
| high | `MolinayMendozaJuanAntoniode_Despreciosconamorymasmudablehe` | MOLINAYMENDOZA | 88 | 71/88 (81%) | 30.10 | MOLINAYMENDOZA (71), GONZALEZDEBARCIA (5), CONTRERAS (1), BARREDA (1) |
| high | `Nohaycontraelhonorpoder2` | PSEUDOHURTADODEMENDOZA | 67 | 57/67 (85%) | 29.48 | PSEUDOHURTADODEMENDOZA (57), LOPEZJACINTO (1) |
| high | `ManueldeAneroPuente_LuisPerezelgallego` | MOLINAYMENDOZA | 66 | 56/66 (85%) | 29.10 | MOLINAYMENDOZA (56), HURTADODEMENDOZA (1) |
| high | `II_01338_PoeticaTheologia` | AVELLANEDA | 83 | 73/83 (88%) | 28.37 | AVELLANEDA (73), SANTATERESA (2), LICENCIADOROJAS (1), BARRIONUEVO (1), ROMEROROQUE (1) |
| high | `ObraspoticasdeLuisdeGngora` | CASTROYSALAZAR | 306 | 285/306 (93%) | 28.30 | CASTROYSALAZAR (285), MELO (4), ROMEROROQUE (3), AVELLANEDA (2), BOLEAYALVARADO (1) |
| high | `BARRIOS_VariasComedias` | AVELLANEDA | 398 | 371/398 (93%) | 27.48 | AVELLANEDA (371), LICENCIADOROJAS (1), GONGORA (1), VALDIVIELSO (1), CONTRERAS (1) |
| high | `GongoraLuisde_DoctorCarlinoEl` | SANDOVAL | 479 | 448/479 (94%) | 26.08 | SANDOVAL (448), MIRACLESSOTOMAYOR (5), LEONORCUEVA (3), MEDINA (1), SANTATERESA (1) |
| high | `Dichaydesdichadelnombre` | GARCIAMARCOS | 112 | 95/112 (85%) | 25.94 | GARCIAMARCOS (95), LICENCIADOROJAS (1), GODINEZMANRIQUE (1), MELO (1) |
| high | `TellezGabriel_Celosconcelossecuran` | BELMONTE | 68 | 55/68 (81%) | 24.71 | BELMONTE (55), GONZALEZDEBARCIA (1), JIMENEZSEDENO (1), LEIVARAMIREZ (1) |
| high | `RojasZorrillaFranciscodeAtribu_FortunasdedonJuandeCastroyLemo` | LEIVARAMIREZ | 54 | 45/54 (83%) | 24.62 | LEIVARAMIREZ (45), LICENCIADOROJAS (1), CERVANTES (1), ROSETENINO (1), QUEVEDO (1) |
| high | `PedroFranciscodeLaniniySagredo_SeraloqueDiosquisiere` | LANINI | 111 | 96/111 (86%) | 24.19 | LANINI (96), VIDALYSALVADOR (4), QUINONES (1), AVELLANEDADELACUEVA (1), REMON (1) |
| high | `MATOScorrecciones_VaqueroEmperador_acto1_Autografo` | MATOSFRAGOSO | 36 | 35/36 (97%) | 24.01 | MATOSFRAGOSO (35), VIDALYSALVADOR (1) |
| high | `DelaHozyMotaJuanClaudio_JosefsalvadordeEgiptoytriunfos` | HOZYMOTA | 113 | 100/113 (88%) | 23.71 | HOZYMOTA (100), REMON (3) |
| high | `BANCES_HOZYMOTA_SanBernardoAbad_Autografo` | HOZYMOTA | 120 | 107/120 (89%) | 23.47 | HOZYMOTA (107), VIDALYSALVADOR (3), CASTILLOSOLORZANO (1), ZABALETA (1), GONZALEZDEBARCIA (1) |
| high | `FranciscodeLeivaRamirezdeArell_Nohaycontraunpadrerazon` | LEIVARAMIREZ | 169 | 150/169 (89%) | 23.41 | LEIVARAMIREZ (150), VIDALYSALVADOR (2), HURTADODEMENDOZA (2), LANINI (1), LOPEZDECARDENA (1) |
| high | `ARCE_ZapaterovizcainoEl` | CECILIANACIMIENTO | 12 | 10/12 (83%) | 23.06 | CECILIANACIMIENTO (10), VARGASMACHUCA (2) |
| high | `LaniniySagredoPedroFranciscode_SaberobligaraDiosparallegarase` | LANINI | 68 | 56/68 (82%) | 22.79 | LANINI (56), LICENCIADOROJAS (2), LEONORCUEVA (1), MORETO (1) |
| high | `FranciscoAntoniodeBancesCandam_PorsureyyporsudamaMaseselruido` | AVELLANEDA | 87 | 76/87 (87%) | 22.52 | AVELLANEDA (76), VIDALYSALVADOR (1) |
| high | `PedroAlvarezdeAyllon_Eglogapastoril` | CECILIANACIMIENTO | 119 | 97/119 (82%) | 22.32 | CECILIANACIMIENTO (97), CERVANTES (14), GOMEZACOSTA (2), CASTILLOSOLORZANO (1) |
| high | `GallegosManuelde_InfiernodeamorEl` | GALLEGOS | 135 | 113/135 (84%) | 22.25 | GALLEGOS (113), ROMEROROQUE (2), GONZALEZDETORRES (1), VARGASMACHUCA (1), VIDALYSALVADOR (1) |
| high | `AYALA_HechosyTravesuras2` | CASTROYSALAZAR | 93 | 87/93 (94%) | 21.63 | CASTROYSALAZAR (87), GONZALEZDETORRES (2), SANDOVAL (2), LANINI (1), MELO (1) |
| high | `RojasVillandrandoAgustinde_NaturaldesdichadoEl` | ROJASVILLANDRANDO | 123 | 101/123 (82%) | 21.43 | ROJASVILLANDRANDO (101), VARGAS (1), CASTILLOSOLORZANO (1), SANTATERESA (1), LICENCIADOROJAS (1) |
| high | `JUANAINES_AutossobrelaquentaquedioelBachillerDonMatheoOrtizdeTorres_Firma` | VARGASMACHUCA | 1 | 1/1 (100%) | 20.83 | VARGASMACHUCA (1) |
| high | `JuanClaudiodelaHozyMotaFrancis_SanBernardoabad` | CASTROYSALAZAR | 61 | 53/61 (87%) | 20.82 | CASTROYSALAZAR (53), MELO (1) |
| high | `MesaGasparde_BrutoatenienseEl` | MESA | 137 | 111/137 (81%) | 20.48 | MESA (111), VIDALYSALVADOR (3), VARGAS (2), VARGASMACHUCA (1), MONTALBAN (1) |
| high | `CubillodeAragonAlvaro_ComendadoresdeCordobaoelhonord` | CLARAMONTE | 61 | 49/61 (80%) | 20.05 | CLARAMONTE (49), MATOSFRAGOSO (3), ENRIQUEZ (2), SALAZARYTORRES (2) |
| high | `ORMOTAJUAN_Elbuenjueznotienepatria_Novena` | CASTROYSALAZAR | 48 | 45/48 (94%) | 19.20 | CASTROYSALAZAR (45), BATRES (1), GILENRIQUEZ (1), BOLEAYALVARADO (1) |
| high | `GONZALEZ_ApostolDeLaGrecia` | GONZALEZDEBARCIA | 70 | 61/70 (87%) | 19.09 | GONZALEZDEBARCIA (61), VIDALYSALVADOR (3), CASTILLOSOLORZANO (1) |
| high | `CARTA_SaDeMiranda` | VARGASMACHUCA | 2 | 2/2 (100%) | 19.07 | VARGASMACHUCA (2) |
| high | `MERCADERDECERVELLON_NoPuedeHaberDosQueSeAmen` | VIDALYSALVADOR | 120 | 120/120 (100%) | 18.66 | VIDALYSALVADOR (120) |
| high | `NICODEMUS_Actusindiferentesinindividuo` | GILENRIQUEZ | 35 | 30/35 (86%) | 18.65 | GILENRIQUEZ (30), VERATASSIS (2), LEONORCUEVA (1) |
| high | `VAYALARDE_VAYALARDE1PARTE` | GILENRIQUEZ | 49 | 42/49 (86%) | 17.39 | GILENRIQUEZ (42), VERATASSIS (3), CASTROYSALAZAR (3), SANDOVAL (1) |
| high | `AVILA_VengaLoQueViniere` | CARVAJAL | 45 | 42/45 (93%) | 17.08 | CARVAJAL (42), SANTATERESA (1), QUINONES (1), CONTRERAS (1) |
| high | `GarciadePradoJoseAntonio_Convertirseelmalenbien` | GARCIADEPRADO | 165 | 140/165 (85%) | 17.03 | GARCIADEPRADO (140), GONZALEZDETORRES (3), BARREDA (1), AGUADOELVIEJO (1), SAAVEDRAFAJARDO (1) |
| high | `FajardoyAcevedoAntonio_Linajeshaceelamor` | FAJARDOYACEVEDO | 147 | 119/147 (81%) | 16.94 | FAJARDOYACEVEDO (119), CALLE (1), BARREDA (1), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| high | `PaulinoHomedes_SanPascualBailon` | VIDALYSALVADOR | 71 | 64/71 (90%) | 16.79 | VIDALYSALVADOR (64), VARGASMACHUCA (2), CASTILLOSOLORZANO (1) |
| high | `CastilloSolorzanoAlonsodel_Mayorazgofigurayelinterescasti` | CASTILLOSOLORZANO | 117 | 107/117 (92%) | 16.77 | CASTILLOSOLORZANO (107), VIDALYSALVADOR (1), HURTADODEMENDOZA (1) |
| high | `ZAMORA_SerFinoYNoParecerlo` | VIDALYSALVADOR | 171 | 171/171 (100%) | 16.61 | VIDALYSALVADOR (171) |
| high | `AGUAYO_VallesDeSopetran` | VIDALYSALVADOR | 152 | 127/152 (84%) | 16.45 | VIDALYSALVADOR (127) |
| high | `REYES_CulebradeORO_Autografo` | CONTRERAS | 276 | 235/276 (85%) | 16.30 | CONTRERAS (235), BANCESCANDAMO (19), CECILIANACIMIENTO (12), CASTILLOSOLORZANO (1), LEIVARAMIREZ (1) |
| high | `GONZALEZDEBUSTOS_RemedioEstaEnElDano` | LORENZANA | 50 | 48/50 (96%) | 15.98 | LORENZANA (48), MELO (1), HURTADODEMENDOZA (1) |
| high | `AntonioEnriquezGomez_Nohaycontraelhonorpoder` | SANDOVAL | 77 | 65/77 (84%) | 15.94 | SANDOVAL (65), LICENCIADOROJAS (1), SANTATERESA (1), GARCIAMARCOS (1), CASTROYSALAZAR (1) |
| high | `ZabaletaJuande_HonraviveenlosmuertosLa` | ZABALETA | 133 | 116/133 (87%) | 15.59 | ZABALETA (116), LEIVARAMIREZ (4), CERVANTES (1), ROJASZORRILLA (1), GRACIAN (1) |
| high | `VEGA_MejorAlcaldeElRey` | AVELLANEDA | 32 | 28/32 (88%) | 15.36 | AVELLANEDA (28), BELMONTE (1) |
| high | `SaraviayMendozaGasparde_Loqueescomedia` | SARAVIAYMENDOZA | 187 | 154/187 (82%) | 14.76 | SARAVIAYMENDOZA (154), MELO (3), GONZALEZDETORRES (2), CANIZARES (1), LICENCIADOROJAS (1) |
| high | `BenavidesJuande_MarteespanolGuzmandonAlvarodeG` | BENAVIDES | 131 | 108/131 (82%) | 14.67 | BENAVIDES (108), GONZALEZDETORRES (2), GONZALEZDEBARCIA (1) |
| high | `MelchorFernandezdeLeon_ObrasdedonMelchorFernandezdeLe` | VIDALYSALVADOR | 177 | 172/177 (97%) | 14.61 | VIDALYSALVADOR (172), AVELLANEDA (2) |
| high | `DiegodeNajerayZegri_AguademejorvidaEl` | CASTROYSALAZAR | 20 | 17/20 (85%) | 13.70 | CASTROYSALAZAR (17) |
| high | `GaspardeAvila_VenerableBernardinodeObregonEl` | LICENCIADOROJAS | 87 | 73/87 (84%) | 13.19 | LICENCIADOROJAS (73), CECILIANACIMIENTO (2), ENRIQUEZ (2), PAREDES (1), AMESCUA (1) |
| high | `AgustinManueldeCastilla_MariadelSocorroBeataMercenaria` | VIDALYSALVADOR | 74 | 61/74 (82%) | 12.48 | VIDALYSALVADOR (61), VERATASSIS (6), LEONORCUEVA (1), CERVANTES (1), GONZALEZDEBARCIA (1) |
| high | `AntonioEnriquezGomez_ValienteDiegodeCamasEl` | PAREDES | 37 | 31/37 (84%) | 12.46 | PAREDES (31), GOMEZACOSTA (1), REMON (1) |
| high | `COUTOPESTANA_LOACamposElysiosDeAmor` | PAREDES | 9 | 8/9 (89%) | 11.91 | PAREDES (8) |
| high | `RAMOSDELCASTILLO_Atribuido_AutoSacramental` | FAJARDOYACEVEDO | 14 | 12/14 (86%) | 11.44 | FAJARDOYACEVEDO (12), MOLINAYMENDOZA (1) |
| high | `VELEZDEGUEVARA_CeloshacenestrellasLos` | MELO | 112 | 110/112 (98%) | 11.40 | MELO (110), LEONORCUEVA (2) |
| high | `CorderoJacinto_MayortrancedehonorEl` | CORDERO | 115 | 99/115 (86%) | 11.38 | CORDERO (99), VIDALYSALVADOR (2), BANCESCANDAMO (2), LICENCIADOROJAS (1), ENRIQUEZ (1) |
| high | `RemonAlonsode_TresmujeresenunaLas` | PAREDES | 73 | 66/73 (90%) | 11.28 | PAREDES (66), AMESCUA (1), CARVAJAL (1) |
| high | `SIMONAGUADO_Atribuido_LaPlazaDelRetiro` | ANDOSILLA | 5 | 4/5 (80%) | 11.18 | ANDOSILLA (4), CASTILLOSOLORZANO (1) |
| high | `ClaramonteAndresde_SecretoenlamujerEl` | CLARAMONTE | 107 | 86/107 (80%) | 11.05 | CLARAMONTE (86), MIRACLESSOTOMAYOR (3), MEDINA (1), CERVANTES (1), LORENZANA (1) |
| high | `VelezGuevara_autoracomedias` | MELO | 184 | 148/184 (80%) | 10.95 | MELO (148), CARVAJAL (2), LEONORCUEVA (2), LICENCIADOROJAS (1), TORRESLORENZODE (1) |
| high | `VelezGuevara_findefiesta` | MELO | 184 | 148/184 (80%) | 10.95 | MELO (148), CARVAJAL (2), LEONORCUEVA (2), LICENCIADOROJAS (1), TORRESLORENZODE (1) |
| high | `VelezGuevara_loaanosreina` | MELO | 184 | 148/184 (80%) | 10.95 | MELO (148), CARVAJAL (2), LEONORCUEVA (2), LICENCIADOROJAS (1), TORRESLORENZODE (1) |
| high | `GonzalezdeBarciaCarballidoyZun_GranprofetaEliseoEl` | GONZALEZDEBARCIA | 59 | 48/59 (81%) | 10.82 | GONZALEZDEBARCIA (48), VIDALYSALVADOR (1), ROMEROROQUE (1), LICENCIADOROJAS (1), REMON (1) |
| high | `JosedeArroyoAtribuidoCristobal_HonorenelsuplicioyprodigiodeCa` | GALLEGOS | 86 | 70/86 (81%) | 10.60 | GALLEGOS (70), GONZALEZDEBARCIA (1), BATRES (1), LOPEZJACINTO (1) |
| high | `MALVEZZI_HistoriaDeEspana1` | CERVANTES | 130 | 112/130 (86%) | 10.47 | CERVANTES (112), BANCESCANDAMO (15), VARGASMACHUCA (1), GRACIAN (1) |
| high | `FOLCH_ObrarContraSuIntencion` | AVELLANEDA | 43 | 43/43 (100%) | 10.37 | AVELLANEDA (43) |
| high | `BOLEA_TetisPeleo_VicenteCamacho` | GILENRIQUEZ | 100 | 87/100 (87%) | 10.24 | GILENRIQUEZ (87), VIDALYSALVADOR (3), ROSETENINO (2), QUINONES (1), GARCIAMARCOS (1) |
| high | `CastroyBellvisGuillendeAtribui_Quienmalasmanashatardeonuncala` | BELMONTE | 55 | 45/55 (82%) | 10.08 | BELMONTE (45), SANDOVAL (3), LICENCIADOROJAS (2), CASTILLOSOLORZANO (1) |
| medium | `CuevaySilvaFranciscodela_Narciso` | CUEVAYSILVA | 26 | 16/26 (62%) | 75.21 | CUEVAYSILVA (16), BANCESCANDAMO (1), LICENCIADOROJAS (1) |
| medium | `LaniniySagredoPedroFranciscode_HijodelcarpinterooelninodeZara` | LANINI | 61 | 47/61 (77%) | 61.82 | LANINI (47), GONZALEZDEBARCIA (1), CERVANTES (1), MELO (1) |
| medium | `LopezdeCastroDiego_MarcoAntonioyCleopatraTragedia` | LOPEZDECASTRO | 33 | 20/33 (61%) | 57.83 | LOPEZDECASTRO (20), LICENCIADOROJAS (1), LORENZANA (1), GONZALEZDETORRES (1) |
| medium | `ClaramonteAndresde_HornodeConstantinoplaEl` | CLARAMONTE | 29 | 17/29 (59%) | 57.33 | CLARAMONTE (17), VIDALYSALVADOR (1), HURTADODEMENDOZA (1), MULSA (1) |
| medium | `MedinaFranciscode_Milagrosossucesosdelalmiranted` | MEDINA | 26 | 17/26 (65%) | 56.92 | MEDINA (17), GONZALEZDETORRES (1), LOPEZDECASTRO (1) |
| medium | `LoaparalafiestadeNuestraSenoradePenaSacra_Autografo` | LANINI | 18 | 9/18 (50%) | 53.88 | LANINI (9) |
| medium | `LuisdeBelmonteBermudezAtribuid_CercoylibertaddeSevillaporelre` | MEDINA | 47 | 28/47 (60%) | 53.11 | MEDINA (28), SANDOVAL (2), GONZALEZDETORRES (1), GONZALEZDEBARCIA (1), LOPEZJACINTO (1) |
| medium | `GodinezManriqueFelipeAtribuido_IgnorantediscretoAutoalodivino` | LICENCIADOROJAS | 33 | 23/33 (70%) | 53.04 | LICENCIADOROJAS (23), TORRESLORENZODE (1) |
| medium | `RojasFranciscode_EsclavoalodivinoyMartirdeZarag` | LICENCIADOROJAS | 36 | 26/36 (72%) | 49.75 | LICENCIADOROJAS (26), VIDALYSALVADOR (1) |
| medium | `CaxesiJuan_HospitaldeSanRoqueEl` | CAXESI | 23 | 17/23 (74%) | 48.71 | CAXESI (17) |
| medium | `RuizAlceoJuan_NavegaciondeUlisesLa` | RUIZALCEO | 34 | 24/34 (71%) | 48.43 | RUIZALCEO (24), CERVANTES (1), SANDOVAL (1) |
| medium | `LaniniySagredoPedroFranciscode_Habladmeenentrando` | LANINI | 64 | 51/64 (80%) | 42.79 | LANINI (51), VIDALYSALVADOR (2), GONZALEZDEBARCIA (1), PAREDES (1) |
| medium | `CuencayArguelloAmbrosio_TejedoresLos` | CUENCAYARGUELLO | 18 | 9/18 (50%) | 41.64 | CUENCAYARGUELLO (9), CASTILLOSOLORZANO (1) |
| medium | `CanizaresySuarezdeToledoJosede_Introduccionenformadebailepara` | CANIZARES | 8 | 4/8 (50%) | 40.34 | CANIZARES (4), BANCESCANDAMO (1) |
| medium | `AntoniodeZamora_SortijaLa` | CASTROYSALAZAR | 12 | 8/12 (67%) | 40.28 | CASTROYSALAZAR (8), GONZALEZDEBARCIA (1) |
| medium | `CanizaresySuarezdeToledoJosede_CaballoEl` | CANIZARES | 8 | 5/8 (62%) | 40.25 | CANIZARES (5), BANCESCANDAMO (1) |
| medium | `CalderonAtribuido_DamaoelgalanfantasmaLa` | MOLINAYMENDOZA | 13 | 9/13 (69%) | 39.54 | MOLINAYMENDOZA (9), LEONORCUEVA (1), ROMEROROQUE (1) |
| medium | `TellezGabrielAtribuido_HabladmeenentrandoCelosdeamory` | CANIZARES | 27 | 19/27 (70%) | 37.99 | CANIZARES (19), SARAVIAYMENDOZA (1), LORENZANA (1), CASTILLOSOLORZANO (1) |
| medium | `ElrayodeAndalucia` | GILENRIQUEZ | 25 | 16/25 (64%) | 37.64 | GILENRIQUEZ (16), GONZALEZDEBARCIA (1), AVELLANEDA (1), BELMONTE (1) |
| medium | `QuinonesdeBenaventeLuis_Bailedelmundo` | QUINONES | 18 | 12/18 (67%) | 36.15 | QUINONES (12) |
| medium | `LaniniySagredoPedroFranciscode_Nacimientodelalbaparaquenacies` | LANINI | 58 | 45/58 (78%) | 35.74 | LANINI (45), GONZALEZDEBARCIA (2), ROMEROROQUE (1), MOLINAYMENDOZA (1) |
| medium | `JeronimoGuedejayQuiroga_Enelsuenoestalamuerte` | CANIZARES | 26 | 19/26 (73%) | 35.39 | CANIZARES (19), CASTROYSALAZAR (1) |
| medium | `JuanPerezdeMontalban_DeshonrahonrosaLa` | MORETO | 52 | 39/52 (75%) | 35.34 | MORETO (39), LICENCIADOROJAS (2), MULSA (2) |
| medium | `BancesCandamoFranciscoAntoniod_Theatrodelospasadosypresentess` | BANCESCANDAMO | 95 | 72/95 (76%) | 35.27 | BANCESCANDAMO (72), GONZALEZDEBARCIA (16), VIDALYSALVADOR (2), CASTILLOSOLORZANO (2), BOLEAYALVARADO (1) |
| medium | `JosedeValdivielso_DescensiondeNuestraSenoraenlas` | LICENCIADOROJAS | 79 | 47/79 (60%) | 34.64 | LICENCIADOROJAS (47), LORENZANA (1), GONZALEZDEBARCIA (1) |
| medium | `MoretoyCavanaAgustin_Poderdelaamistadyvenganzasinca` | MORETO | 91 | 69/91 (76%) | 34.06 | MORETO (69), GARCIADEPRADO (3), FBQUIROS (2), VALDIVIELSO (1) |
| medium | `MiradeAmescuaAntonio_PrimercondedeFlandesEl` | CASTROYSALAZAR | 41 | 23/41 (56%) | 32.84 | CASTROYSALAZAR (23), MELO (6), LANINI (2), GONZALEZDEBARCIA (1) |
| medium | `LaniniySagredoPedroFranciscode_Dialogoqueserepresentoenlacolo` | LANINI | 32 | 21/32 (66%) | 32.72 | LANINI (21), PSEUDOHURTADODEMENDOZA (1), GONZALEZDEBARCIA (1), MOLINAYMENDOZA (1), HOZYMOTA (1) |
| medium | `VegaCarpioLopedeAtribuidoCalde_NecedadeneldiscretoLa` | PSEUDOHURTADODEMENDOZA | 57 | 36/57 (63%) | 32.11 | PSEUDOHURTADODEMENDOZA (36), TORRESLORENZODE (5), PAREDES (4), CAXESI (1) |
| medium | `SotoJuande_VirgendelRosarioLa` | JUANDESOTO | 61 | 41/61 (67%) | 31.46 | JUANDESOTO (41), CARVAJAL (1), GONZALEZDETORRES (1) |
| medium | `RojasFranciscode_MartiriodeSantaLuciavirgenymar` | LICENCIADOROJAS | 27 | 21/27 (78%) | 30.89 | LICENCIADOROJAS (21) |
| medium | `FajardoyAcevedoAntonio_SalomondeMallorcaEl` | FAJARDOYACEVEDO | 66 | 52/66 (79%) | 30.35 | FAJARDOYACEVEDO (52), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| medium | `BernardinodeObregonAtribuidoMo_DivinoportuguessanAntoniodePad` | FAJARDOYACEVEDO | 72 | 55/72 (76%) | 29.64 | FAJARDOYACEVEDO (55), GONGORA (1), ANDOSILLA (1), HURTADODEMENDOZA (1), BANCESCANDAMO (1) |
| medium | `GonzalezdeTorresManuel_MejormaestroamorEl` | GONZALEZDETORRES | 56 | 44/56 (79%) | 29.27 | GONZALEZDETORRES (44), GONZALEZDEBARCIA (2), CALLE (1), VIDALYSALVADOR (1) |
| medium | `CanizaresySuarezdeToledoJosede_LoaquehizolacompaniadeJosePrad` | CANIZARES | 10 | 5/10 (50%) | 28.80 | CANIZARES (5), GONZALEZDEBARCIA (1), VIDALYSALVADOR (1) |
| medium | `AndresDomingo_NacimientoEl` | MESA | 55 | 31/55 (56%) | 28.31 | MESA (31), GONZALEZDETORRES (1), VIDALYSALVADOR (1), CASTILLOSOLORZANO (1), QUINONES (1) |
| medium | `LapuentedeMantible` | SANDOVAL | 40 | 27/40 (68%) | 28.27 | SANDOVAL (27), LANINI (3), PAREDES (2), TAMAYO (1) |
| medium | `CanizaresySuarezdeToledoJosede_SoponesLos` | CANIZARES | 10 | 5/10 (50%) | 27.76 | CANIZARES (5), CERVANTES (2), AMESCUA (1) |
| medium | `MatosFragosoJuande_FregonaLa` | LEIVARAMIREZ | 8 | 5/8 (62%) | 27.06 | LEIVARAMIREZ (5), CERVANTES (1), GARCIADEPRADO (1) |
| medium | `BelmonteBermudezLuisde_BodasdeFineoLas` | BELMONTE | 55 | 35/55 (64%) | 26.82 | BELMONTE (35), VIDALYSALVADOR (2) |
| medium | `VelezdeGuevaraLuis_SerranadelaVeraLa` | VELEZ | 143 | 109/143 (76%) | 26.82 | VELEZ (109), DIAMANTE (5), CERVANTES (1), CASTILLOSOLORZANO (1), CONTRERAS (1) |
| medium | `GilEnriquezAndres_Nohayprevencioncontraelhado` | GILENRIQUEZ | 18 | 13/18 (72%) | 26.15 | GILENRIQUEZ (13), VIDALYSALVADOR (1), TIRSO (1) |
| medium | `FajardoyAcevedoAntonio_ConquistadeGranadaLa` | FAJARDOYACEVEDO | 75 | 57/75 (76%) | 25.90 | FAJARDOYACEVEDO (57), JIMENEZSEDENO (2), MEDINA (1), GONZALEZDETORRES (1), SARAVIAYMENDOZA (1) |
| medium | `CanizaresySuarezdeToledoJosede_Mirenquemehacenpedazos` | CANIZARES | 8 | 4/8 (50%) | 25.72 | CANIZARES (4), GONZALEZDEBARCIA (1), LEONORCUEVA (1) |
| medium | `AvellanedaLorenzode_VidaconversionymuertedeAguedad` | AVELLANEDA | 257 | 175/257 (68%) | 25.39 | AVELLANEDA (175), VIDALYSALVADOR (3), GONZALEZDEBARCIA (1), PSEUDOHURTADODEMENDOZA (1), BENAVIDES (1) |
| medium | `FranciscoManueldeMelo_Comedia` | MELO | 270 | 163/270 (60%) | 25.04 | MELO (163), ROMEROROQUE (96), CARVAJAL (2), GRACIAN (2), VARGASMACHUCA (2) |
| medium | `QUINONESDEBENAVENTE_NocheDeSanJuan` | LOPEZJACINTO | 12 | 8/12 (67%) | 24.43 | LOPEZJACINTO (8) |
| medium | `LuisdeBelmonteBermudez_SatisfechoEl` | PSEUDOHURTADODEMENDOZA | 62 | 49/62 (79%) | 23.36 | PSEUDOHURTADODEMENDOZA (49), LEIVARAMIREZ (3), CERVANTES (1), HOZYMOTA (1), CASTILLOSOLORZANO (1) |
| medium | `VELEZDEGUEVARA_MaspesaelRey` | GONZALEZDETORRES | 37 | 23/37 (62%) | 22.54 | GONZALEZDETORRES (23), MULSA (12), MENESES (1) |
| medium | `VelezdeGuevaraLuis_ReyensuimaginacionEl` | VELEZ | 127 | 93/127 (73%) | 22.02 | VELEZ (93), AMESCUA (3), SANTATERESA (1), HURTADODEMENDOZA (1), SAAVEDRAFAJARDO (1) |
| medium | `CartaSANTATERESA_AlvaroMendoza` | SANTATERESA | 2 | 1/2 (50%) | 21.87 | SANTATERESA (1) |
| medium | `HozyMotaJuanClaudiodela_TorosdeAlcalaLos` | HOZYMOTA | 10 | 6/10 (60%) | 21.71 | HOZYMOTA (6), GONZALEZDEBARCIA (1), BANCESCANDAMO (1) |
| medium | `CordobayMaldonadoAlonso_VenganzaenelsepulcroLa` | MORETO | 51 | 34/51 (67%) | 20.76 | MORETO (34), DIAMANTE (3), VILLEGASJUANBAUTISTA (1), CERVANTES (1), VIDALYSALVADOR (1) |
| medium | `LosmartiresdeMadridydejarunreinoporotro4` | MOLINAYMENDOZA | 52 | 38/52 (73%) | 20.11 | MOLINAYMENDOZA (38), FAJARDOYACEVEDO (4), LOPEZJACINTO (1), LEIVARAMIREZ (1), CANIZARES (1) |
| medium | `VillegasdelaCruzyBerrioDiegoAt_NacimientodeSanJuanBautistaEl` | VILLEGASDELACRUZ | 57 | 33/57 (58%) | 19.76 | VILLEGASDELACRUZ (33), LICENCIADOROJAS (1), BOLEAYALVARADO (1), GONZALEZDEBARCIA (1), VIDALYSALVADOR (1) |
| medium | `COLABORADA_ElPolifemoyCirce` | CASTROYSALAZAR | 46 | 36/46 (78%) | 19.54 | CASTROYSALAZAR (36), CERVANTES (2), LORENZANA (2), BELMONTE (1) |
| medium | `OLMEDO_Arias_Autografo` | HOZYMOTA | 6 | 3/6 (50%) | 19.31 | HOZYMOTA (3), LANINI (1), CASTILLOSOLORZANO (1) |
| medium | `TellezGabriel_SantaJuanaParteIIIIyIIIpartede` | TIRSO | 331 | 180/331 (54%) | 18.81 | TIRSO (180), BATRES (49), LEIVARAMIREZ (16), QUINONES (9), ENRIQUEZ (7) |
| medium | `MiraclesSotomayorFrancisco_Quienbienamatardeolvida` | MIRACLESSOTOMAYOR | 150 | 116/150 (77%) | 18.70 | MIRACLESSOTOMAYOR (116), JUANDESOTO (1), LORENZANA (1), JIMENEZSEDENO (1), MULSA (1) |
| medium | `COUTOPESTANA_OndeHayRazonHayDesculpa` | AVELLANEDA | 47 | 32/47 (68%) | 18.11 | AVELLANEDA (32), MEDINA (10), PAREDES (3), TORRESLORENZODE (2) |
| medium | `AntoniodeZamora_NomuerequienviveenDiosSanMercu` | CASTROYSALAZAR | 76 | 57/76 (75%) | 17.99 | CASTROYSALAZAR (57), GARCIAMARCOS (2), VIDALYSALVADOR (2), PAREDES (1), HURTADODEMENDOZA (1) |
| medium | `ComediasLopeVegaEtAL-II-461` | PACHECO | 521 | 364/521 (70%) | 17.60 | PACHECO (364), MEDINA (59), TORRESLORENZODE (45), RUIZALCEO (21), LANINI (15) |
| medium | `CartaSANTATERESA_JeronimoGracian` | SANTATERESA | 4 | 2/4 (50%) | 17.58 | SANTATERESA (2), HURTADODEMENDOZA (1) |
| medium | `CALLEJA_SanFrancescoJavier` | VIDALYSALVADOR | 9 | 7/9 (78%) | 17.55 | VIDALYSALVADOR (7), PAREDES (2) |
| medium | `SANCHEZ_Desgraciaventurosa` | PACHECO | 49 | 36/49 (74%) | 17.54 | PACHECO (36), LANINI (9), TORRESLORENZODE (4) |
| medium | `Cepeda_BurlasdeBeniticoLas` | LICENCIADOROJAS | 31 | 21/31 (68%) | 16.19 | LICENCIADOROJAS (21), SANTATERESA (2), GONZALEZDEBARCIA (1) |
| medium | `JuandeVelascoyGuzman_PerdidadeEspanaLamasinjustaven` | MOLINAYMENDOZA | 84 | 59/84 (70%) | 15.95 | MOLINAYMENDOZA (59), GARCIAMARCOS (12), GONZALEZDEBARCIA (2), CARVAJAL (1), CASTILLOSOLORZANO (1) |
| medium | `EsperezdeBorsaFranciscoAtribui_Obrassoncalidadhazanasdelgrand` | MORETO | 30 | 17/30 (57%) | 15.86 | MORETO (17), CANIZARES (2), VERATASSIS (1), CALDERON (1) |
| medium | `VegaCarpioLopede_VentadelazarzuelaLa` | BELMONTE | 29 | 21/29 (72%) | 15.62 | BELMONTE (21), CARVAJAL (1), TORRESLORENZODE (1) |
| medium | `JuandeBenavidesAtribuido_VidaymuertedeSanCristobal` | ROMEROROQUE | 28 | 15/28 (54%) | 15.54 | ROMEROROQUE (15), GALLEGOS (2), CLARAMONTE (1) |
| medium | `MontalbanJuanPerezde_Loquesonjuiciosdelcielo` | MORETO | 46 | 23/46 (50%) | 15.49 | MORETO (23), CLARAMONTE (15), LOPEZDECASTRO (1), SANDOVAL (1), CASTILLOSOLORZANO (1) |
| medium | `ROJASVICENCIO_BodasenelSuplicio_Autografo` | AVELLANEDA | 90 | 71/90 (79%) | 15.42 | AVELLANEDA (71), MELO (12), LANINI (4), SANDOVAL (2), GONZALEZDEBARCIA (1) |
| medium | `RojasZorrillaFranciscode_PersilesySegismundoHallarsepar` | SANDOVAL | 79 | 56/79 (71%) | 15.26 | SANDOVAL (56), PAREDES (3), LEONORCUEVA (3), LOPEZJACINTO (3), GONZALEZDEBARCIA (1) |
| medium | `MoretoyCavanaAgustinAtribuido_FortunamerecidaLa` | CANIZARES | 32 | 23/32 (72%) | 15.24 | CANIZARES (23), REMON (2), MOLINAYMENDOZA (2), MORETO (2), LICENCIADOROJAS (1) |
| medium | `MatosFragosoJuande_JobdelasmujeresSantaIsabelrein` | PAREDES | 88 | 64/88 (73%) | 15.17 | PAREDES (64), VIDALYSALVADOR (4), GONGORA (2), VARGASMACHUCA (2), CORDERO (1) |
| medium | `RuanoMargaritaAtribuido_PosadasdeMadridLas` | RUANO | 12 | 6/12 (50%) | 15.12 | RUANO (6), LEONORCUEVA (1), GONZALEZDEBARCIA (1), VARGASMACHUCA (1), GARCIAMARCOS (1) |
| medium | `Laverdadyeltiempoentiempo` | GONZALEZDEBARCIA | 15 | 9/15 (60%) | 14.98 | GONZALEZDEBARCIA (9) |
| medium | `MoretoyCavanaAgustin_CenadeBaltasarLa` | TORRESLORENZODE | 54 | 33/54 (61%) | 14.96 | TORRESLORENZODE (33), ANDOSILLA (6), SANDOVAL (4), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| medium | `CalleFranciscodela_TreshermanosdelcieloMartiresde` | CALLE | 151 | 114/151 (76%) | 14.91 | CALLE (114), MIRACLESSOTOMAYOR (1), CERVANTES (1), GARCIAMARCOS (1), VILLEGASJUANBAUTISTA (1) |
| medium | `VAYALARDE_Pedro_MagicoSalermo_Novena` | GILENRIQUEZ | 48 | 34/48 (71%) | 14.90 | GILENRIQUEZ (34), SANDOVAL (8), VERATASSIS (4), LANINI (2) |
| medium | `VegaCarpioLopede_Ovejaperdida` | CASTROYSALAZAR | 36 | 24/36 (67%) | 14.59 | CASTROYSALAZAR (24), BANCESCANDAMO (1), MELO (1), LANINI (1), PAREDES (1) |
| medium | `BatresAlonsode_Venganzashaysihayinjurias` | BATRES | 131 | 100/131 (76%) | 14.44 | BATRES (100), VIDALYSALVADOR (5), SANDOVAL (3), BENAVIDES (1), LEIVARAMIREZ (1) |
| medium | `FranciscoAntoniodeBancesCandam_Cualeslafieramayorentrelosmons` | VIDALYSALVADOR | 64 | 51/64 (80%) | 14.32 | VIDALYSALVADOR (51), CASTILLOSOLORZANO (2), CECILIANACIMIENTO (1), GONZALEZDEBARCIA (1), HOZYMOTA (1) |
| medium | `MLHouse_CaballeroSacramentoCOLOR` | LOPE | 73 | 46/73 (63%) | 14.12 | LOPE (46), ROMEROROQUE (3), HURTADODEMENDOZA (2), CERVANTES (2), CAXESI (2) |
| medium | `FrancisodeAvellanedadelaCuevay_VolverseelrayoenlaurelSeguiraD` | MELO | 65 | 51/65 (78%) | 14.10 | MELO (51), GONZALEZDEBARCIA (2), MEDINA (1), SANDOVAL (1), LOPEZJACINTO (1) |
| medium | `BancesCandamoAtribuido_ObrarbienqueDiosesDios` | MESA | 53 | 35/53 (66%) | 14.10 | MESA (35), LICENCIADOROJAS (3), SANTATERESA (2), GONZALEZDEBARCIA (1), SALAZARYTORRES (1) |
| medium | `FranciscodelosSantos_LavenidadelaflotaAutoyloa` | AVELLANEDA | 102 | 54/102 (53%) | 13.99 | AVELLANEDA (54), VIDALYSALVADOR (17), PAREDES (16) |
| medium | `GodinezManriqueFelipe_TraicioncontrasuduenoLa` | GODINEZMANRIQUE | 109 | 62/109 (57%) | 13.93 | GODINEZMANRIQUE (62), CONTRERAS (8), LOPEZJACINTO (4), BATRES (4), QUINONES (4) |
| medium | `VelezdeGuevaraLuis_PrivadoperseguidoEllucerodeCas` | CALDERON | 71 | 42/71 (59%) | 13.53 | CALDERON (42), BELMONTE (12), MONTALBAN (4), CERVANTES (1), TIRSO (1) |
| medium | `Correspondencia2SANTATERESA` | CECILIANACIMIENTO | 329 | 170/329 (52%) | 13.48 | CECILIANACIMIENTO (170), PAREDES (76), AVELLANEDA (22), GOMEZACOSTA (9), LANINI (6) |
| medium | `Ellirioylaazucena` | VIDALYSALVADOR | 42 | 30/42 (71%) | 13.25 | VIDALYSALVADOR (30), CASTROYSALAZAR (2), GARCIAMARCOS (1) |
| medium | `MelchorFernandezdeLeon_PrimertemplodeamorEl` | SANDOVAL | 61 | 40/61 (66%) | 13.25 | SANDOVAL (40), GILENRIQUEZ (4), LOPEZJACINTO (1), CERVANTES (1), QUINONES (1) |
| medium | `CanizaresySuarezdeToledoJosede_FalsonunciodePortugalEl` | CASTROYSALAZAR | 56 | 42/56 (75%) | 13.17 | CASTROYSALAZAR (42), TORRESLORENZODE (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), MOLINAYMENDOZA (1) |
| medium | `Lasmesasdelafortuna` | CASTROYSALAZAR | 35 | 25/35 (71%) | 13.16 | CASTROYSALAZAR (25), GILENRIQUEZ (2), SANDOVAL (1) |
| medium | `Elprivadoperseguido` | SANDOVAL | 58 | 30/58 (52%) | 12.55 | SANDOVAL (30), CASTROYSALAZAR (18), GONZALEZDEBARCIA (1), BELMONTE (1) |
| medium | `ZAMORA_Presomuertoyvencedor` | CASTROYSALAZAR | 68 | 50/68 (74%) | 12.33 | CASTROYSALAZAR (50), GILENRIQUEZ (11), ROSETENINO (2), MELO (2), VIDALYSALVADOR (1) |
| medium | `AntonioFolchdeCardonaAlagon_EntradadelaReinaEntremesqueseh` | MOLINAYMENDOZA | 20 | 11/20 (55%) | 12.06 | MOLINAYMENDOZA (11), PAREDES (1), VIDALYSALVADOR (1) |
| medium | `CorderoJacinto_FavorenlasentenciaEl` | CORDERO | 119 | 90/119 (76%) | 11.90 | CORDERO (90), MONTALBAN (2), ONAVIEDMAYTORRES (2), SANTATERESA (1), CONTRERAS (1) |
| medium | `CUBILLO_AgravioSatisfecho` | REMON | 49 | 38/49 (78%) | 11.85 | REMON (38), ROJASZORRILLA (5), MESA (4), CARVAJAL (2) |
| medium | `FranciscoAntoniodeCastroySalaz_GaranonEl` | SANDOVAL | 14 | 8/14 (57%) | 11.85 | SANDOVAL (8), ROMEROROQUE (1), LEONORCUEVA (1), BANCESCANDAMO (1) |
| medium | `CARTAS_SAAVEDRA_Autografo` | SAAVEDRAFAJARDO | 3 | 2/3 (67%) | 11.74 | SAAVEDRAFAJARDO (2), MULSA (1) |
| medium | `GasparAguilar_VenganzahonrosaLa` | GOMEZACOSTA | 48 | 26/48 (54%) | 11.67 | GOMEZACOSTA (26), BENAVIDES (3), SANTATERESA (2), GARCIAMARCOS (2), MELO (1) |
| medium | `MiradeAmescuaAntonio_PedroTelonario` | MEDINA | 31 | 20/31 (64%) | 11.63 | MEDINA (20), TORRESLORENZODE (2), CERVANTES (1) |
| medium | `AntoniodeZamora_Presomuertoyvencedortodoscumpl` | BELMONTE | 72 | 54/72 (75%) | 11.41 | BELMONTE (54), MOLINAYMENDOZA (5), LICENCIADOROJAS (1), VIDALYSALVADOR (1), GONZALEZDEBARCIA (1) |
| medium | `FrancisodeAvellanedadelaCuevay_Capuchinoescocesysegundosansan` | CANIZARES | 55 | 36/55 (66%) | 11.39 | CANIZARES (36), MORETO (11), HOZYMOTA (1), LEONORCUEVA (1), DAVILAYPALOMARES (1) |
| medium | `AntonioHurtadodeMendoza_SenordebuenasnochesEl` | BELMONTE | 65 | 42/65 (65%) | 11.32 | BELMONTE (42), SANDOVAL (10), CONTRERAS (1), QUINONES (1), BARREDA (1) |
| medium | `VegaCarpioLopedeAtribuido_NuestraSenoradelaCandelariaysu` | ALARCON | 64 | 36/64 (56%) | 11.12 | ALARCON (36), CAXESI (5), GILENRIQUEZ (4), GARCIAMARCOS (2), RUIZALCEO (2) |
| medium | `Elvalornotieneedad2` | LEIVARAMIREZ | 61 | 37/61 (61%) | 10.96 | LEIVARAMIREZ (37), ROSETENINO (12), BELMONTE (1), LANINI (1) |
| medium | `VelezdeGuevaraLuisFranciscodeR_TambientieneelsolmenguanteNoha` | LEIVARAMIREZ | 72 | 57/72 (79%) | 10.88 | LEIVARAMIREZ (57), MONTALBAN (1), MOLINAYMENDOZA (1), LOPEZDELCAMPO (1), FAJARDOYACEVEDO (1) |
| medium | `Lasferiasdelalmaauto` | BARRIONUEVO | 22 | 13/22 (59%) | 10.83 | BARRIONUEVO (13) |
| medium | `DiegodeNajerayZegriAtribuido_TorneodelasartesliberalesEl` | LEONORCUEVA | 22 | 12/22 (55%) | 10.77 | LEONORCUEVA (12), LICENCIADOROJAS (1), CERVANTES (1), MELO (1) |
| medium | `PedroRoseteNino_SoloenDioslaconfianza` | CASTROYSALAZAR | 70 | 44/70 (63%) | 10.74 | CASTROYSALAZAR (44), SANDOVAL (5), VIDALYSALVADOR (4), MOLINAYMENDOZA (3), GARCIAMARCOS (2) |
| medium | `VALLEJO_Carlos_SanHermenegildo_Novena` | HOZYMOTA | 65 | 46/65 (71%) | 10.67 | HOZYMOTA (46), GARCIADEPRADO (14), GONZALEZDEBARCIA (2), VARGASMACHUCA (1), VIDALYSALVADOR (1) |
| medium | `JuandelCastillo_EsclavosdesuesclavayHacerbienn` | VIDALYSALVADOR | 68 | 47/68 (69%) | 10.59 | VIDALYSALVADOR (47), CASTROYSALAZAR (11), LICENCIADOROJAS (1), HURTADODEMENDOZA (1), LOPEZJACINTO (1) |
| medium | `MoretoyCavanaAgustinAtribuido_HermanosencontradosLos` | MOLINAYMENDOZA | 61 | 47/61 (77%) | 10.58 | MOLINAYMENDOZA (47), GONZALEZDEBARCIA (3), VIDALYSALVADOR (1) |
| medium | `Dichaydesdichadelhombre` | ROMEROROQUE | 84 | 45/84 (54%) | 10.51 | ROMEROROQUE (45), CALLE (12), GARCIAMARCOS (6), SANDOVAL (5), CASTROYSALAZAR (3) |
| medium | `LapuertaMacarena` | PAREDES | 78 | 54/78 (69%) | 10.24 | PAREDES (54), GONZALEZDETORRES (4), VIDALYSALVADOR (2), CASTROYSALAZAR (2), GARCIAMARCOS (2) |
| medium | `FrancisodeAvellanedadelaCuevay_VolverseelrayoenlaureloSeguira` | LEIVARAMIREZ | 131 | 92/131 (70%) | 10.11 | LEIVARAMIREZ (92), CALLE (13), MORETO (2), VERATASSIS (1), ROSETENINO (1) |
| medium | `BoleayAlvaradoJuande_PatronadelasmusasdiscipuladeSa` | BOLEAYALVARADO | 73 | 40/73 (55%) | 10.10 | BOLEAYALVARADO (40), MOLINAYMENDOZA (19), CANIZARES (4), SANDOVAL (1), VELEZ (1) |
| medium | `JoseGarcesAtribuidoAnonimo_OrganistadelcieloSantaCeciliaP` | VIDALYSALVADOR | 136 | 121/136 (89%) | 9.93 | VIDALYSALVADOR (121), QUEVEDO (5), VALDIVIELSO (2), VARGASMACHUCA (1), HURTADODEMENDOZA (1) |
| medium | `CastroyBellvisGuillende_Ingratitudporamor` | PSEUDOHURTADODEMENDOZA | 115 | 87/115 (76%) | 9.87 | PSEUDOHURTADODEMENDOZA (87), CERVANTES (2), BELMONTE (2), DIAMANTE (1), VIDALYSALVADOR (1) |
| medium | `AntoniodeSolisMonteserFrancisc_RenegadadeValladolidLa` | FAJARDOYACEVEDO | 105 | 94/105 (90%) | 9.83 | FAJARDOYACEVEDO (94), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), LEONORCUEVA (1) |
| medium | `ElmayorReydelosreyes` | ROJASZORRILLA | 66 | 42/66 (64%) | 9.79 | ROJASZORRILLA (42), QUEVEDO (5), GALLEGOS (4), BELMONTE (3), CONTRERAS (1) |
| medium | `VILLAMEDIANA_GloriaNiquea` | MELO | 56 | 39/56 (70%) | 9.71 | MELO (39), GOMEZACOSTA (6), LICENCIADOROJAS (2), GONZALEZDETORRES (1), ONAVIEDMAYTORRES (1) |
| medium | `JeronimodeCancerAtribuido_CondesdeCarrionLos` | GARCIAMARCOS | 59 | 46/59 (78%) | 9.41 | GARCIAMARCOS (46), VIDALYSALVADOR (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), MOLINAYMENDOZA (1) |
| medium | `Papelesvariosgongorinos_013` | CALLE | 100 | 89/100 (89%) | 9.31 | CALLE (89), JIMENEZSEDENO (3), FAJARDOYACEVEDO (2), SARAVIAYMENDOZA (1), CANIZARES (1) |
| medium | `FranciscoAntoniodeBancesCandam_Sangrevaloryfortuna` | LEIVARAMIREZ | 47 | 24/47 (51%) | 9.30 | LEIVARAMIREZ (24), ROSETENINO (4), TORRESLORENZODE (4), MORETO (2), GONZALEZDEBARCIA (1) |
| medium | `MiradeAmescuaAntonioLuisdeBelm_MartirdeMadridNohaymalqueporbi` | BELMONTE | 59 | 30/59 (51%) | 9.29 | BELMONTE (30), ANDOSILLA (11), REMON (4), ALARCON (3), LOPEZJACINTO (1) |
| medium | `JuanBautistaDiamante_NacimientodeCristoLaanunciacio` | PAREDES | 42 | 29/42 (69%) | 9.15 | PAREDES (29), COELLO (4), LICENCIADOROJAS (1), BANCESCANDAMO (1) |
| medium | `VELEZDEGUEVARA_Nohaycontravalorencantos_Austria` | MELO | 114 | 112/114 (98%) | 9.14 | MELO (112), CERVANTES (1) |
| medium | `MoretoyCavanaAgustin_Nopuedeser` | CASTROYSALAZAR | 56 | 32/56 (57%) | 9.08 | CASTROYSALAZAR (32), SANDOVAL (12), LICENCIADOROJAS (1), BELMONTE (1), GILENRIQUEZ (1) |
| medium | `TellezGabriel_Sutilezasdeamor` | PSEUDOHURTADODEMENDOZA | 60 | 43/60 (72%) | 9.06 | PSEUDOHURTADODEMENDOZA (43), BELMONTE (3), VELEZ (2), CONTRERAS (1) |
| medium | `MatosFragosoJuande_Inocenciaperseguidayvenganzaen` | MOLINAYMENDOZA | 64 | 44/64 (69%) | 9.04 | MOLINAYMENDOZA (44), BELMONTE (13), ENRIQUEZ (1), PSEUDOHURTADODEMENDOZA (1), CALLE (1) |
| medium | `TellezGabriel_MayordesenganoEl` | CUEVAYSILVA | 33 | 24/33 (73%) | 8.99 | CUEVAYSILVA (24), CASTILLOSOLORZANO (1) |
| medium | `VegaCarpioLopede_LocoporfuerzaEl` | LANINI | 62 | 52/62 (84%) | 8.93 | LANINI (52), PACHECO (2), AVELLANEDA (1), LOPEZDECARDENA (1) |
| medium | `FranciscodePaulaGonzalezdeBust_MosqueterodeFlandesEl` | GALLEGOS | 94 | 82/94 (87%) | 8.93 | GALLEGOS (82), GONZALEZDEBARCIA (1), RUANO (1) |
| medium | `MiradeAmescuaAntonio_MontedelapiedadEl` | BELMONTE | 24 | 14/24 (58%) | 8.90 | BELMONTE (14), MONTALBAN (2), CANIZARES (1), LOPEZDECASTRO (1), LEONORCUEVA (1) |
| medium | `QuevedoyVillegasFranciscodeAtr_MudanzasdeFortunaRigordelasdes` | SANDOVAL | 65 | 37/65 (57%) | 8.82 | SANDOVAL (37), BELMONTE (12), FAJARDOYACEVEDO (4), PAREDES (2), CARVAJAL (1) |
| medium | `LuisdeBelmonteBermudez_MayorcontrarioamigoEl` | SANDOVAL | 59 | 46/59 (78%) | 8.77 | SANDOVAL (46), CASTROYSALAZAR (2), GILENRIQUEZ (2), LICENCIADOROJAS (1), CERVANTES (1) |
| medium | `FONTANELLA_Miscel_dramatico` | VIDALYSALVADOR | 300 | 281/300 (94%) | 8.75 | VIDALYSALVADOR (281), GONZALEZDEBARCIA (5), GARCIADEPRADO (2), ENRIQUEZ (1), VERATASSIS (1) |
| medium | `Poesasvariasdediferentesautores` | CASTROYSALAZAR | 222 | 140/222 (63%) | 8.70 | CASTROYSALAZAR (140), VIDALYSALVADOR (70), VERATASSIS (2), MARCHANTE (2), GONZALEZDETORRES (1) |
| medium | `Obrasdiversasenversoyenprosa_2` | VIDALYSALVADOR | 176 | 142/176 (81%) | 8.69 | VIDALYSALVADOR (142), VARGASMACHUCA (11), CASTROYSALAZAR (6), ENRIQUEZ (3), CECILIANACIMIENTO (3) |
| medium | `BACHILLERRINCON_PeorEstaQueEstaba` | MELO | 4 | 2/4 (50%) | 8.67 | MELO (2), CECILIANACIMIENTO (1), LOPEZJACINTO (1) |
| medium | `JUANAINES_VillancicosNolasco` | LICENCIADOROJAS | 5 | 5/5 (100%) | 8.66 | LICENCIADOROJAS (5) |
| medium | `Elpleitomatrimonialdelcuerpoyelalma3` | CASTROYSALAZAR | 54 | 39/54 (72%) | 8.64 | CASTROYSALAZAR (39), VIDALYSALVADOR (4), MOLINAYMENDOZA (3), CARVAJAL (2), SANDOVAL (1) |
| medium | `GODINEZ_TorosdelAlma` | QUEVEDO | 22 | 15/22 (68%) | 8.62 | QUEVEDO (15), REMON (3), BELMONTE (2), LOPE (1), MONTALBAN (1) |
| medium | `Autornoencontrado_Loasacramental` | SANDOVAL | 6 | 3/6 (50%) | 8.55 | SANDOVAL (3), LEONORCUEVA (1) |
| medium | `ROSETE_ExaltacionAveMaria` | CASTROYSALAZAR | 71 | 57/71 (80%) | 8.48 | CASTROYSALAZAR (57), MOLINAYMENDOZA (7), ROMEROROQUE (2), SANDOVAL (1), GARCIAMARCOS (1) |
| medium | `MiradeAmescuaAntonioAtribuidoJ_BatalladelAlbisymayorhechodeCa` | GARCIAMARCOS | 68 | 45/68 (66%) | 8.44 | GARCIAMARCOS (45), SANDOVAL (7), PAREDES (3), LORENZANA (1), CLARAMONTE (1) |
| medium | `GONZALEZDEBUSTOS_LaGranRosaDeViterboOSantaRosaDeViterbo` | MEDINA | 73 | 55/73 (75%) | 8.41 | MEDINA (55), MELO (15) |
| medium | `PedroRoseteNinoAtribuido_Miraalfin` | MESA | 66 | 38/66 (58%) | 8.41 | MESA (38), TORRESLORENZODE (8), LEIVARAMIREZ (6), BANCESCANDAMO (1), VILLEGASDELACRUZ (1) |
| medium | `Porsureyyporsudama2` | GILENRIQUEZ | 72 | 42/72 (58%) | 8.40 | GILENRIQUEZ (42), BELMONTE (16), MOLINAYMENDOZA (2), CORDERO (1), SANDOVAL (1) |
| medium | `COMEDIA_AlmaCorpusChristi` | BENAVIDES | 65 | 65/65 (100%) | 8.37 | BENAVIDES (65) |
| medium | `PolidorComedia-II-1591` | AVELLANEDA | 114 | 95/114 (83%) | 8.35 | AVELLANEDA (95), LICENCIADOROJAS (15), CASTILLOSOLORZANO (1) |
| medium | `MonteserFranciscoAntoniode_CaballerodeOlmedoEl` | JIMENEZSEDENO | 36 | 23/36 (64%) | 8.26 | JIMENEZSEDENO (23), FAJARDOYACEVEDO (3), GONZALEZDEBARCIA (1), PAREDES (1) |
| medium | `ArroyoJosede_InocenciaeneldesiertoSantaGeno` | MOLINAYMENDOZA | 61 | 36/61 (59%) | 8.21 | MOLINAYMENDOZA (36), FAJARDOYACEVEDO (14), GONZALEZDEBARCIA (4), AGUADOELVIEJO (1), JIMENEZSEDENO (1) |
| medium | `VegaCarpioLopede_IsladelsolLa` | BELMONTE | 67 | 36/67 (54%) | 8.05 | BELMONTE (36), BATRES (3), ENRIQUEZ (2), CASTILLOSOLORZANO (1), LEONORCUEVA (1) |
| medium | `AntonioEnriquezGomezAtribuido_Culpamasprovechosayvidaymuerte` | VIDALYSALVADOR | 76 | 56/76 (74%) | 8.04 | VIDALYSALVADOR (56), CANIZARES (3), MOLINAYMENDOZA (3), LICENCIADOROJAS (1), VERATASSIS (1) |
| medium | `ARBOREDA_Enganoshayquesonjustos` | FAJARDOYACEVEDO | 83 | 45/83 (54%) | 8.03 | FAJARDOYACEVEDO (45), LEIVARAMIREZ (24), LICENCIADOROJAS (1), LEONORCUEVA (1), QUINONES (1) |
| medium | `VELEZDEGUEVARA_TabernayelbodegonLa` | MELO | 10 | 10/10 (100%) | 8.02 | MELO (10) |
| medium | `VARIOS_MiscelaneosRealBiblioteca` | CECILIANACIMIENTO | 24 | 12/24 (50%) | 7.99 | CECILIANACIMIENTO (12), GOMEZACOSTA (5), VALDIVIELSO (2), VARGASMACHUCA (2), BARRIONUEVO (1) |
| medium | `NAJERA_AguaDeMejorVidaEl` | GONZALEZDEBARCIA | 60 | 41/60 (68%) | 7.96 | GONZALEZDEBARCIA (41), VIDALYSALVADOR (8), FAJARDOYACEVEDO (2), LICENCIADOROJAS (1), VARGASMACHUCA (1) |
| medium | `FONTANELLA_AmorFirmesaIPorfia` | VIDALYSALVADOR | 384 | 292/384 (76%) | 7.95 | VIDALYSALVADOR (292), GODINEZMANRIQUE (30), VARGASMACHUCA (16), PAREDES (8), CECILIANACIMIENTO (7) |
| medium | `AgustindeSalazaryTorres_Bailedelherbolario` | GONZALEZDEBARCIA | 346 | 175/346 (51%) | 7.92 | GONZALEZDEBARCIA (175), VIDALYSALVADOR (56), LOPEZDELCAMPO (28), CASTILLOSOLORZANO (11), CECILIANACIMIENTO (9) |
| medium | `SegundapartedelapuertaMacarena` | PAREDES | 73 | 50/73 (68%) | 7.91 | PAREDES (50), GARCIAMARCOS (5), JIMENEZSEDENO (2), AVELLANEDADELACUEVA (2), SARAVIAYMENDOZA (1) |
| medium | `FranciscodeVillegasAtribuidoJu_ReydonSebastianPortuguesmasher` | MOLINAYMENDOZA | 65 | 44/65 (68%) | 7.85 | MOLINAYMENDOZA (44), GONZALEZDEBARCIA (4), GALLEGOS (3), JIMENEZSEDENO (1) |
| medium | `VelezdeGuevaraLuis_NinfadelcieloCondesabandoleray` | VILLEGASJUANBAUTISTA | 61 | 33/61 (54%) | 7.80 | VILLEGASJUANBAUTISTA (33), ROJASZORRILLA (6), CLARAMONTE (4), BELMONTE (3), CAXESI (2) |
| medium | `YRAZABAL_Celossinsaber` | VIDALYSALVADOR | 70 | 52/70 (74%) | 7.79 | VIDALYSALVADOR (52), CASTROYSALAZAR (15), ENRIQUEZ (1), MARCHANTE (1), BELMONTE (1) |
| medium | `BRAVO_AMasDesdenMasAmor` | PAREDES | 57 | 31/57 (54%) | 7.78 | PAREDES (31), ROMEROROQUE (14), SANDOVAL (1), TORRESLORENZODE (1), FAJARDOYACEVEDO (1) |
| medium | `CASTRO_MONTESER_Hidalga` | VIDALYSALVADOR | 4 | 3/4 (75%) | 7.72 | VIDALYSALVADOR (3) |
| medium | `Papelesvariosgongorinos_014` | CALLE | 111 | 91/111 (82%) | 7.72 | CALLE (91), JIMENEZSEDENO (12), FAJARDOYACEVEDO (2), GILENRIQUEZ (1) |
| medium | `VegaCarpioLopedeAtribuidoMonta_PrincipedonCarlosEl` | MESA | 65 | 52/65 (80%) | 7.69 | MESA (52), ROSETENINO (2), VIDALYSALVADOR (1), AVELLANEDA (1) |
| medium | `MORALES_Amoresylocurasdelcondeloco` | BELMONTE | 29 | 25/29 (86%) | 7.65 | BELMONTE (25), VIDALYSALVADOR (2), PAREDES (1), AMESCUA (1) |
| medium | `VACA_NinoPerdido` | BELMONTE | 12 | 10/12 (83%) | 7.63 | BELMONTE (10), BATRES (1), ALARCON (1) |
| medium | `ElpastorFido` | GONZALEZDEBARCIA | 50 | 39/50 (78%) | 7.54 | GONZALEZDEBARCIA (39), GARCIADEPRADO (2) |
| medium | `TARREGA_MoriscosHornachos` | RUIZALCEO | 28 | 20/28 (71%) | 7.53 | RUIZALCEO (20), TORRESLORENZODE (4), MEDINA (2), VARGAS (1), TAMAYO (1) |
| medium | `VegaCarpioLopede_SanAgustinoEldivinoafricano` | LOPEZDECASTRO | 42 | 22/42 (52%) | 7.51 | LOPEZDECASTRO (22), LORENZANA (4), ONAVIEDMAYTORRES (3), GOMEZACOSTA (2), CERVANTES (1) |
| medium | `Losojosdelcielo` | CAXESI | 43 | 27/43 (63%) | 7.49 | CAXESI (27), ROJASVILLANDRANDO (3), SALAZARYTORRES (2), CASTILLOSOLORZANO (1), MEDINA (1) |
| medium | `MelchorFernandezdeLeon_IcaroyDedalo` | ROMEROROQUE | 58 | 47/58 (81%) | 7.48 | ROMEROROQUE (47), FAJARDOYACEVEDO (6), CASTILLOSOLORZANO (2) |
| medium | `COUTOPESTANA_HechizoDeAmorLosCelos` | PAREDES | 41 | 32/41 (78%) | 7.47 | PAREDES (32), BELMONTE (5), GONZALEZDEBARCIA (1), TORRESLORENZODE (1), CASTILLOSOLORZANO (1) |
| medium | `CASTRO_LoQueSonMujeres_British` | MORETO | 32 | 21/32 (66%) | 7.47 | MORETO (21), ROSETENINO (3), LANINI (2), BELMONTE (1), ROJASZORRILLA (1) |
| medium | `FajardoyAcevedoAntonio_ValorhacefortunaEl` | FAJARDOYACEVEDO | 139 | 102/139 (73%) | 7.40 | FAJARDOYACEVEDO (102), VIDALYSALVADOR (2), LICENCIADOROJAS (1), CARVAJAL (1), REMON (1) |
| medium | `JuanBautistadeVillegas_Moricagarridayhermanosmasamant` | MESA | 60 | 34/60 (57%) | 7.39 | MESA (34), BELMONTE (9), MONTALBAN (2), ROJASZORRILLA (2), CERVANTES (1) |
| medium | `MontalbanJuanPerezdeAtribuido_ObrarbienqueDiosdeDios` | GARCIAMARCOS | 64 | 51/64 (80%) | 7.38 | GARCIAMARCOS (51), CALLE (2), CARVAJAL (1), CASTILLOSOLORZANO (1), SANDOVAL (1) |
| medium | `SUAREZ_DeLaNocheALaManana` | GARCIADEPRADO | 53 | 41/53 (77%) | 7.37 | GARCIADEPRADO (41), CARVAJAL (10), AVELLANEDADELACUEVA (1), LEIVARAMIREZ (1) |
| medium | `CanizaresySuarezdeToledoJosede_Salirelamordelmundo` | CANIZARES | 31 | 16/31 (52%) | 7.35 | CANIZARES (16), VIDALYSALVADOR (5), GONZALEZDEBARCIA (1) |
| medium | `JuanDiazdelaCalle_DejarporDioslacoronayprodigios` | VIDALYSALVADOR | 116 | 102/116 (88%) | 7.27 | VIDALYSALVADOR (102), PAREDES (7), CASTILLOSOLORZANO (2), VARGASMACHUCA (1), VERATASSIS (1) |
| medium | `CAIRASCOFIGUEROA_RecibimientoObispoCanarias` | BENAVIDES | 37 | 36/37 (97%) | 7.23 | BENAVIDES (36), VARGASMACHUCA (1) |
| medium | `ElprincipeDonCarlos` | CASTROYSALAZAR | 71 | 38/71 (54%) | 7.21 | CASTROYSALAZAR (38), GARCIAMARCOS (20), VIDALYSALVADOR (2), LICENCIADOROJAS (1), SANDOVAL (1) |
| medium | `Elgalanfantasma` | GARCIADEPRADO | 59 | 34/59 (58%) | 7.14 | GARCIADEPRADO (34), GILENRIQUEZ (7), BELMONTE (2), CANIZARES (2), CALDERON (2) |
| medium | `VegaCarpioLopede_PrincipeperfectoPrimeraparteEl` | CALLE | 179 | 96/179 (54%) | 7.07 | CALLE (96), SARAVIAYMENDOZA (13), MONTALBAN (6), GARCIAMARCOS (5), QUINONES (4) |
| medium | `LuisdeBelmonteBermudez_Elmayorcontrarioamigo` | GONZALEZDEBARCIA | 71 | 46/71 (65%) | 7.01 | GONZALEZDEBARCIA (46), VIDALYSALVADOR (7), PAREDES (7), CORDERO (2), ENRIQUEZ (2) |
| medium | `QUINONESDEBENAVENTE_OtanezYFariseo` | VIDALYSALVADOR | 10 | 8/10 (80%) | 6.99 | VIDALYSALVADOR (8), ENRIQUEZ (1) |
| medium | `TellezGabriel_BellacosoisGomez` | TORRESLORENZODE | 52 | 36/52 (69%) | 6.99 | TORRESLORENZODE (36), BATRES (2), LICENCIADOROJAS (1), VIDALYSALVADOR (1), QUINONES (1) |
| medium | `RojasZorrillaFranciscodeLuisde_Mejoramigoelmuertoycapuchinoes` | ANDOSILLA | 66 | 41/66 (62%) | 6.98 | ANDOSILLA (41), CANIZARES (7), AGUADOELVIEJO (5), MOLINAYMENDOZA (2), LICENCIADOROJAS (1) |
| medium | `ElreydonSebastianyPortuguesmasheroico` | CANIZARES | 22 | 11/22 (50%) | 6.85 | CANIZARES (11), MORETO (2), CASTROYSALAZAR (2), BOLEAYALVARADO (1), SANDOVAL (1) |
| medium | `MiradeAmescuaAntonio_NuestraSenoradelosRemedios` | ROMEROROQUE | 32 | 20/32 (62%) | 6.84 | ROMEROROQUE (20), FAJARDOYACEVEDO (2), GONZALEZDEBARCIA (1), SANDOVAL (1), MOLINAYMENDOZA (1) |
| medium | `VegaCarpioLopedeAtribuido_Guardaryguardarse` | FAJARDOYACEVEDO | 74 | 52/74 (70%) | 6.83 | FAJARDOYACEVEDO (52), CALLE (3), ROMEROROQUE (2), GONZALEZDEBARCIA (1), GARCIADEPRADO (1) |
| medium | `VARIOS_AGranDanoGranRemedio` | GARCIAMARCOS | 73 | 54/73 (74%) | 6.81 | GARCIAMARCOS (54), PAREDES (2), CORDERO (2), GONZALEZDEBARCIA (1), CARVAJAL (1) |
| medium | `CARUJO_Extranjeroensupatria` | VARGASMACHUCA | 157 | 130/157 (83%) | 6.80 | VARGASMACHUCA (130), MELO (15), CASTILLOSOLORZANO (1), CERVANTES (1) |
| medium | `GODINEZ_OtroRomance` | VERATASSIS | 3 | 2/3 (67%) | 6.78 | VERATASSIS (2), GILENRIQUEZ (1) |
| medium | `JeronimoVillaizan_Ofenderconlasfinezas` | CALLE | 67 | 48/67 (72%) | 6.77 | CALLE (48), GILENRIQUEZ (6), SANDOVAL (3), GONZALEZDETORRES (1), GARCIADEPRADO (1) |
| medium | `VegaCarpioLopedeAtribuido_SantaCasilda` | SANDOVAL | 51 | 31/51 (61%) | 6.76 | SANDOVAL (31), TORRESLORENZODE (2), BELMONTE (2), FAJARDOYACEVEDO (1), ONAVIEDMAYTORRES (1) |
| medium | `TELLEZ_AmorYAmistad` | LEIVARAMIREZ | 66 | 37/66 (56%) | 6.75 | LEIVARAMIREZ (37), JUANDESOTO (14), GARCIAMARCOS (2), TORRESLORENZODE (2), LICENCIADOROJAS (1) |
| medium | `AntonioEnriquezGomez_GrancardenaldeEspanadonGildeAl` | SANDOVAL | 65 | 35/65 (54%) | 6.73 | SANDOVAL (35), CASTROYSALAZAR (21), LICENCIADOROJAS (1), PSEUDOHURTADODEMENDOZA (1), MOLINAYMENDOZA (1) |
| medium | `ANUNCIBAY_SegundoAlejandro` | CARVAJAL | 51 | 35/51 (69%) | 6.72 | CARVAJAL (35), CERVANTES (8), REMON (2), QUEVEDO (1), ENRIQUEZ (1) |
| medium | `QUINONESDEBENAVENTE_Comilon1` | QUINONES | 8 | 8/8 (100%) | 6.71 | QUINONES (8) |
| medium | `MoretoyCavanaAgustin_Loquepuedelaaprension` | GARCIADEPRADO | 64 | 49/64 (77%) | 6.68 | GARCIADEPRADO (49), CALLE (3), CALDERON (3), GILENRIQUEZ (2), BELMONTE (1) |
| medium | `LoshijosdelaBarbuda2` | CANIZARES | 71 | 57/71 (80%) | 6.68 | CANIZARES (57), REMON (2), AVELLANEDADELACUEVA (1), LEIVARAMIREZ (1), GARCIADEPRADO (1) |
| medium | `CanizaresySuarezdeToledoJosede_IlustrefregonaLa` | CASTROYSALAZAR | 75 | 40/75 (53%) | 6.65 | CASTROYSALAZAR (40), GONZALEZDETORRES (6), VIDALYSALVADOR (5), VERATASSIS (3), SANDOVAL (3) |
| medium | `ARBOREDA_MasDivinoRemedio` | CALDERON | 118 | 62/118 (52%) | 6.62 | CALDERON (62), GARCIADEPRADO (36), QUINONES (5), LEONORCUEVA (1), AMESCUA (1) |
| medium | `AntonioEnriquezGomez_SantaTaez` | FAJARDOYACEVEDO | 72 | 59/72 (82%) | 6.58 | FAJARDOYACEVEDO (59), LICENCIADOROJAS (1), ANDOSILLA (1), LEONORCUEVA (1), QUINONES (1) |
| medium | `VILLAROEL_PurpuraCatalanaSanRamon` | MEDINA | 52 | 48/52 (92%) | 6.57 | MEDINA (48), SANDOVAL (1), GILENRIQUEZ (1), CERVANTES (1), MULSA (1) |
| medium | `LospastoresdeBelen` | ROMEROROQUE | 25 | 14/25 (56%) | 6.56 | ROMEROROQUE (14), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), ANDOSILLA (1), FAJARDOYACEVEDO (1) |
| medium | `AntoniodeZamora_GurruminasLas` | MOLINAYMENDOZA | 12 | 6/12 (50%) | 6.52 | MOLINAYMENDOZA (6), GONZALEZDEBARCIA (1), CANIZARES (1), JIMENEZSEDENO (1), LICENCIADOROJAS (1) |
| medium | `CANCER_ROSETE_ROJASZORRILLA_BandoleroSolposto` | VERATASSIS | 35 | 22/35 (63%) | 6.52 | VERATASSIS (22), LOPEZDECARDENA (10), VIDALYSALVADOR (1), MORETO (1), ROSETENINO (1) |
| medium | `MoretoyCavanaAgustinAtribuido_SatisfacercallandoEl` | ROMEROROQUE | 57 | 44/57 (77%) | 6.52 | ROMEROROQUE (44), FAJARDOYACEVEDO (2), PAREDES (1) |
| medium | `QUINONESDEBENAVENTE_DosLetras` | QUINONES | 9 | 5/9 (56%) | 6.51 | QUINONES (5), MESA (1) |
| medium | `CanizaresySuarezdeToledoJosede_PicaritoenEspanaEl` | MOLINAYMENDOZA | 65 | 41/65 (63%) | 6.49 | MOLINAYMENDOZA (41), FAJARDOYACEVEDO (10), ROMEROROQUE (6), LICENCIADOROJAS (1), GARCIAMARCOS (1) |
| medium | `GodinezManriqueFelipe_IgnorantediscretoAutoalodivino` | GALLEGOS | 35 | 18/35 (51%) | 6.48 | GALLEGOS (18), BELMONTE (4), ROJASZORRILLA (3), CLARAMONTE (2), PACHECO (1) |
| medium | `ElmayorReydelosreyes2` | LICENCIADOROJAS | 36 | 24/36 (67%) | 6.48 | LICENCIADOROJAS (24), LEONORCUEVA (1), SALAZARYTORRES (1), MESA (1) |
| medium | `FranciscoTomasdeCastellanos_RenegadoFranciscoymartirmasval` | ROMEROROQUE | 53 | 47/53 (89%) | 6.47 | ROMEROROQUE (47), LICENCIADOROJAS (1), GONGORA (1) |
| medium | `LuisdeBelmonteBermudezFrancisc_ElmayorcontrarioamigoEldemonio` | MOLINAYMENDOZA | 73 | 44/73 (60%) | 6.45 | MOLINAYMENDOZA (44), GALLEGOS (13), GONZALEZDEBARCIA (2), LICENCIADOROJAS (1), CASTILLOSOLORZANO (1) |
| medium | `VegaCarpioLopede_CompetenciaenlosnoblesLa` | GALLEGOS | 38 | 23/38 (60%) | 6.45 | GALLEGOS (23), ROMEROROQUE (5), LICENCIADOROJAS (2), SANDOVAL (2), LEONORCUEVA (1) |
| medium | `VegaCarpioLopede_LocuraporelalmaLa` | CALLE | 71 | 50/71 (70%) | 6.45 | CALLE (50), LOPEZDECASTRO (3), TORRESLORENZODE (2), ROMEROROQUE (1), PACHECO (1) |
| medium | `JeronimodeCancerAlonsoAlfaroLu_LunaafricanaLa` | GARCIADEPRADO | 86 | 58/86 (67%) | 6.43 | GARCIADEPRADO (58), VIDALYSALVADOR (8), GONZALEZDEBARCIA (1), LOPEZDECARDENA (1), MORETO (1) |
| medium | `AntonioEnriquezGomez_SoberbiadeNembrotLa` | CECILIANACIMIENTO | 44 | 24/44 (55%) | 6.39 | CECILIANACIMIENTO (24), VIDALYSALVADOR (5), CONTRERAS (5), PAREDES (1), VARGASMACHUCA (1) |
| medium | `JoseLopezdeSedano_DeshonraestaenlaculpaLa` | CUEVAYSILVA | 77 | 40/77 (52%) | 6.35 | CUEVAYSILVA (40), LOPEZDECARDENA (26), GARCIAMARCOS (1), AVELLANEDA (1) |
| medium | `CanizaresySuarezdeToledoJosede_Siunavezllegaaquererlamasfirme` | SANDOVAL | 74 | 52/74 (70%) | 6.34 | SANDOVAL (52), MOLINAYMENDOZA (9), CERVANTES (1), GONZALEZDEBARCIA (1), CASTROYSALAZAR (1) |
| medium | `Elcaballerodelaardienteespada` | CARVAJAL | 33 | 17/33 (52%) | 6.31 | CARVAJAL (17), CAXESI (4), CONTRERAS (2), LORENZANA (2) |
| medium | `VegaCarpioLopede_ObediencialaureadayprimerCarlo` | MESA | 71 | 42/71 (59%) | 6.30 | MESA (42), ANDOSILLA (15), TAMAYO (2), QUINONES (2), LICENCIADOROJAS (1) |
| medium | `OTEIZA_AtreoDesdichado_Autografo` | ROSETENINO | 52 | 40/52 (77%) | 6.25 | ROSETENINO (40), MULSA (3), GARCIAMARCOS (3), AVELLANEDA (1), LEIVARAMIREZ (1) |
| medium | `LarenunciaciondelreyWambayfundaciondelaVirgendelaMata` | MOLINAYMENDOZA | 66 | 37/66 (56%) | 6.25 | MOLINAYMENDOZA (37), FAJARDOYACEVEDO (16), ROMEROROQUE (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| medium | `Obrasdiversasenversoyenprosa_1` | VIDALYSALVADOR | 175 | 119/175 (68%) | 6.25 | VIDALYSALVADOR (119), VARGASMACHUCA (24), ENRIQUEZ (21), CASTILLOSOLORZANO (3), PAREDES (2) |
| medium | `AntonioManueldelCampo_RenegadodeFranciaySantoCristod` | AVELLANEDA | 75 | 64/75 (85%) | 6.25 | AVELLANEDA (64), VIDALYSALVADOR (1), CERVANTES (1), CONTRERAS (1), VARGASMACHUCA (1) |
| medium | `DiegodeFigueroayCordobaAtribui_DonaRodriguez` | MARCHANTE | 17 | 9/17 (53%) | 6.24 | MARCHANTE (9), ONAVIEDMAYTORRES (5), GONZALEZDEBARCIA (1), LICENCIADOROJAS (1) |
| medium | `AntonioFolchdeCardonaAlagon_Lomejoreslomejor` | CASTILLOSOLORZANO | 99 | 67/99 (68%) | 6.23 | CASTILLOSOLORZANO (67), VIDALYSALVADOR (8), RUANO (4), SANDOVAL (3), GONZALEZDEBARCIA (3) |
| medium | `FrancisodeAvellanedadelaCuevay_CapuchinoescocesysegundosanAle` | PAREDES | 72 | 43/72 (60%) | 6.22 | PAREDES (43), LANINI (21), LOPEZJACINTO (1) |
| medium | `FranciscoAntoniodeCastroySalaz_Elgaranon` | VARGASMACHUCA | 14 | 10/14 (71%) | 6.19 | VARGASMACHUCA (10) |
| medium | `PorsureyyporsudamaoMseselruidoquelasnueces` | BOLEAYALVARADO | 69 | 45/69 (65%) | 6.17 | BOLEAYALVARADO (45), GILENRIQUEZ (6), GARCIAMARCOS (3), CALLE (2), LLOBREGATYESTEVE (1) |
| medium | `JuandeLemusAtribuidoMoretoyCav_Nadiepierdalaesperanza` | BELMONTE | 64 | 34/64 (53%) | 6.02 | BELMONTE (34), BATRES (17), GONZALEZDEBARCIA (1), ALARCON (1), FAJARDOYACEVEDO (1) |
| medium | `VegaCarpioLopede_FuerzalastimosaLa` | GARCIAMARCOS | 78 | 57/78 (73%) | 6.01 | GARCIAMARCOS (57), PAREDES (6), ROMEROROQUE (6), GONZALEZDEBARCIA (1) |
| medium | `LOPEZDEBENAVIDES_JoyaDeLasMontanas` | CONTRERAS | 82 | 47/82 (57%) | 5.97 | CONTRERAS (47), QUINONES (18), HURTADODEMENDOZA (13), GARCIADEPRADO (2), CALDERON (1) |
| medium | `TellezGabriel_MujerquemandaencasaAcabyEliasL` | ANDOSILLA | 66 | 45/66 (68%) | 5.94 | ANDOSILLA (45), TIRSO (5), QUINONES (2), TAMAYO (1), LEIVARAMIREZ (1) |
| medium | `LosmrtiresdeMadridydejarunreinoporotro` | CASTROYSALAZAR | 61 | 33/61 (54%) | 5.90 | CASTROYSALAZAR (33), MELO (8), SANDOVAL (5), ONAVIEDMAYTORRES (3), HURTADODEMENDOZA (1) |
| medium | `MarceloAntoniodeAyalayGuzman_TravesurasdeDLuisCoelloprimera` | TORRESLORENZODE | 128 | 81/128 (63%) | 5.90 | TORRESLORENZODE (81), ROMEROROQUE (14), LANINI (12), CASTROYSALAZAR (5), VIDALYSALVADOR (1) |
| medium | `AntoniodeZamora_LoaparaelautoEltemplovivodeDio` | VIDALYSALVADOR | 387 | 261/387 (67%) | 5.90 | VIDALYSALVADOR (261), CASTILLOSOLORZANO (53), VARGASMACHUCA (19), MARCHANTE (13), ENRIQUEZ (11) |
| medium | `VARIOS_AutosMonasterioNuestraSenoraCruz` | ENRIQUEZ | 76 | 61/76 (80%) | 5.87 | ENRIQUEZ (61), CASTILLOSOLORZANO (4), CERVANTES (3), CONTRERAS (2), AMESCUA (1) |
| medium | `VegaCarpioLopedeAtribuido_MayorcoronaLa` | ANDOSILLA | 64 | 37/64 (58%) | 5.86 | ANDOSILLA (37), MESA (13), TAMAYO (3), GONZALEZDEBARCIA (1), MEDINA (1) |
| medium | `QUINONESDEBENAVENTE_Comilon` | QUINONES | 20 | 14/20 (70%) | 5.86 | QUINONES (14), MESA (2), VIDALYSALVADOR (1) |
| medium | `VALLEJO_Carlos_Amar_es_saber_vencer_Novena` | CASTROYSALAZAR | 75 | 45/75 (60%) | 5.85 | CASTROYSALAZAR (45), VIDALYSALVADOR (9), GILENRIQUEZ (7), BOLEAYALVARADO (6), CANIZARES (4) |
| medium | `CARDENAS_PeligrosporamarLos_Autografo` | GONZALEZDEBARCIA | 30 | 21/30 (70%) | 5.83 | GONZALEZDEBARCIA (21), VIDALYSALVADOR (6), CERVANTES (2) |
| medium | `FANNINISAGREDO_Habladme_en_entrando_Novena` | GILENRIQUEZ | 61 | 33/61 (54%) | 5.82 | GILENRIQUEZ (33), CANIZARES (13), SANDOVAL (4), CASTROYSALAZAR (3), VARGASMACHUCA (1) |
| medium | `VidalySalvadorManuel_Contraelencantoelescudo` | MELO | 86 | 68/86 (79%) | 5.81 | MELO (68), CASTROYSALAZAR (3), GONGORA (2), VIDALYSALVADOR (2), CARVAJAL (1) |
| medium | `CALDERONatribuido_DialogopurisimaConcencao` | CERVANTES | 7 | 7/7 (100%) | 5.79 | CERVANTES (7) |
| medium | `GabrielGamez_BelloirissetavinoSacraVirgende` | SANDOVAL | 87 | 45/87 (52%) | 5.73 | SANDOVAL (45), BELMONTE (30), GONZALEZDETORRES (2), VARGASMACHUCA (1), CANIZARES (1) |
| medium | `ClaramonteAndresde_NuevoreyGallinatoyventuraporde` | ROJASVILLANDRANDO | 26 | 13/26 (50%) | 5.72 | ROJASVILLANDRANDO (13), PACHECO (5), CONTRERAS (1), LOPEZDECASTRO (1) |
| medium | `VegaCarpioLopedeAtribuido_HonraporlamujerLa` | BELMONTE | 59 | 30/59 (51%) | 5.72 | BELMONTE (30), MONTALBAN (14), QUEVEDO (4), CALDERON (1), ENRIQUEZ (1) |
| medium | `SARAVIAMENDOZA_TodoestasujetoaAmor` | SARAVIAYMENDOZA | 216 | 135/216 (62%) | 5.71 | SARAVIAYMENDOZA (135), VIDALYSALVADOR (52), VARGASMACHUCA (3), GILENRIQUEZ (2), LICENCIADOROJAS (1) |
| medium | `ACOSTA_VidabeataCaterina` | VARGASMACHUCA | 81 | 51/81 (63%) | 5.71 | VARGASMACHUCA (51), CECILIANACIMIENTO (19), CERVANTES (8), MELO (2) |
| medium | `VegaCarpioLopedeAtribuidoVelez_MejorenamoradalaMagdalenaLa` | ALARCON | 45 | 28/45 (62%) | 5.67 | ALARCON (28), ANDOSILLA (3), ROSETENINO (2), GARCIADEPRADO (2), LICENCIADOROJAS (1) |
| medium | `FOLCHDECARDONA_Obrarcontrasuintencion` | CASTROYSALAZAR | 237 | 124/237 (52%) | 5.67 | CASTROYSALAZAR (124), SANDOVAL (43), GARCIAMARCOS (35), CANIZARES (12), MORETO (7) |
| medium | `LoquevadelhombreaDios` | ROMEROROQUE | 50 | 28/50 (56%) | 5.62 | ROMEROROQUE (28), GONZALEZDEBARCIA (9), VARGASMACHUCA (1), CASTROYSALAZAR (1), FAJARDOYACEVEDO (1) |
| medium | `MiradeAmescuaAntonioMontalbanJ_PolifemoyCirce` | ROMEROROQUE | 50 | 37/50 (74%) | 5.62 | ROMEROROQUE (37), GONZALEZDEBARCIA (5), CERVANTES (1), GONGORA (1), CANIZARES (1) |
| medium | `TellezGabriel_VenturatedeDioshijo` | LEIVARAMIREZ | 59 | 41/59 (70%) | 5.62 | LEIVARAMIREZ (41), JUANDESOTO (7), TORRESLORENZODE (2), TAMAYO (1), VALDIVIELSO (1) |
| medium | `ARROYO_PobreMasPoderoso` | GARCIADEPRADO | 64 | 33/64 (52%) | 5.57 | GARCIADEPRADO (33), CARVAJAL (16), LANINI (4), CERVANTES (3), HOZYMOTA (2) |
| medium | `Nohayamigoparaamigo` | BELMONTE | 64 | 35/64 (55%) | 5.45 | BELMONTE (35), SANDOVAL (5), MESA (3), LEIVARAMIREZ (3), ANDOSILLA (2) |
| medium | `ZAMORA_AmarEsSaberVencer` | GILENRIQUEZ | 80 | 49/80 (61%) | 5.37 | GILENRIQUEZ (49), CASTROYSALAZAR (9), MARCHANTE (7), LICENCIADOROJAS (1), CALLE (1) |
| medium | `RODRIGUEZGOMEZ_Enganarparareinar` | CANIZARES | 50 | 39/50 (78%) | 5.34 | CANIZARES (39), GONZALEZDEBARCIA (2), CASTILLOSOLORZANO (1) |
| medium | `MIRADEAMESCUA_Callarenbuenaocasion` | PAREDES | 118 | 68/118 (58%) | 5.33 | PAREDES (68), TORRESLORENZODE (17), BELMONTE (13), BARRIONUEVO (6), CAXESI (2) |
| medium | `Elpleitomatrimonialdelcuerpoyelalma` | GONZALEZDEBARCIA | 50 | 36/50 (72%) | 5.32 | GONZALEZDEBARCIA (36), AVELLANEDADELACUEVA (2), GARCIADEPRADO (2), GODINEZMANRIQUE (1) |
| medium | `MiradeAmescuaAntonioAtribuido_HermosuradeFenixymatracasdeSev` | LEIVARAMIREZ | 66 | 33/66 (50%) | 5.29 | LEIVARAMIREZ (33), BELMONTE (7), GARCIAMARCOS (7), ENRIQUEZ (4), TORRESLORENZODE (1) |
| medium | `JosedeCobaledayAguilar_ConversiondesanEustachioantesl` | CECILIANACIMIENTO | 239 | 126/239 (53%) | 5.23 | CECILIANACIMIENTO (126), AVELLANEDA (47), PAREDES (25), GOMEZACOSTA (13), VARGASMACHUCA (11) |
| medium | `VegaCarpioLopede_FloresdedonJuanyRicoypobretroc` | ROMEROROQUE | 79 | 48/79 (61%) | 5.23 | ROMEROROQUE (48), FAJARDOYACEVEDO (16), GARCIAMARCOS (3), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| medium | `Elprimerrefugiodelhombre` | MELO | 66 | 45/66 (68%) | 5.23 | MELO (45), CAXESI (2), GARCIADEPRADO (2), BANCESCANDAMO (1), PAREDES (1) |
| medium | `CalderonAtribuido_ConsumodelvellonEl` | VIDALYSALVADOR | 464 | 238/464 (51%) | 5.18 | VIDALYSALVADOR (238), CASTILLOSOLORZANO (75), LANINI (41), PAREDES (30), CECILIANACIMIENTO (26) |
| medium | `DiegodeAguayoyTerones_GrancapitanEl` | LEIVARAMIREZ | 67 | 45/67 (67%) | 5.18 | LEIVARAMIREZ (45), BATRES (9), ENRIQUEZ (2), GONZALEZDEBARCIA (1), CASTILLOSOLORZANO (1) |
| medium | `MALO_AmistadVenceAlRigor3` | FAJARDOYACEVEDO | 70 | 51/70 (73%) | 5.17 | FAJARDOYACEVEDO (51), LEIVARAMIREZ (8), GARCIAMARCOS (2), CALLE (1) |
| medium | `AntonioMartinezdeMeneses_MejoralcaldeelreyyNohaycuentac` | BELMONTE | 61 | 35/61 (57%) | 5.16 | BELMONTE (35), ROJASZORRILLA (16), LOPEZDECASTRO (2), SANDOVAL (2), LOPEZJACINTO (1) |
| medium | `ZAMORA_MisticaMonarquia` | MELO | 72 | 65/72 (90%) | 5.12 | MELO (65), CASTROYSALAZAR (1) |
| medium | `Papelesvariosgongorinos_6` | SARAVIAYMENDOZA | 100 | 88/100 (88%) | 5.10 | SARAVIAYMENDOZA (88), VARGAS (5), GARCIAMARCOS (1), MONTALBAN (1), RUIZALCEO (1) |
| medium | `CastroyBellvisGuillende_Quiennoseaventura` | CLARAMONTE | 66 | 34/66 (52%) | 5.10 | CLARAMONTE (34), GALLEGOS (7), MENESES (7), VELEZ (2), LEIVARAMIREZ (2) |
| medium | `Laperfectacasada` | BATRES | 65 | 45/65 (69%) | 5.06 | BATRES (45), BELMONTE (3), LEIVARAMIREZ (2), GARCIADEPRADO (2), CERVANTES (1) |
| medium | `MONTERO_AmarSinFavorecer` | MOLINAYMENDOZA | 91 | 57/91 (63%) | 5.05 | MOLINAYMENDOZA (57), FAJARDOYACEVEDO (9), JIMENEZSEDENO (8), LEIVARAMIREZ (5), HURTADODEMENDOZA (1) |
| medium | `JuanBautistaDiamanteMatosFrago_CortesanaenlasierraLa` | CALLE | 63 | 36/63 (57%) | 5.04 | CALLE (36), JIMENEZSEDENO (9), FAJARDOYACEVEDO (8), MOLINAYMENDOZA (2), GARCIAMARCOS (1) |
| medium | `MatosFragosoJuande_Mudablearrepentidoyelingratoag` | ALARCON | 61 | 32/61 (52%) | 5.03 | ALARCON (32), BOLEAYALVARADO (8), MATOSFRAGOSO (5), ANDOSILLA (2), HURTADODEMENDOZA (1) |
| medium | `VidalySalvadorManuel_Disimularesvencer` | ROMEROROQUE | 47 | 31/47 (66%) | 5.02 | ROMEROROQUE (31), MOLINAYMENDOZA (5), ALARCON (2), GONZALEZDEBARCIA (1), FAJARDOYACEVEDO (1) |
| medium | `QUINONESDEBENAVENTE_Honradas` | QUINONES | 14 | 7/14 (50%) | 4.99 | QUINONES (7), VALDIVIELSO (3), CASTILLOSOLORZANO (1), ROJASZORRILLA (1) |
| medium | `ArboredaAlejandroatribuido_MartirvalienteenRomaSanJorgeEl` | CORDERO | 62 | 48/62 (77%) | 4.97 | CORDERO (48), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), VARGAS (1), GARCIAMARCOS (1) |
| medium | `ENRIQUEZGOMEZ_SantaTaez` | VIDALYSALVADOR | 116 | 85/116 (73%) | 4.97 | VIDALYSALVADOR (85), VERATASSIS (8), VARGASMACHUCA (2), HURTADODEMENDOZA (2), QUINONES (1) |
| medium | `ElcubodelaAlmudena` | GONZALEZDEBARCIA | 47 | 37/47 (79%) | 4.94 | GONZALEZDEBARCIA (37), ROMEROROQUE (2), PACHECO (1) |
| medium | `AntoniodeZamora_HondadeDavidLa` | VIDALYSALVADOR | 56 | 28/56 (50%) | 4.90 | VIDALYSALVADOR (28), MOLINAYMENDOZA (7), CASTROYSALAZAR (5), CUEVAYSILVA (1), GONZALEZDEBARCIA (1) |
| medium | `PEREZDEBORJA_BandosDeSalamanca` | MORETO | 84 | 52/84 (62%) | 4.86 | MORETO (52), CASTROYSALAZAR (13), CANIZARES (8), ROSETENINO (2), GONGORA (1) |
| medium | `Ladestruccindelostemplarios` | LANINI | 74 | 55/74 (74%) | 4.85 | LANINI (55), LEIVARAMIREZ (5), ENRIQUEZ (2), LEONORCUEVA (2), MENESES (1) |
| medium | `JeronimoVillaizan_Transformacionesdeamor` | BATRES | 61 | 39/61 (64%) | 4.84 | BATRES (39), LEIVARAMIREZ (4), ANDOSILLA (3), SANDOVAL (2), GONZALEZDEBARCIA (1) |
| medium | `ElpastorFido3` | CASTROYSALAZAR | 56 | 32/56 (57%) | 4.83 | CASTROYSALAZAR (32), SANDOVAL (6), GARCIAMARCOS (4), MELO (2), GONZALEZDEBARCIA (1) |
| medium | `MALVEZZI_DeLaGuerraDelPalatinado_Bolonia` | CERVANTES | 261 | 165/261 (63%) | 4.81 | CERVANTES (165), SANDOVAL (43), AVELLANEDA (12), MELO (12), HURTADODEMENDOZA (11) |
| medium | `QUINONESDEBENAVENTE_Jaques` | QUINONES | 12 | 9/12 (75%) | 4.80 | QUINONES (9), HURTADODEMENDOZA (1), MESA (1) |
| medium | `RemonAlonsodeAtribuidoTellezGa_NinfadelcieloAutosacramentalLa` | MESA | 28 | 18/28 (64%) | 4.77 | MESA (18), TAMAYO (2), LORENZANA (1) |
| medium | `DELGADO_ProdigiodePolonia` | LORENZANA | 24 | 14/24 (58%) | 4.77 | LORENZANA (14), PACHECO (6), BARRIONUEVO (2), AVELLANEDA (1), BANCESCANDAMO (1) |
| medium | `ZAMORA_TemplodeDios` | VIDALYSALVADOR | 72 | 56/72 (78%) | 4.77 | VIDALYSALVADOR (56), ENRIQUEZ (7), GARCIADEPRADO (3), VERATASSIS (2) |
| medium | `QUINONESDEBENAVENTE_Sacristanes` | BELMONTE | 18 | 13/18 (72%) | 4.68 | BELMONTE (13), VIDALYSALVADOR (2), ROJASZORRILLA (1), VALDIVIELSO (1) |
| medium | `ClaramonteAndresde_CatolicaprincesaLeopoldaLa` | BATRES | 81 | 51/81 (63%) | 4.67 | BATRES (51), CARVAJAL (3), LEIVARAMIREZ (3), GALLEGOS (3), MULSA (2) |
| medium | `QUINONESDEBENAVENTE_NinaPrimeraParte` | MATOSFRAGOSO | 12 | 8/12 (67%) | 4.67 | MATOSFRAGOSO (8), VIDALYSALVADOR (2), LICENCIADOROJAS (2) |
| medium | `VelezdeGuevaraLuis_JornadadelreydonSebastianenAfr` | CONTRERAS | 59 | 31/59 (52%) | 4.66 | CONTRERAS (31), TORRESLORENZODE (9), LICENCIADOROJAS (2), MESA (2), ENRIQUEZ (2) |
| medium | `FranciscodelaTorreySevil_BatalladelosdosLa` | GARCIADEPRADO | 81 | 44/81 (54%) | 4.61 | GARCIADEPRADO (44), BATRES (13), CALDERON (8), QUINONES (3), CONTRERAS (2) |
| medium | `JuandeZabaleta_HijodeMarcoAurelioEl` | CALDERON | 53 | 33/53 (62%) | 4.51 | CALDERON (33), ROJASZORRILLA (6), ENRIQUEZ (2), ROSETENINO (2), HURTADODEMENDOZA (1) |
| medium | `ZAMORA_LoaparaLacuartaparte` | VIDALYSALVADOR | 68 | 37/68 (54%) | 4.51 | VIDALYSALVADOR (37), GONGORA (16), CASTROYSALAZAR (11), GARCIADEPRADO (2), HURTADODEMENDOZA (1) |
| medium | `MONTESER_Martinete` | DIAMANTE | 14 | 8/14 (57%) | 4.51 | DIAMANTE (8), AMESCUA (1) |
| medium | `Varios_obradramaticapoesias_Palacio` | MEDINA | 23 | 16/23 (70%) | 4.43 | MEDINA (16), LOPEZDECASTRO (6), MESA (1) |
| medium | `SimondeSanmateo_CidEl` | QUEVEDO | 42 | 26/42 (62%) | 4.42 | QUEVEDO (26), CECILIANACIMIENTO (3), BELMONTE (1), ENRIQUEZ (1), VIDALYSALVADOR (1) |
| medium | `MiradeAmescuaAntonio_RuyLopezdeAvalos` | LEIVARAMIREZ | 72 | 40/72 (56%) | 4.41 | LEIVARAMIREZ (40), SANDOVAL (6), TORRESLORENZODE (3), MESA (2), QUINONES (2) |
| medium | `CastroyBellvisGuillende_MocedadesdelCidLas` | MESA | 59 | 31/59 (52%) | 4.37 | MESA (31), CONTRERAS (4), CASTILLOSOLORZANO (3), MORETO (3), ROJASVILLANDRANDO (2) |
| medium | `LeonMerchanteoMarchanteJuanMan_SombrayelsacristanLa` | VIDALYSALVADOR | 20 | 11/20 (55%) | 4.34 | VIDALYSALVADOR (11), BELMONTE (4), VERATASSIS (4), LOPEZDELCAMPO (1) |
| medium | `GodinezManriqueFelipeAtribuido_TorosdelalmaLos` | SANDOVAL | 46 | 23/46 (50%) | 4.31 | SANDOVAL (23), LEIVARAMIREZ (4), BELMONTE (4), JIMENEZSEDENO (2), FAJARDOYACEVEDO (2) |
| medium | `ElReyDonEnriqueIIIllamadoelEnfermo` | VIDALYSALVADOR | 82 | 53/82 (65%) | 4.31 | VIDALYSALVADOR (53), GONZALEZDEBARCIA (10), RUANO (6), MOLINAYMENDOZA (2), ROMEROROQUE (1) |
| medium | `FernandoFriasySantos_Nohayagravioscomocelossisonlos` | TORRESLORENZODE | 56 | 39/56 (70%) | 4.26 | TORRESLORENZODE (39), LANINI (5), SANDOVAL (2), LICENCIADOROJAS (2), BANCESCANDAMO (1) |
| medium | `LopeAtribuida_Sinsecretonohayamor` | CASTROYSALAZAR | 86 | 67/86 (78%) | 4.24 | CASTROYSALAZAR (67), MELO (7), CASTILLOSOLORZANO (2), CONTRERAS (2), REMON (1) |
| medium | `Villarroel_FelipeQuinto` | CASTROYSALAZAR | 66 | 41/66 (62%) | 4.24 | CASTROYSALAZAR (41), LORENZANA (14), MELO (5), HURTADODEMENDOZA (1), PAREDES (1) |
| medium | `FranciscodePaulaGonzalezdeBust_Enelremedioestaeldanoymuertede` | CASTROYSALAZAR | 57 | 33/57 (58%) | 4.22 | CASTROYSALAZAR (33), ROMEROROQUE (9), GONZALEZDETORRES (6), CUENCAYARGUELLO (2), LOPEZDECASTRO (1) |
| medium | `JuanPerezdeMontalban_VenturaenelenganoLa` | MESA | 60 | 35/60 (58%) | 4.18 | MESA (35), MATOSFRAGOSO (7), LICENCIADOROJAS (4), ROJASZORRILLA (4), GONZALEZDEBARCIA (1) |
| medium | `LOPECALDERON_EspanoladeFlorencia` | JIMENEZSEDENO | 87 | 57/87 (66%) | 4.18 | JIMENEZSEDENO (57), GILENRIQUEZ (17), MOLINAYMENDOZA (6), VIDALYSALVADOR (3), AVELLANEDADELACUEVA (2) |
| medium | `FranciscoJacintodeFunesyVillal_MartirantesdenacerSanMamesEl` | VIDALYSALVADOR | 60 | 36/60 (60%) | 4.17 | VIDALYSALVADOR (36), CANIZARES (8), CASTROYSALAZAR (3), MORETO (2), SANTATERESA (1) |
| medium | `AntonioFolchdeCardonaAlagon_LomejoreslomejorFiestaprecedid` | MOLINAYMENDOZA | 73 | 39/73 (53%) | 4.10 | MOLINAYMENDOZA (39), GARCIADEPRADO (14), CANIZARES (4), CALLE (3), CALDERON (2) |
| medium | `VegaCarpioLopedeAtribuido_PleitoporlahonraoElvalordeFern` | LEIVARAMIREZ | 62 | 35/62 (56%) | 4.03 | LEIVARAMIREZ (35), TORRESLORENZODE (3), MULSA (2), JUANDESOTO (2), GONZALEZDEBARCIA (1) |
| medium | `FranciscodeVitoria_Obligarconelagravio` | AVELLANEDA | 80 | 49/80 (61%) | 4.00 | AVELLANEDA (49), MESA (20), LICENCIADOROJAS (2), VIDALYSALVADOR (1) |
| medium | `LOA_SantisimoSacramentoBNE` | SANDOVAL | 10 | 7/10 (70%) | 3.98 | SANDOVAL (7), LICENCIADOROJAS (1), MEDINA (1) |
| medium | `CARTA_CatharinaGoncalves` | VIDALYSALVADOR | 2 | 2/2 (100%) | 3.96 | VIDALYSALVADOR (2) |
| medium | `LosmartiresdeMadridydejarunreinoporotro3` | GARCIADEPRADO | 60 | 35/60 (58%) | 3.96 | GARCIADEPRADO (35), BATRES (7), CARVAJAL (2), QUINONES (2), ANDOSILLA (2) |
| medium | `FranciscoAntoniodeBancesCandam_Duelosdeingenioyfortuna` | MOLINAYMENDOZA | 81 | 46/81 (57%) | 3.92 | MOLINAYMENDOZA (46), VIDALYSALVADOR (11), LLOBREGATYESTEVE (6), GARCIAMARCOS (2), SANDOVAL (2) |
| medium | `ElprincipedonCarlos2` | CORDERO | 70 | 48/70 (69%) | 3.91 | CORDERO (48), ENRIQUEZ (11), VARGASMACHUCA (1), AVELLANEDA (1), GARCIADEPRADO (1) |
| medium | `VegaCarpioLopede_TrabajosdeJacobSuenoshayquever` | VILLEGASJUANBAUTISTA | 61 | 34/61 (56%) | 3.89 | VILLEGASJUANBAUTISTA (34), CALDERON (10), SARAVIAYMENDOZA (3), PAREDES (1), SANTATERESA (1) |
| medium | `PEREZDEMONTALBAN_Lostemplarios` | SANDOVAL | 65 | 50/65 (77%) | 3.89 | SANDOVAL (50), MELO (7), SANTATERESA (1), GONGORA (1), BENAVIDES (1) |
| medium | `CanizaresySuarezdeToledoJosede_UnprecipicioconotroCalipsoyTel` | SANDOVAL | 56 | 34/56 (61%) | 3.81 | SANDOVAL (34), LANINI (5), MOLINAYMENDOZA (2), GILENRIQUEZ (2), CERVANTES (1) |
| medium | `GODINEZ_Romance` | VERATASSIS | 3 | 3/3 (100%) | 3.79 | VERATASSIS (3) |
| medium | `AntonioEnriquezGomez_Enganarparareinar` | LANINI | 74 | 38/74 (51%) | 3.79 | LANINI (38), PAREDES (11), ROSETENINO (7), JIMENEZSEDENO (6), GARCIAMARCOS (3) |
| medium | `GaspardePuigaltyLluqui_Peligrodelasangreyremedioenela` | VIDALYSALVADOR | 66 | 33/66 (50%) | 3.75 | VIDALYSALVADOR (33), MARCHANTE (12), LOPEZDELCAMPO (5), GONZALEZDEBARCIA (2), LEONORCUEVA (2) |
| medium | `JuandeGrajalesAtribuidoVegaCar_ReyporsemejanzaEl` | CASTILLOSOLORZANO | 57 | 38/57 (67%) | 3.75 | CASTILLOSOLORZANO (38), ALARCON (6), ENRIQUEZ (3), GARCIADEPRADO (2), JIMENEZSEDENO (1) |
| medium | `POLOPYVALDES_HidalgoteDeJaca` | SANDOVAL | 111 | 72/111 (65%) | 3.74 | SANDOVAL (72), GILENRIQUEZ (20), MEDINA (5), DAVILAYPALOMARES (5), LANINI (4) |
| medium | `SERONSPINOSSA_Garcilasoenamorado` | MEDINA | 102 | 52/102 (51%) | 3.73 | MEDINA (52), VERATASSIS (13), GILENRIQUEZ (11), VARGAS (8), LANINI (5) |
| medium | `CristobaldeMonroyySilva_MayorvasallodelmayorsenorElgig` | VIDALYSALVADOR | 48 | 30/48 (62%) | 3.68 | VIDALYSALVADOR (30), BELMONTE (4), LOPEZDELCAMPO (3), ROSETENINO (1), CALDERON (1) |
| medium | `ErasoyArteagaFranciscode_Delagraviohacervenganzaohablar` | PAREDES | 79 | 41/79 (52%) | 3.67 | PAREDES (41), VIDALYSALVADOR (16), SANDOVAL (10), LORENZANA (1), GONZALEZDEBARCIA (1) |
| medium | `LarenegadadeValladolid` | GARCIAMARCOS | 69 | 54/69 (78%) | 3.67 | GARCIAMARCOS (54), PAREDES (2), LEIVARAMIREZ (1), ROMEROROQUE (1), FAJARDOYACEVEDO (1) |
| medium | `HURTADO_Quererporsoloquerer_acto2` | SARAVIAYMENDOZA | 67 | 44/67 (66%) | 3.63 | SARAVIAYMENDOZA (44), GARCIADEPRADO (12), CALLE (8), GILENRIQUEZ (2), ROSETENINO (1) |
| medium | `JuanBautistaDiamanteAtribuidoM_CapitanJepteoCumplirleaDioslap` | CASTILLOSOLORZANO | 62 | 42/62 (68%) | 3.59 | CASTILLOSOLORZANO (42), ALARCON (4), GONZALEZDEBARCIA (3), GARCIADEPRADO (2), PACHECO (1) |
| medium | `PabloPolopyValdesAtribuidoPedr_SitioysocorrodeVienaporelgranv` | GARCIADEPRADO | 62 | 31/62 (50%) | 3.56 | GARCIADEPRADO (31), ALARCON (9), MORETO (6), ROSETENINO (5), LEIVARAMIREZ (2) |
| medium | `MONTORO_NoHayConAmorCompetencias` | AVELLANEDA | 86 | 56/86 (65%) | 3.53 | AVELLANEDA (56), GONZALEZDETORRES (10), MELO (8), CASTROYSALAZAR (4), SARAVIAYMENDOZA (3) |
| medium | `ROSETE_HistoriaDelSeyano_1` | VIDALYSALVADOR | 81 | 61/81 (75%) | 3.53 | VIDALYSALVADOR (61), GILENRIQUEZ (6), VERATASSIS (3), MARCHANTE (2), BANCESCANDAMO (1) |
| medium | `DiegodeVillanuevayNunezJosedeL_Principedeldesiertoyermitanode` | ROMEROROQUE | 96 | 54/96 (56%) | 3.52 | ROMEROROQUE (54), FAJARDOYACEVEDO (15), PAREDES (6), ALARCON (4), LANINI (2) |
| medium | `JuanGonzalezdeVillacastin_MonstruodelasierraypastorAngel` | SANDOVAL | 65 | 37/65 (57%) | 3.51 | SANDOVAL (37), PAREDES (8), BELMONTE (6), MOLINAYMENDOZA (2), LICENCIADOROJAS (1) |
| medium | `GaspardeAvila_Fingirporconservarlabocaynoelc` | QUEVEDO | 50 | 25/50 (50%) | 3.51 | QUEVEDO (25), LOPE (9), BELMONTE (4), LICENCIADOROJAS (1), CAXESI (1) |
| medium | `AVILA_ComediadeSantaCaterina` | AVELLANEDA | 93 | 66/93 (71%) | 3.50 | AVELLANEDA (66), CECILIANACIMIENTO (24), CUEVAYSILVA (2), GOMEZACOSTA (1) |
| medium | `ENRIQUEZGOMEZ_Grancardenaldongilprimeraparte` | CERVANTES | 62 | 60/62 (97%) | 3.50 | CERVANTES (60), GONGORA (2) |
| medium | `RodrigodeHerrerayRibera_PrimertemplodeEspanaySanSegund` | COELLO | 111 | 66/111 (60%) | 3.49 | COELLO (66), TIRSO (16), CONTRERAS (9), BATRES (3), MESA (2) |
| medium | `MIRADEAMESCUA_DesgraciadaRaquelLa` | VIDALYSALVADOR | 60 | 48/60 (80%) | 3.49 | VIDALYSALVADOR (48), AVELLANEDA (3), CASTROYSALAZAR (2), LOPEZDELCAMPO (2), CASTILLOSOLORZANO (1) |
| medium | `CAIRASCOFIGUEROA_TragediaSantaSusana` | BENAVIDES | 42 | 33/42 (79%) | 3.46 | BENAVIDES (33), SANDOVAL (6), AVELLANEDA (3) |
| medium | `LagaleotadelcondedeNiebla` | MELO | 88 | 47/88 (53%) | 3.44 | MELO (47), GARCIAMARCOS (20), ROMEROROQUE (4), GONZALEZDEBARCIA (2), CASTROYSALAZAR (2) |
| medium | `SOUSA_GalanTerceroMarido` | HURTADODEMENDOZA | 23 | 19/23 (83%) | 3.43 | HURTADODEMENDOZA (19), GARCIADEPRADO (1), VELEZ (1), GONGORA (1), MONTALBAN (1) |
| medium | `ClaramonteAndresde_PacienciaenlafortunaLa` | CLARAMONTE | 67 | 37/67 (55%) | 3.42 | CLARAMONTE (37), AGUADOELVIEJO (10), GALLEGOS (3), JUANDESOTO (1), CARVAJAL (1) |
| medium | `CALDERONoVALDIVIESO_CruzDondeMurioCristo_British` | GILENRIQUEZ | 31 | 18/31 (58%) | 3.40 | GILENRIQUEZ (18), QUEVEDO (5), GARCIADEPRADO (2), HURTADODEMENDOZA (1), MEDINA (1) |
| medium | `PERALTA_TriunfosDeAmorYPoder_British` | CASTROYSALAZAR | 112 | 76/112 (68%) | 3.38 | CASTROYSALAZAR (76), SANDOVAL (28), DAVILAYPALOMARES (2), MELO (2), AVELLANEDA (1) |
| medium | `JuanBautistaDiamante_ValornotieneedadSansondeExtrem` | PAREDES | 90 | 51/90 (57%) | 3.38 | PAREDES (51), GARCIAMARCOS (24), MELO (3), VIDALYSALVADOR (1), JIMENEZSEDENO (1) |
| medium | `CastroyBellvisGuillendeMiradeA_ManzanadeladiscordiayrobodeEle` | FAJARDOYACEVEDO | 90 | 48/90 (53%) | 3.36 | FAJARDOYACEVEDO (48), QUINONES (14), SANDOVAL (9), LEIVARAMIREZ (2), CARVAJAL (1) |
| medium | `VegaCarpioLopede_TorneosdeCristoconelamordivino` | BELMONTE | 30 | 19/30 (63%) | 3.34 | BELMONTE (19), BATRES (6), LEIVARAMIREZ (3), ALARCON (1), GARCIAMARCOS (1) |
| medium | `MiradeAmescuaAntonio_HeroyLeandro` | CALDERON | 58 | 33/58 (57%) | 3.34 | CALDERON (33), LEIVARAMIREZ (5), ALARCON (4), ROSETENINO (2), BELMONTE (2) |
| medium | `CalderonAntonioCoelloyOchoaAnt_PastorFidoEl` | VIDALYSALVADOR | 87 | 45/87 (52%) | 3.33 | VIDALYSALVADOR (45), PAREDES (16), CECILIANACIMIENTO (9), MELO (6), CASTROYSALAZAR (4) |
| medium | `AntoniodeZamora_TemplovivodeDiosEl` | GARCIADEPRADO | 39 | 29/39 (74%) | 3.31 | GARCIADEPRADO (29), VIDALYSALVADOR (2), CERVANTES (1), ENRIQUEZ (1), CASTILLOSOLORZANO (1) |
| medium | `CastroyBellvisGuillende_CaballeroperfectoEl` | QUEVEDO | 54 | 39/54 (72%) | 3.30 | QUEVEDO (39), GALLEGOS (4), GONZALEZDEBARCIA (2), CERVANTES (1), GARCIADEPRADO (1) |
| medium | `ENRIQUEZGOMEZ_MayorProdigioDeLasMisas` | QUEVEDO | 112 | 57/112 (51%) | 3.29 | QUEVEDO (57), ENRIQUEZ (30), LEIVARAMIREZ (6), BELMONTE (6), CASTILLOSOLORZANO (3) |
| medium | `Lahonraporlamujer1a45` | MIRACLESSOTOMAYOR | 45 | 25/45 (56%) | 3.25 | MIRACLESSOTOMAYOR (25), CLARAMONTE (6), LICENCIADOROJAS (1), CARVAJAL (1), GONZALEZDEBARCIA (1) |
| medium | `NICODEMUS_LoaentremesadaparaNavidad` | GILENRIQUEZ | 16 | 13/16 (81%) | 3.20 | GILENRIQUEZ (13), VERATASSIS (2), VIDALYSALVADOR (1) |
| medium | `GARCIA_RayoDelCieloYLimpiaConcepcion` | LEIVARAMIREZ | 87 | 53/87 (61%) | 3.18 | LEIVARAMIREZ (53), BELMONTE (26), QUINONES (2), CUEVAYSILVA (1), REMON (1) |
| medium | `MiradeAmescuaAntonio_ReinaSevillaycarbonerosdeFranc` | CALLE | 66 | 39/66 (59%) | 3.17 | CALLE (39), FAJARDOYACEVEDO (15), JIMENEZSEDENO (2), CASTILLOSOLORZANO (1), LOPEZJACINTO (1) |
| medium | `Lafuerzadelacostumbre` | MESA | 119 | 70/119 (59%) | 3.15 | MESA (70), QUINONES (12), CUEVAYSILVA (7), LICENCIADOROJAS (2), BATRES (2) |
| medium | `MARTINEZDEMENESES_JusticiaAlCulpado` | VERATASSIS | 106 | 74/106 (70%) | 3.11 | VERATASSIS (74), SANDOVAL (23), GILENRIQUEZ (5), VIDALYSALVADOR (1), CANIZARES (1) |
| medium | `VelezdeGuevaraLuis_MesaredondayEldivinoCarlomagno` | ROMEROROQUE | 40 | 20/40 (50%) | 3.11 | ROMEROROQUE (20), FAJARDOYACEVEDO (5), GARCIAMARCOS (2), PAREDES (2), BELMONTE (1) |
| medium | `RojasZorrillaFranciscode_Nohayamigoparaamigo` | ROMEROROQUE | 56 | 36/56 (64%) | 3.09 | ROMEROROQUE (36), MEDINA (9), TORRESLORENZODE (2), SANDOVAL (2), LORENZANA (1) |
| medium | `JeronimoVillaizanAtribuido_Agrandanogranremedio` | SARAVIAYMENDOZA | 558 | 377/558 (68%) | 3.06 | SARAVIAYMENDOZA (377), CASTILLOSOLORZANO (44), GARCIAMARCOS (37), ROMEROROQUE (23), GONZALEZDEBARCIA (20) |
| medium | `FUNESYVILLALPANDO_MartirDeOrienteSanMames` | VIDALYSALVADOR | 240 | 208/240 (87%) | 3.06 | VIDALYSALVADOR (208), VARGASMACHUCA (17), GONGORA (2), ENRIQUEZ (2) |
| medium | `JoseFlores_LoaalaConcepcion` | CASTILLOSOLORZANO | 232 | 149/232 (64%) | 3.03 | CASTILLOSOLORZANO (149), ENRIQUEZ (36), AVELLANEDA (19), LANINI (3), LICENCIADOROJAS (3) |
| low | `LaniniySagredoPedroFranciscode_LoaparalafiestadeNuestraSenora` | LANINI | 17 | 7/17 (41%) | 51.16 | LANINI (7) |
| low | `AvellanedadelaCuevayGuerraFran_HijadeldoctorLa` | AVELLANEDADELACUEVA | 15 | 6/15 (40%) | 48.41 | AVELLANEDADELACUEVA (6), CERVANTES (1) |
| low | `JuanBautistadeVillegas_DespreciadaqueridaLa` | VILLEGASJUANBAUTISTA | 51 | 25/51 (49%) | 46.91 | VILLEGASJUANBAUTISTA (25), CERVANTES (1), SARAVIAYMENDOZA (1), VARGASMACHUCA (1) |
| low | `CanizaresySuarezdeToledoJosede_SayodeBenitoEl` | CANIZARES | 15 | 6/15 (40%) | 41.79 | CANIZARES (6) |
| low | `CastroySalazarFranciscoAntonio_VejeteenamoradoEl` | CASTROYSALAZAR | 14 | 6/14 (43%) | 41.76 | CASTROYSALAZAR (6), LICENCIADOROJAS (1) |
| low | `SalazaryTorresDiegode_SacristanahorcadoEl` | SALAZARYTORRES | 17 | 8/17 (47%) | 38.61 | SALAZARYTORRES (8), ROMEROROQUE (1), CASTILLOSOLORZANO (1) |
| low | `SimonAguadoelViejo_NegrosLos` | AGUADOELVIEJO | 17 | 7/17 (41%) | 37.22 | AGUADOELVIEJO (7), CERVANTES (1), QUINONES (1) |
| low | `MulsaMiguelde_VerdadesdeZonzoLas` | MULSA | 27 | 6/27 (22%) | 36.96 | MULSA (6), VARGAS (1) |
| low | `LeonMerchanteJuanManuelde_VisitadelospresosLa` | MARCHANTE | 31 | 10/31 (32%) | 35.26 | MARCHANTE (10), VIDALYSALVADOR (2), CASTILLOSOLORZANO (1) |
| low | `LaniniySagredoPedroFranciscode_PerladeCatalunaypenasdeMontser` | LANINI | 68 | 32/68 (47%) | 33.84 | LANINI (32), MOLINAYMENDOZA (13), CANIZARES (10), CERVANTES (1), GARCIAMARCOS (1) |
| low | `PedroFranciscodeLaniniySagredo_PlumaLa` | LANINI | 16 | 5/16 (31%) | 33.38 | LANINI (5), PAREDES (1) |
| low | `LeonMarchanteManuelde_MotesLos` | MARCHANTE | 35 | 11/35 (31%) | 32.22 | MARCHANTE (11), VIDALYSALVADOR (4), MORETO (1) |
| low | `CanizaresySuarezdeToledoJosede_PelucasEntremesLas` | CASTROYSALAZAR | 17 | 7/17 (41%) | 32.12 | CASTROYSALAZAR (7), JIMENEZSEDENO (1) |
| low | `FranciscoAntoniodeCastroySalaz_SacaLa` | MOLINAYMENDOZA | 18 | 8/18 (44%) | 30.47 | MOLINAYMENDOZA (8), QUINONES (1) |
| low | `Entrebobosandaeljuegosainete_Autografo` | FBQUIROS | 27 | 8/27 (30%) | 30.14 | FBQUIROS (8), GONZALEZDETORRES (1), REMON (1) |
| low | `QuirosFranciscoBernardode_CallesdeMadridLas` | FBQUIROS | 27 | 8/27 (30%) | 29.90 | FBQUIROS (8), VALDIVIELSO (1), HURTADODEMENDOZA (1), DIAMANTE (1) |
| low | `SimonAguadoelViejo_PlatilloEl` | AGUADOELVIEJO | 37 | 15/37 (40%) | 28.66 | AGUADOELVIEJO (15), CASTILLOSOLORZANO (1), SAAVEDRAFAJARDO (1), AVELLANEDA (1) |
| low | `TellezGabrielAtribuidoClaramon_MariHernandezlagallega` | MORETO | 25 | 11/25 (44%) | 28.24 | MORETO (11), LANINI (5), HURTADODEMENDOZA (1), LOPEZJACINTO (1) |
| low | `CartaSANTATERESA_IsabelOsorio` | CERVANTES | 3 | 1/3 (33%) | 26.68 | CERVANTES (1), SANTATERESA (1), PAREDES (1) |
| low | `QuinonesdeBenaventeLuisAtribui_Pandurico` | MOLINAYMENDOZA | 17 | 7/17 (41%) | 22.75 | MOLINAYMENDOZA (7) |
| low | `AvellanedadelaCuevayGuerraFran_InfiernoElEntremesdeJuanRana` | AVELLANEDADELACUEVA | 35 | 14/35 (40%) | 22.54 | AVELLANEDADELACUEVA (14), GODINEZMANRIQUE (1), GONGORA (1), MIRACLESSOTOMAYOR (1) |
| low | `VegaCarpioLopede_NinezdelpadreRojasPrimeraparte` | LORENZANA | 26 | 12/26 (46%) | 21.57 | LORENZANA (12), PACHECO (6), BELMONTE (1), CANIZARES (1) |
| low | `LaniniySagredoPedroFranciscode_DiadelcorpusenMadrid` | LANINI | 15 | 6/15 (40%) | 21.16 | LANINI (6), CERVANTES (1) |
| low | `VegaCarpioLopedeAtribuido_EsclavofingidoEl` | ROJASVILLANDRANDO | 27 | 11/27 (41%) | 20.31 | ROJASVILLANDRANDO (11), JUANDESOTO (4), BELMONTE (3), CASTROYSALAZAR (1), VERATASSIS (1) |
| low | `INES_GUEVARA_AmorEsMasLaberinto` | MELO | 42 | 20/42 (48%) | 20.14 | MELO (20), CANIZARES (7), CASTROYSALAZAR (4), CARVAJAL (1), LANINI (1) |
| low | `JUANAINES_AmorLaberinto` | MELO | 42 | 20/42 (48%) | 20.14 | MELO (20), CANIZARES (7), CASTROYSALAZAR (4), CARVAJAL (1), LANINI (1) |
| low | `AvellanedadelaCuevayGuerraFran_Eltiteretier` | AVELLANEDADELACUEVA | 31 | 11/31 (36%) | 19.48 | AVELLANEDADELACUEVA (11), QUINONES (1) |
| low | `MoretoyCavanaAgustinJeronimode_PapeldeJulioenLafuerzadelnatur` | MESA | 55 | 10/55 (18%) | 18.38 | MESA (10), RUIZALCEO (6), CASTROYSALAZAR (6), QUINONES (4), VIDALYSALVADOR (4) |
| low | `ZAMORA_AspidesHayBasiliscos` | CANIZARES | 44 | 19/44 (43%) | 17.31 | CANIZARES (19), MOLINAYMENDOZA (13), LICENCIADOROJAS (1), CERVANTES (1), CASTROYSALAZAR (1) |
| low | `PedroCalderondelaBarcaAtribuid_LenguasLasEntremesparaelautode` | FAJARDOYACEVEDO | 16 | 5/16 (31%) | 17.06 | FAJARDOYACEVEDO (5), LICENCIADOROJAS (1) |
| low | `CORREAS_ArteLengua` | BARRIONUEVO | 35 | 17/35 (49%) | 16.86 | BARRIONUEVO (17), DAVILAYPALOMARES (12), LICENCIADOROJAS (6) |
| low | `CanizaresySuarezdeToledoJosede_TalegoencantadoEl` | CANIZARES | 18 | 8/18 (44%) | 16.83 | CANIZARES (8), GONZALEZDEBARCIA (1) |
| low | `AyalaAlonsode_ParatodoEntremesymojigangaEl` | CASTROYSALAZAR | 18 | 8/18 (44%) | 16.23 | CASTROYSALAZAR (8), CASTILLOSOLORZANO (1), SANDOVAL (1) |
| low | `HozyMotaJuanClaudiodela_RondadelentremesLa` | HOZYMOTA | 20 | 6/20 (30%) | 15.57 | HOZYMOTA (6), CASTILLOSOLORZANO (1), LORENZANA (1), LANINI (1), TORRESLORENZODE (1) |
| low | `Tresingeniossinespecificar_MujerdePeribanezLa` | LANINI | 30 | 13/30 (43%) | 15.54 | LANINI (13), MORETO (7), BARRIONUEVO (2), LEONORCUEVA (1), LORENZANA (1) |
| low | `FranciscodelaCalleAtribuidoJua_Poderyamorcompitiendo` | MORETO | 25 | 9/25 (36%) | 15.30 | MORETO (9), CANIZARES (7), PSEUDOHURTADODEMENDOZA (2), MIRACLESSOTOMAYOR (1), HURTADODEMENDOZA (1) |
| low | `LaniniySagredoPedroFranciscode_Nuevoespejoenlacorteyignoradap` | COELLO | 88 | 37/88 (42%) | 14.67 | COELLO (37), LANINI (19), TAMAYO (17), LICENCIADOROJAS (3), GONZALEZDEBARCIA (1) |
| low | `TellodeMenesesAntonio_Hallarvidadandomuerteyenladesg` | ROMEROROQUE | 36 | 14/36 (39%) | 14.46 | ROMEROROQUE (14), GONZALEZDEBARCIA (5), CAXESI (5), BANCESCANDAMO (2), GARCIADEPRADO (1) |
| low | `VegaCarpioLopede_HechosdeGarcilasodelaVegayMoro` | SANDOVAL | 19 | 9/19 (47%) | 14.00 | SANDOVAL (9), TORRESLORENZODE (5), CARVAJAL (2), QUEVEDO (1) |
| low | `CodiceFacticio-II-460` | TORRESLORENZODE | 426 | 147/426 (34%) | 13.89 | TORRESLORENZODE (147), GOMEZACOSTA (61), BELMONTE (44), ROSETENINO (34), LEIVARAMIREZ (26) |
| low | `VegaCarpioLopede_SantiagoelVerde` | CONTRERAS | 39 | 11/39 (28%) | 13.75 | CONTRERAS (11), ENRIQUEZ (10), BARRIONUEVO (3), LOPEZDECARDENA (3), LICENCIADOROJAS (1) |
| low | `BaltasardeFunesyVillalpandoAtr_BuenmaridoEl` | BARRIONUEVO | 400 | 198/400 (50%) | 13.72 | BARRIONUEVO (198), VIDALYSALVADOR (81), ONAVIEDMAYTORRES (36), LOPEZDELCAMPO (15), CECILIANACIMIENTO (11) |
| low | `LaniniySagredoPedroFranciscode_TontillosLos` | LANINI | 13 | 5/13 (38%) | 13.44 | LANINI (5), QUINONES (1) |
| low | `VegaCarpioLopede_OcasionperdidaLa` | ROJASZORRILLA | 61 | 24/61 (39%) | 13.26 | ROJASZORRILLA (24), TORRESLORENZODE (11), BELMONTE (9), ENRIQUEZ (5), GILENRIQUEZ (2) |
| low | `RojasZorrillaFranciscode_NuestraSenoradeAtochaySegundoJ` | LANINI | 37 | 14/37 (38%) | 13.15 | LANINI (14), GILENRIQUEZ (4), CASTROYSALAZAR (3), CANIZARES (2), TORRESLORENZODE (2) |
| low | `MONTESER_Hidalga` | MOLINAYMENDOZA | 10 | 4/10 (40%) | 12.99 | MOLINAYMENDOZA (4), LLOBREGATYESTEVE (1), FAJARDOYACEVEDO (1) |
| low | `PedroFranciscodeLaniniySagredo_PlazadeMadridEntremesLa` | LANINI | 11 | 3/11 (27%) | 12.97 | LANINI (3) |
| low | `AgustindeSalazaryTorres_MolineroEl` | MOLINAYMENDOZA | 9 | 3/9 (33%) | 12.94 | MOLINAYMENDOZA (3), ROMEROROQUE (1), VIDALYSALVADOR (1), CASTILLOSOLORZANO (1) |
| low | `GarciaBacadeMontalvo_VisitagravosaLa` | LOPEZJACINTO | 14 | 6/14 (43%) | 12.13 | LOPEZJACINTO (6) |
| low | `CartaSANTATERESA_BNP` | SANTATERESA | 6 | 2/6 (33%) | 12.10 | SANTATERESA (2) |
| low | `JeronimodeCancer_PortuguesEl` | GONZALEZDEBARCIA | 15 | 4/15 (27%) | 11.90 | GONZALEZDEBARCIA (4), RUANO (1) |
| low | `VeraTassisyVillarroelDiegoJuan_OidoylavistaEl` | LORENZANA | 27 | 5/27 (18%) | 11.65 | LORENZANA (5), VERATASSIS (5), CARVAJAL (2), LICENCIADOROJAS (1), VIDALYSALVADOR (1) |
| low | `LaniniySagredoPedroFranciscode_TarascaLa` | LANINI | 16 | 5/16 (31%) | 11.10 | LANINI (5), AMESCUA (1), ROMEROROQUE (1) |
| low | `GarciadePradoJoseAntonio_ConquistadeValenciayninecesdes` | GARCIADEPRADO | 70 | 31/70 (44%) | 10.88 | GARCIADEPRADO (31), MOLINAYMENDOZA (24), CAXESI (1), HOZYMOTA (1), GONZALEZDEBARCIA (1) |
| low | `LEON_ALasBodasDeLosExcelentisimosSenores_Autografo` | MARCHANTE | 27 | 8/27 (30%) | 10.77 | MARCHANTE (8), LICENCIADOROJAS (2), REMON (2), CARVAJAL (2), BANCESCANDAMO (2) |
| low | `SanBernardoabad` | ANDOSILLA | 76 | 29/76 (38%) | 10.75 | ANDOSILLA (29), SANDOVAL (22), MOLINAYMENDOZA (7), GONZALEZDEBARCIA (1), BELMONTE (1) |
| low | `CastroyBellvisGuillende_MejoresposoSanJoseEl` | CLARAMONTE | 67 | 21/67 (31%) | 10.73 | CLARAMONTE (21), BELMONTE (8), LEIVARAMIREZ (6), FAJARDOYACEVEDO (5), MOLINAYMENDOZA (4) |
| low | `MatosFragosoJuande_MudosLos` | LEIVARAMIREZ | 13 | 5/13 (38%) | 10.65 | LEIVARAMIREZ (5) |
| low | `VegaCarpioLopede_Quienamanohagafieros` | TORRESLORENZODE | 63 | 26/63 (41%) | 10.53 | TORRESLORENZODE (26), CASTILLOSOLORZANO (5), BATRES (5), GONZALEZDEBARCIA (1), CERVANTES (1) |
| low | `JuanPerezdeMontalban_Deuncastigodosvenganzas` | MORETO | 28 | 10/28 (36%) | 10.50 | MORETO (10), CLARAMONTE (6), ROJASZORRILLA (3), LICENCIADOROJAS (1), HURTADODEMENDOZA (1) |
| low | `GasparAguilar_MercaderamanteEl` | CAXESI | 33 | 14/33 (42%) | 9.88 | CAXESI (14), LOPEZDECASTRO (5), LORENZANA (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `DiegoJimenezdeEnciso_PrimeroduquedeFlorenciaEl` | BELMONTE | 60 | 27/60 (45%) | 9.75 | BELMONTE (27), COELLO (17), QUEVEDO (3), PAREDES (2), CAXESI (2) |
| low | `CastilloSolorzanoAlonsodel_FuegodadodelcieloEl` | GILENRIQUEZ | 19 | 8/19 (42%) | 9.65 | GILENRIQUEZ (8), PSEUDOHURTADODEMENDOZA (1), LOPE (1), RUIZALCEO (1), TORRESLORENZODE (1) |
| low | `CastroMatiasdeAtribuido_MelonarEl` | QUINONES | 15 | 6/15 (40%) | 9.57 | QUINONES (6) |
| low | `MANZANO_AsombroDeLaSierra` | CUENCAYARGUELLO | 32 | 12/32 (38%) | 9.49 | CUENCAYARGUELLO (12), LOPEZJACINTO (9), GONZALEZDETORRES (2), LANINI (2), CONTRERAS (1) |
| low | `MiradeAmescuaAntonio_SacristanesLos` | CASTROYSALAZAR | 15 | 5/15 (33%) | 9.44 | CASTROYSALAZAR (5), CECILIANACIMIENTO (1), VIDALYSALVADOR (1) |
| low | `LaniniySagredoPedroFranciscode_Tiaysobrina` | LANINI | 17 | 5/17 (29%) | 9.32 | LANINI (5), SANDOVAL (2), QUINONES (1) |
| low | `JuanBautistadeVillegas_ValienteLucidoroRodamontearago` | ROMEROROQUE | 52 | 9/52 (17%) | 9.30 | ROMEROROQUE (9), CASTILLOSOLORZANO (8), DAVILAYPALOMARES (7), TORRESLORENZODE (6), GOMEZACOSTA (3) |
| low | `VegaCarpioLopede_MayorazgodudosoEl` | SANDOVAL | 66 | 19/66 (29%) | 9.19 | SANDOVAL (19), QUINONES (17), ALARCON (7), FAJARDOYACEVEDO (5), VILLEGASDELACRUZ (3) |
| low | `ClaramonteAndresde_Delosmeritosdeamorelsilencioes` | MORETO | 30 | 9/30 (30%) | 9.16 | MORETO (9), CANIZARES (9), GILENRIQUEZ (4), LICENCIADOROJAS (1), CARVAJAL (1) |
| low | `QuinonesdeBenaventeLuis_MalcontentaLa` | LEONORCUEVA | 16 | 7/16 (44%) | 9.11 | LEONORCUEVA (7), LICENCIADOROJAS (1), ROMEROROQUE (1) |
| low | `MiradeAmescuaAntonio_ClavodeJaelEl` | BELMONTE | 42 | 18/42 (43%) | 9.10 | BELMONTE (18), ROJASZORRILLA (15), LEIVARAMIREZ (2), VIDALYSALVADOR (1) |
| low | `FranciscodeVillegasJoseRojo_NinecesdeRoldanLas` | MORETO | 64 | 28/64 (44%) | 9.08 | MORETO (28), LEIVARAMIREZ (12), GILENRIQUEZ (3), ROJASZORRILLA (2), BARREDA (1) |
| low | `AntoniodeZamora_SargentoPalominoEl` | CASTROYSALAZAR | 15 | 5/15 (33%) | 9.02 | CASTROYSALAZAR (5), LICENCIADOROJAS (1), MOLINAYMENDOZA (1) |
| low | `MoretoyCavanaAgustinAtribuido_BandoleradeBaezaypeligrodealab` | VIDALYSALVADOR | 81 | 36/81 (44%) | 8.90 | VIDALYSALVADOR (36), SANDOVAL (32), CECILIANACIMIENTO (1), BANCESCANDAMO (1), AVELLANEDA (1) |
| low | `CorrespondenciaSANTATERESA` | CECILIANACIMIENTO | 544 | 199/544 (37%) | 8.81 | CECILIANACIMIENTO (199), VARGASMACHUCA (67), CASTILLOSOLORZANO (52), BANCESCANDAMO (35), ROMEROROQUE (34) |
| low | `Variosautores_Papelessueltosdevariasobrasdra` | CUEVAYSILVA | 109 | 39/109 (36%) | 8.79 | CUEVAYSILVA (39), MESA (10), RUIZALCEO (8), TAMAYO (8), MEDINA (7) |
| low | `VegaCarpioLopede_DivinopastoroelpastoringratoEl` | ANDOSILLA | 27 | 12/27 (44%) | 8.73 | ANDOSILLA (12), MULSA (5), CLARAMONTE (1), MESA (1), LICENCIADOROJAS (1) |
| low | `LeonMerchanteoMarchanteJuanMan_RefugiodelospoetasEl` | CANIZARES | 15 | 4/15 (27%) | 8.73 | CANIZARES (4), QUINONES (2), LICENCIADOROJAS (1), SARAVIAYMENDOZA (1) |
| low | `GodinezManriqueFelipe_ReinaEsterLa` | CLARAMONTE | 74 | 15/74 (20%) | 8.72 | CLARAMONTE (15), ANDOSILLA (10), TORRESLORENZODE (9), CASTROYSALAZAR (9), ROMEROROQUE (5) |
| low | `FelipeSanchezAtribuido_NuestraSenoradelPilar` | MOLINAYMENDOZA | 19 | 5/19 (26%) | 8.69 | MOLINAYMENDOZA (5), SANDOVAL (3), CASTROYSALAZAR (2), CARVAJAL (1), ROMEROROQUE (1) |
| low | `JuanPerezdeMontalban_TemplariosLos` | ENRIQUEZ | 48 | 14/48 (29%) | 8.67 | ENRIQUEZ (14), VIDALYSALVADOR (14), BELMONTE (10), CORDERO (1) |
| low | `VegaCarpioLopede_MaestrodedanzarEl` | BELMONTE | 30 | 10/30 (33%) | 8.64 | BELMONTE (10), FBQUIROS (7), VERATASSIS (2), BANCESCANDAMO (1), SANDOVAL (1) |
| low | `RodrigodeHerrerayRibera_BatalladeClavijoyvotodeSantiag` | GILENRIQUEZ | 27 | 9/27 (33%) | 8.61 | GILENRIQUEZ (9), TORRESLORENZODE (4), SANDOVAL (2), LICENCIADOROJAS (1), HURTADODEMENDOZA (1) |
| low | `QuinonesdeBenaventeLuis_RabanosLos` | QUINONES | 17 | 6/17 (35%) | 8.61 | QUINONES (6), CERVANTES (1), BELMONTE (1), ANDOSILLA (1) |
| low | `DiegodeFigueroayCordoba_PresumidaLa` | JIMENEZSEDENO | 17 | 3/17 (18%) | 8.58 | JIMENEZSEDENO (3), LEIVARAMIREZ (3), TORRESLORENZODE (1) |
| low | `NicolasdeValleyEstradaAtribuid_BenjamindelaIglesiayMartirSanJ` | CASTROYSALAZAR | 39 | 10/39 (26%) | 8.57 | CASTROYSALAZAR (10), MOLINAYMENDOZA (6), VIDALYSALVADOR (6), LANINI (3), ROMEROROQUE (1) |
| low | `LaniniySagredoPedroFranciscode_DamacomendadorLa` | VERATASSIS | 67 | 33/67 (49%) | 8.45 | VERATASSIS (33), LANINI (9), GILENRIQUEZ (8), SANDOVAL (2), PAREDES (1) |
| low | `ZAMORA_CANIZARES_AngelicaYMedoro_Autografo` | MORETO | 81 | 25/81 (31%) | 8.42 | MORETO (25), LANINI (22), VIDALYSALVADOR (13), LOPEZDELCAMPO (3), CASTROYSALAZAR (3) |
| low | `AntonioHurtadodeMendoza_Quererporsoloquerer` | CASTILLOSOLORZANO | 258 | 55/258 (21%) | 8.39 | CASTILLOSOLORZANO (55), VIDALYSALVADOR (39), PAREDES (26), AVELLANEDA (17), GOMEZACOSTA (9) |
| low | `RomanMonterodeEspinosa_Hayculpaenquenohaydelito` | BOLEAYALVARADO | 38 | 10/38 (26%) | 8.35 | BOLEAYALVARADO (10), LORENZANA (7), GILENRIQUEZ (4), MOLINAYMENDOZA (2), LICENCIADOROJAS (1) |
| low | `FranciscodePaulaGonzalezdeBust_EspanolViriatoEl` | GOMEZACOSTA | 59 | 15/59 (25%) | 8.34 | GOMEZACOSTA (15), VIDALYSALVADOR (13), LANINI (6), GONZALEZDETORRES (3), GONZALEZDEBARCIA (3) |
| low | `Elmontedelapiedad` | ROJASZORRILLA | 29 | 12/29 (41%) | 8.32 | ROJASZORRILLA (12), CAXESI (5), CERVANTES (1), BELMONTE (1), MORETO (1) |
| low | `CASTRO_LoQueSonMujeres` | CASTROYSALAZAR | 13 | 6/13 (46%) | 8.23 | CASTROYSALAZAR (6), SANDOVAL (4), AMESCUA (1) |
| low | `VelezdeGuevaraLuis_ProsperayadversafortunadeJosey` | ROMEROROQUE | 64 | 21/64 (33%) | 8.18 | ROMEROROQUE (21), CLARAMONTE (17), GARCIAMARCOS (13), BARREDA (2), TORRESLORENZODE (2) |
| low | `VegaCarpioLopede_Loaentredosacercadelasmujeres` | AVELLANEDA | 150 | 54/150 (36%) | 8.09 | AVELLANEDA (54), GOMEZACOSTA (36), PAREDES (13), CECILIANACIMIENTO (11), BENAVIDES (8) |
| low | `Ladamaduende` | MESA | 63 | 22/63 (35%) | 8.07 | MESA (22), ANDOSILLA (20), SALAZARYTORRES (5), CLARAMONTE (2), CARVAJAL (1) |
| low | `DiegoCalleja_ComediadelbeatoEstanislaodeKos` | LOPEZJACINTO | 461 | 224/461 (49%) | 8.02 | LOPEZJACINTO (224), BARRIONUEVO (71), LOPEZDELCAMPO (51), CONTRERAS (39), CAXESI (30) |
| low | `VegaCarpioLopedeAtribuido_Nuncamuchocostopoco` | ANDOSILLA | 66 | 29/66 (44%) | 8.01 | ANDOSILLA (29), BELMONTE (20), QUINONES (6), GONZALEZDEBARCIA (1), GARCIAMARCOS (1) |
| low | `AgustindeCastellanos_Mientrasyopodolasvinas` | TORRESLORENZODE | 65 | 32/65 (49%) | 7.98 | TORRESLORENZODE (32), MEDINA (12), SANDOVAL (7), RUIZALCEO (3), CASTILLOSOLORZANO (1) |
| low | `MigueldeLlera_Volverporsumismohonor` | DIAMANTE | 46 | 14/46 (30%) | 7.98 | DIAMANTE (14), LOPEZDELCAMPO (10), LOPEZDECARDENA (4), GONZALEZDEBARCIA (2), CASTROYSALAZAR (2) |
| low | `JuandeCastroSalazar_PutosLos` | MOLINAYMENDOZA | 16 | 4/16 (25%) | 7.95 | MOLINAYMENDOZA (4), CASTILLOSOLORZANO (1), VARGASMACHUCA (1), DIAMANTE (1) |
| low | `RojasZorrillaFranciscode_TraicionbuscaelcastigoLa` | ANDOSILLA | 79 | 27/79 (34%) | 7.81 | ANDOSILLA (27), CLARAMONTE (23), MESA (13), SALAZARYTORRES (3), GONZALEZDEBARCIA (2) |
| low | `RojasZorrillaFranciscodeJeroni_VillanogransenorogranTamerland` | BELMONTE | 61 | 25/61 (41%) | 7.80 | BELMONTE (25), ROJASZORRILLA (18), LEIVARAMIREZ (7), MONTALBAN (3), CECILIANACIMIENTO (1) |
| low | `Loshermanosencontrados` | MORETO | 23 | 8/23 (35%) | 7.79 | MORETO (8), LANINI (2), CANIZARES (1), ROJASZORRILLA (1), GILENRIQUEZ (1) |
| low | `PabloPolopyValdes_PanderaLa` | MELO | 16 | 4/16 (25%) | 7.78 | MELO (4), VIDALYSALVADOR (1), FAJARDOYACEVEDO (1), ROMEROROQUE (1) |
| low | `CanizaresySuarezdeToledoJosede_Honordaentendimientoyelmasbobo` | CASTROYSALAZAR | 50 | 22/50 (44%) | 7.75 | CASTROYSALAZAR (22), LANINI (9), GILENRIQUEZ (5), TORRESLORENZODE (3), SANDOVAL (1) |
| low | `QuirosFranciscoBernardode_MacilentoyastrologofingidoEl` | QUINONES | 14 | 6/14 (43%) | 7.75 | QUINONES (6), LICENCIADOROJAS (1) |
| low | `TellezGabriel_PenadeFranciaLa` | ANDOSILLA | 80 | 39/80 (49%) | 7.74 | ANDOSILLA (39), FAJARDOYACEVEDO (7), LEIVARAMIREZ (7), GALLEGOS (7), BATRES (4) |
| low | `VegaCarpioLopedeAtribuido_CasamientoporCristoEl` | MESA | 56 | 18/56 (32%) | 7.74 | MESA (18), QUINONES (11), GARCIAMARCOS (11), TORRESLORENZODE (2), LICENCIADOROJAS (1) |
| low | `VegaCarpioLopede_NochetoledanaLa` | ROMEROROQUE | 46 | 20/46 (44%) | 7.64 | ROMEROROQUE (20), GOMEZACOSTA (5), FAJARDOYACEVEDO (4), CASTILLOSOLORZANO (2), PACHECO (1) |
| low | `AntonioEnriquezGomez_SantaPelagia` | VIDALYSALVADOR | 553 | 144/553 (26%) | 7.58 | VIDALYSALVADOR (144), VERATASSIS (121), LEIVARAMIREZ (44), MORETO (39), CASTILLOSOLORZANO (33) |
| low | `ClaramonteAndresde_Deunyerronacenmil` | ANDOSILLA | 71 | 33/71 (46%) | 7.55 | ANDOSILLA (33), BELMONTE (21), QUINONES (2), LEIVARAMIREZ (2), CASTILLOSOLORZANO (1) |
| low | `VidalySalvadorManuel_Loasacramentalalegoricaparaela` | VIDALYSALVADOR | 11 | 4/11 (36%) | 7.49 | VIDALYSALVADOR (4), PAREDES (4), LEONORCUEVA (1), LOPEZDELCAMPO (1) |
| low | `MigueldeCervantesSaavederaMigu_TratodeArgel` | BARRIONUEVO | 43 | 13/43 (30%) | 7.48 | BARRIONUEVO (13), GOMEZACOSTA (5), AVELLANEDA (5), ENRIQUEZ (4), CECILIANACIMIENTO (2) |
| low | `MonteserFranciscoAntoniode_HidalgaLa` | MOLINAYMENDOZA | 17 | 5/17 (29%) | 7.48 | MOLINAYMENDOZA (5), LICENCIADOROJAS (2), ROMEROROQUE (2) |
| low | `LosesforciasdeMilan` | GARCIAMARCOS | 63 | 19/63 (30%) | 7.44 | GARCIAMARCOS (19), MENESES (15), MORETO (6), LEIVARAMIREZ (5), ROSETENINO (3) |
| low | `RomanMonterodeEspinosa_Eneldichosoesmeritolaculpa` | CALLE | 99 | 41/99 (41%) | 7.43 | CALLE (41), JIMENEZSEDENO (18), FAJARDOYACEVEDO (9), TORRESLORENZODE (5), LEIVARAMIREZ (4) |
| low | `TURIA_PatrondeValenciaBritish` | MORETO | 38 | 11/38 (29%) | 7.42 | MORETO (11), CANIZARES (9), GILENRIQUEZ (7), LANINI (6), LOPEZDECARDENA (4) |
| low | `ClaramonteAndresde_MayorreydelosreyesEl` | FAJARDOYACEVEDO | 56 | 26/56 (46%) | 7.41 | FAJARDOYACEVEDO (26), QUEVEDO (11), LOPE (3), BELMONTE (3), LEIVARAMIREZ (2) |
| low | `CalderonRojasZorrillaFrancisco_JardindeFalerinaEl` | CASTROYSALAZAR | 55 | 14/55 (26%) | 7.38 | CASTROYSALAZAR (14), MOLINAYMENDOZA (14), GILENRIQUEZ (14), CANIZARES (2), GONZALEZDEBARCIA (1) |
| low | `ArboredaAlejandro_Siamormataamordalavida` | LEIVARAMIREZ | 68 | 32/68 (47%) | 7.38 | LEIVARAMIREZ (32), MOLINAYMENDOZA (20), LOPEZJACINTO (1), HURTADODEMENDOZA (1), LEONORCUEVA (1) |
| low | `Nohaycontraunpadrerazon` | SANDOVAL | 78 | 32/78 (41%) | 7.34 | SANDOVAL (32), GARCIAMARCOS (11), FAJARDOYACEVEDO (10), MESA (8), BELMONTE (6) |
| low | `VILLAROEL_AngelMilagroYMujer` | SANDOVAL | 76 | 31/76 (41%) | 7.28 | SANDOVAL (31), CASTROYSALAZAR (27), LICENCIADOROJAS (1), MESA (1), HURTADODEMENDOZA (1) |
| low | `ArgensolaLupercioLeonardode_Isabela` | ENRIQUEZ | 108 | 51/108 (47%) | 7.25 | ENRIQUEZ (51), CECILIANACIMIENTO (30), CASTILLOSOLORZANO (11), GOMEZACOSTA (3), QUEVEDO (2) |
| low | `ClaramonteAndresde_EsclavadelcielosantaEngraciaLa` | PSEUDOHURTADODEMENDOZA | 68 | 24/68 (35%) | 7.23 | PSEUDOHURTADODEMENDOZA (24), BELMONTE (23), MEDINA (5), TORRESLORENZODE (3), LOPEZJACINTO (1) |
| low | `QuirosFranciscoBernardode_LunadelaSagrayvidadeSantaJuana` | TORRESLORENZODE | 56 | 16/56 (29%) | 7.22 | TORRESLORENZODE (16), GILENRIQUEZ (12), JIMENEZSEDENO (11), BELMONTE (4), LEIVARAMIREZ (2) |
| low | `MiradeAmescuaAntonioAtribuido_CaballerosnuevosycarbonerosdeT` | SANDOVAL | 41 | 12/41 (29%) | 7.21 | SANDOVAL (12), HERNANDEZPADILLA (5), BARRIONUEVO (5), RUIZALCEO (3), LOPEZDECASTRO (2) |
| low | `MonteserFranciscoAntoniode_LocosEntremesdedFranciscoAnton` | ROMEROROQUE | 16 | 7/16 (44%) | 7.19 | ROMEROROQUE (7) |
| low | `JosedeFigueroayCordoba_TrancaLa` | FAJARDOYACEVEDO | 16 | 6/16 (38%) | 7.16 | FAJARDOYACEVEDO (6), LICENCIADOROJAS (1), LEONORCUEVA (1) |
| low | `ElsegundoJob` | BELMONTE | 59 | 22/59 (37%) | 7.16 | BELMONTE (22), QUINONES (15), BATRES (3), FAJARDOYACEVEDO (2), LICENCIADOROJAS (1) |
| low | `LarenegadadeValladolid2` | GARCIAMARCOS | 71 | 31/71 (44%) | 7.14 | GARCIAMARCOS (31), ANDOSILLA (10), LEIVARAMIREZ (9), MOLINAYMENDOZA (4), GARCIADEPRADO (2) |
| low | `MulsaMiguelde_HurtodelneneEntremesEl` | MULSA | 15 | 3/15 (20%) | 7.13 | MULSA (3), REMON (1), TAMAYO (1), CARVAJAL (1) |
| low | `GodinezManriqueFelipe_Bastaintentarlo` | LANINI | 22 | 8/22 (36%) | 7.11 | LANINI (8), MORETO (2), CANIZARES (2), GILENRIQUEZ (2), PACHECO (2) |
| low | `MoretoyCavanaAgustin_ReyvalienteyjusticieroRicohomb` | CASTROYSALAZAR | 69 | 29/69 (42%) | 7.06 | CASTROYSALAZAR (29), SANDOVAL (14), MELO (12), GARCIAMARCOS (3), GONZALEZDEBARCIA (1) |
| low | `LeandroVadillos_PrincipiodelaInquisicionyprime` | CALLE | 95 | 46/95 (48%) | 7.04 | CALLE (46), ROSETENINO (15), MIRACLESSOTOMAYOR (3), JUANDESOTO (3), VARGAS (2) |
| low | `CubillodeAragonAlvaroAtribuido_CondeDirlosoelcondedeIrlosEl` | ROMEROROQUE | 51 | 25/51 (49%) | 6.98 | ROMEROROQUE (25), JUANDESOTO (7), GONZALEZDEBARCIA (2), BATRES (1), FAJARDOYACEVEDO (1) |
| low | `LuisdeBelmonteBermudez_CercodeSevillaporelreydonFerna` | BELMONTE | 59 | 14/59 (24%) | 6.98 | BELMONTE (14), PAREDES (12), LEIVARAMIREZ (6), ROJASZORRILLA (4), ENRIQUEZ (4) |
| low | `MoretoyCavanaAgustin_FuerzadelnaturalLa` | GILENRIQUEZ | 54 | 15/54 (28%) | 6.91 | GILENRIQUEZ (15), CASTROYSALAZAR (14), LANINI (12), GONZALEZDEBARCIA (1), VARGASMACHUCA (1) |
| low | `VegaCarpioLopede_DivinopastoroelninopastorEl` | SALAZARYTORRES | 32 | 13/32 (41%) | 6.90 | SALAZARYTORRES (13), MESA (3), ANDOSILLA (3), CERVANTES (1), GONZALEZDEBARCIA (1) |
| low | `LadevocindelasnimasdePurgatorio` | GOMEZACOSTA | 45 | 19/45 (42%) | 6.86 | GOMEZACOSTA (19), SARAVIAYMENDOZA (5), CASTILLOSOLORZANO (3), CERVANTES (2), GONZALEZDEBARCIA (1) |
| low | `FrancisodeAvellanedadelaCuevay_Nochesdeinviernoyperdoneenenfe` | FAJARDOYACEVEDO | 14 | 2/14 (14%) | 6.85 | FAJARDOYACEVEDO (2), TORRESLORENZODE (2), GARCIAMARCOS (1) |
| low | `RojasZorrillaFranciscode_CaindeCatalunaEl` | ALARCON | 69 | 30/69 (44%) | 6.84 | ALARCON (30), GARCIADEPRADO (10), PAREDES (4), CALLE (4), TORRESLORENZODE (4) |
| low | `JuanAntoniodeMojica_ReyangeldeSiciliaprincipedemon` | MORETO | 46 | 17/46 (37%) | 6.84 | MORETO (17), LANINI (7), AVELLANEDADELACUEVA (4), PACHECO (3), ROSETENINO (2) |
| low | `CASTROSALAZAR_Atribuido_ElMaestroDeNinosYLaRosca` | CASTROYSALAZAR | 8 | 3/8 (38%) | 6.68 | CASTROYSALAZAR (3), SANDOVAL (2), GONZALEZDEBARCIA (1), MELO (1), MOLINAYMENDOZA (1) |
| low | `MiradeAmescuaAntonio_JuradelprincipeLa` | MORETO | 33 | 14/33 (42%) | 6.68 | MORETO (14), ROJASZORRILLA (8), BOLEAYALVARADO (2), GODINEZMANRIQUE (1), SANDOVAL (1) |
| low | `Poesiascastellanasvarias_v2` | SANDOVAL | 364 | 71/364 (20%) | 6.59 | SANDOVAL (71), CONTRERAS (71), AVELLANEDA (26), PAREDES (25), CALDERON (24) |
| low | `JoseAntonioCasquerodelaParra_LoaalosanosdednaJosefadeFiguer` | MELO | 16 | 3/16 (19%) | 6.59 | MELO (3), LANINI (3), ROMEROROQUE (3), CASTROYSALAZAR (2), CERVANTES (1) |
| low | `ClaramonteAndresde_PastoralalbergueEl` | MESA | 67 | 24/67 (36%) | 6.57 | MESA (24), JIMENEZSEDENO (17), QUINONES (8), DAVILAYPALOMARES (3), BATRES (3) |
| low | `PachecosyPalomeques` | GILENRIQUEZ | 30 | 11/30 (37%) | 6.53 | GILENRIQUEZ (11), SANDOVAL (4), CANIZARES (4), BELMONTE (3), LANINI (2) |
| low | `MiguelSanchez_IslabarbaraLa` | TORRESLORENZODE | 61 | 26/61 (43%) | 6.47 | TORRESLORENZODE (26), ANDOSILLA (6), SANDOVAL (4), TAMAYO (4), BARRIONUEVO (4) |
| low | `Galanvalienteydiscreto` | BELMONTE | 60 | 17/60 (28%) | 6.45 | BELMONTE (17), PSEUDOHURTADODEMENDOZA (15), LEIVARAMIREZ (13), ROMEROROQUE (1), VELEZ (1) |
| low | `VALLEJOyMartinez_A_fuerza_de_armas_el_cielo_Novena` | TORRESLORENZODE | 58 | 17/58 (29%) | 6.44 | TORRESLORENZODE (17), MORETO (13), JIMENEZSEDENO (6), MENESES (6), BELMONTE (4) |
| low | `VegaCarpioLopede_DonLopedeCardona` | TORRESLORENZODE | 32 | 8/32 (25%) | 6.44 | TORRESLORENZODE (8), PACHECO (5), CAXESI (3), GONZALEZDEBARCIA (2), VARGAS (2) |
| low | `AntonioEnriquezGomez_EscaladelagraciaLa` | LORENZANA | 49 | 12/49 (24%) | 6.37 | LORENZANA (12), CAXESI (12), LOPEZDELCAMPO (9), VIDALYSALVADOR (2), AMESCUA (2) |
| low | `ClaramonteAndresde_PusosemeelsolsaliomelalunaSant` | MENESES | 62 | 15/62 (24%) | 6.35 | MENESES (15), ROJASZORRILLA (13), CALDERON (11), MORETO (5), ROSETENINO (4) |
| low | `FranciscodeVillegas_Dioshacejusticiaatodos` | LORENZANA | 56 | 27/56 (48%) | 6.34 | LORENZANA (27), LOPEZDELCAMPO (8), CAXESI (7), ROJASZORRILLA (2), GONZALEZDEBARCIA (1) |
| low | `FrancisodeAvellanedadelaCuevay_PorteriadelasdamasLa` | VIDALYSALVADOR | 1000 | 151/1000 (15%) | 6.32 | VIDALYSALVADOR (151), CONTRERAS (97), SANDOVAL (81), CECILIANACIMIENTO (62), GOMEZACOSTA (58) |
| low | `FranciscodePaulaGonzalezdeBust_GranRosadeViterbooSantaRosadeV` | LANINI | 44 | 16/44 (36%) | 6.31 | LANINI (16), MELO (13), VIDALYSALVADOR (3), LICENCIADOROJAS (1), CONTRERAS (1) |
| low | `JuanSilvestreSalvo_PosturasLas` | CANIZARES | 14 | 4/14 (29%) | 6.30 | CANIZARES (4), JIMENEZSEDENO (1), GONZALEZDEBARCIA (1) |
| low | `FranciscoAntoniodeBancesCandam_VisionesLas` | VIDALYSALVADOR | 17 | 4/17 (24%) | 6.27 | VIDALYSALVADOR (4), PACHECO (1), PAREDES (1), GONZALEZDEBARCIA (1), LOPEZDELCAMPO (1) |
| low | `TellezGabriel_BalconesdeMadridLos` | MEDINA | 73 | 21/73 (29%) | 6.19 | MEDINA (21), MESA (18), QUINONES (16), AGUADOELVIEJO (2), LICENCIADOROJAS (2) |
| low | `VegaCarpioLopede_CantaresLos` | LEIVARAMIREZ | 27 | 8/27 (30%) | 6.17 | LEIVARAMIREZ (8), BELMONTE (8), COELLO (1), MENESES (1), QUINONES (1) |
| low | `Laparida` | ANDOSILLA | 16 | 5/16 (31%) | 6.14 | ANDOSILLA (5), LICENCIADOROJAS (1), CLARAMONTE (1) |
| low | `MoretoyCavanaAgustin_LoadeJuanRanaLa` | LORENZANA | 16 | 4/16 (25%) | 6.14 | LORENZANA (4), LANINI (1), CANIZARES (1) |
| low | `FranciscoMudarra_Nadiedigamaldeldiahastaquelalu` | BELMONTE | 66 | 23/66 (35%) | 6.11 | BELMONTE (23), LEIVARAMIREZ (17), SANDOVAL (4), QUINONES (4), GALLEGOS (3) |
| low | `JosedeValdivielso_CaballerodelaardienteespadaEl` | CAXESI | 22 | 7/22 (32%) | 6.06 | CAXESI (7), CARVAJAL (3), BATRES (2), CONTRERAS (1), VIDALYSALVADOR (1) |
| low | `Poesiascastellanasvarias_v6` | GOMEZACOSTA | 182 | 47/182 (26%) | 6.04 | GOMEZACOSTA (47), CORDERO (29), ENRIQUEZ (21), GARCIAMARCOS (14), VIDALYSALVADOR (10) |
| low | `SantosdelaTorre_PrisionesdeAdanLas` | CALDERON | 42 | 14/42 (33%) | 6.04 | CALDERON (14), VIDALYSALVADOR (9), LOPEZDELCAMPO (9), PAREDES (1), COELLO (1) |
| low | `FranciscodeCuevas_MartiresJustoyPastorLos` | LOPE | 323 | 101/323 (31%) | 6.01 | LOPE (101), QUEVEDO (52), BATRES (24), MELO (21), GALLEGOS (20) |
| low | `VelezdeGuevaraLuis_PrincipepodadorEl` | SANDOVAL | 33 | 13/33 (39%) | 6.00 | SANDOVAL (13), BARRIONUEVO (4), GOMEZACOSTA (3), AVELLANEDA (3), ROMEROROQUE (1) |
| low | `CalderonAtribuidoDiegodeNajera_EcoyNarciso` | ALARCON | 177 | 57/177 (32%) | 5.93 | ALARCON (57), MOLINAYMENDOZA (45), MORETO (44), JIMENEZSEDENO (11), CAXESI (2) |
| low | `DiegodeNajerayZegri_PrimerarendencionAutohistorial` | MONTALBAN | 32 | 14/32 (44%) | 5.92 | MONTALBAN (14), ROJASZORRILLA (3), HURTADODEMENDOZA (1), TAMAYO (1), CANIZARES (1) |
| low | `GaspardeBarrionuevoyCarrionAtr_ToqueroEl` | SALAZARYTORRES | 15 | 4/15 (27%) | 5.91 | SALAZARYTORRES (4), LICENCIADOROJAS (1), LEIVARAMIREZ (1), CLARAMONTE (1) |
| low | `CaxesiJuan_DosprimeroshermanosLos` | CAXESI | 30 | 9/30 (30%) | 5.90 | CAXESI (9), CASTILLOSOLORZANO (6), TORRESLORENZODE (4), PAREDES (2), ENRIQUEZ (1) |
| low | `TELLEZ_BalconesdeMadrid_British` | GONZALEZDETORRES | 55 | 22/55 (40%) | 5.82 | GONZALEZDETORRES (22), CASTROYSALAZAR (20), LOPEZDECASTRO (11), MELO (1) |
| low | `MoretoyCavanaAgustin_CasadeAustriaLa` | ROJASZORRILLA | 23 | 8/23 (35%) | 5.79 | ROJASZORRILLA (8), LEIVARAMIREZ (5), LORENZANA (1), JIMENEZSEDENO (1), VELEZ (1) |
| low | `JuandeZabaletaAntonioMartinezd_ReyEnriqueelenfermoEl` | LANINI | 56 | 17/56 (30%) | 5.75 | LANINI (17), TORRESLORENZODE (16), CASTROYSALAZAR (5), GILENRIQUEZ (5), GONZALEZDEBARCIA (1) |
| low | `Santiagoelverde` | CASTILLOSOLORZANO | 42 | 10/42 (24%) | 5.73 | CASTILLOSOLORZANO (10), SANDOVAL (10), LOPEZDECARDENA (4), GONZALEZDEBARCIA (2), ENRIQUEZ (2) |
| low | `Poesiascastellanasvarias_v1` | AVELLANEDA | 429 | 160/429 (37%) | 5.70 | AVELLANEDA (160), VARGASMACHUCA (78), VIDALYSALVADOR (76), CECILIANACIMIENTO (45), PAREDES (16) |
| low | `MoretoyCavanaAgustin_SantoCristodeCabrillaEl` | PAREDES | 62 | 20/62 (32%) | 5.68 | PAREDES (20), GARCIADEPRADO (17), COELLO (4), CORDERO (3), CASTILLOSOLORZANO (2) |
| low | `VegaCarpioLopede_MuertosvivosLos` | ROMEROROQUE | 53 | 23/53 (43%) | 5.67 | ROMEROROQUE (23), CARVAJAL (11), BELMONTE (1), CASTILLOSOLORZANO (1), GONZALEZDEBARCIA (1) |
| low | `PedroRoseteNino_Nohaycontralasuerteindustria` | ANDOSILLA | 62 | 22/62 (36%) | 5.67 | ANDOSILLA (22), LEONORCUEVA (12), LEIVARAMIREZ (10), BELMONTE (3), LOPEZJACINTO (2) |
| low | `LasespigasdeRuth` | GONZALEZDEBARCIA | 48 | 22/48 (46%) | 5.67 | GONZALEZDEBARCIA (22), CANIZARES (6), ROMEROROQUE (6), AVELLANEDADELACUEVA (3), MOLINAYMENDOZA (2) |
| low | `LasprisionesdeAdan` | CANIZARES | 28 | 12/28 (43%) | 5.67 | CANIZARES (12), CASTROYSALAZAR (8), VIDALYSALVADOR (2), ROMEROROQUE (2), MOLINAYMENDOZA (1) |
| low | `AgustinColladodelHierro_Jerusalenrestauradayelgransepu` | TORRESLORENZODE | 55 | 19/55 (34%) | 5.66 | TORRESLORENZODE (19), LEIVARAMIREZ (9), PAREDES (6), GARCIAMARCOS (5), MENESES (3) |
| low | `COUTOPESTANA_TodoEsRiesgoLoFingido` | GILENRIQUEZ | 46 | 16/46 (35%) | 5.62 | GILENRIQUEZ (16), JIMENEZSEDENO (14), CASTROYSALAZAR (9), TORRESLORENZODE (4), LANINI (2) |
| low | `SimonAguadoelViejoAtribuido_MudosbailarinesFindefiestaLos` | ANDOSILLA | 10 | 4/10 (40%) | 5.60 | ANDOSILLA (4), MATOSFRAGOSO (1), GRACIAN (1) |
| low | `AntonioMartinezdeMeneses_LocurasyamoresdelprincipeFisbe` | TORRESLORENZODE | 24 | 5/24 (21%) | 5.59 | TORRESLORENZODE (5), LORENZANA (5), JUANDESOTO (2), CASTILLOSOLORZANO (1), ROJASVILLANDRANDO (1) |
| low | `VegaCarpioLopede_HijosdeMariaAutodelRosarioLos` | BARRIONUEVO | 20 | 5/20 (25%) | 5.58 | BARRIONUEVO (5), MATOSFRAGOSO (3), CECILIANACIMIENTO (1), GONZALEZDEBARCIA (1), MONTALBAN (1) |
| low | `JoseTrejo_PericoyGileta` | PAREDES | 14 | 4/14 (29%) | 5.58 | PAREDES (4), PACHECO (1) |
| low | `AntonioMartinezdeMenesesAtribu_Pedirjusticiaalculpado` | JIMENEZSEDENO | 60 | 20/60 (33%) | 5.50 | JIMENEZSEDENO (20), MOLINAYMENDOZA (9), GARCIAMARCOS (4), ENRIQUEZ (4), SARAVIAYMENDOZA (4) |
| low | `CepedaAtribuido_SanGines` | LORENZANA | 24 | 10/24 (42%) | 5.50 | LORENZANA (10), LOPEZDECASTRO (4), CARVAJAL (1), CECILIANACIMIENTO (1), CAXESI (1) |
| low | `RojasZorrillaFranciscode_Nohayserpadresiendorey` | ROJASZORRILLA | 49 | 18/49 (37%) | 5.50 | ROJASZORRILLA (18), BELMONTE (13), LEIVARAMIREZ (8), QUEVEDO (3), CARVAJAL (1) |
| low | `FernandodeAyalayManuel_DudaenlaobligacionLa` | GOMEZACOSTA | 33 | 12/33 (36%) | 5.50 | GOMEZACOSTA (12), GARCIAMARCOS (3), VARGASMACHUCA (3), CORDERO (3), ROMEROROQUE (2) |
| low | `CanizaresySuarezdeToledoJosede_IndianoperseguidodBrunodeCalah` | CASTROYSALAZAR | 70 | 21/70 (30%) | 5.45 | CASTROYSALAZAR (21), GARCIAMARCOS (19), MOLINAYMENDOZA (17), LICENCIADOROJAS (1), CANIZARES (1) |
| low | `VILLEGAS_CulpaProvechosa` | LORENZANA | 23 | 11/23 (48%) | 5.39 | LORENZANA (11), PACHECO (5), MORETO (3), BARRIONUEVO (1), LOPEZDECARDENA (1) |
| low | `MatosFragosoJuandeSebastianRod_LetradodelcieloEl` | TORRESLORENZODE | 62 | 22/62 (36%) | 5.39 | TORRESLORENZODE (22), PAREDES (20), GARCIAMARCOS (7), MULSA (4), LICENCIADOROJAS (1) |
| low | `VegaCarpioLopede_LocuraporlahonraLa` | SANDOVAL | 34 | 9/34 (26%) | 5.38 | SANDOVAL (9), GARCIAMARCOS (8), CASTROYSALAZAR (3), ROMEROROQUE (1), TORRESLORENZODE (1) |
| low | `VegaCarpioLopede_DevociondelRosarioLa` | LEIVARAMIREZ | 64 | 29/64 (45%) | 5.38 | LEIVARAMIREZ (29), TORRESLORENZODE (19), FAJARDOYACEVEDO (8), JUANDESOTO (1), MONTALBAN (1) |
| low | `LajuventuddeS.IsidroLabrador` | MEDINA | 33 | 11/33 (33%) | 5.36 | MEDINA (11), CUEVAYSILVA (5), VARGAS (4), SANTATERESA (2), LICENCIADOROJAS (1) |
| low | `JUANAINES_EmpenosCasa` | ROMEROROQUE | 62 | 20/62 (32%) | 5.35 | ROMEROROQUE (20), MOLINAYMENDOZA (16), CANIZARES (9), LICENCIADOROJAS (1), CASTROYSALAZAR (1) |
| low | `JuanaInesdelaCruz_EmpenosdeunacasaLos` | ROMEROROQUE | 62 | 20/62 (32%) | 5.35 | ROMEROROQUE (20), MOLINAYMENDOZA (16), CANIZARES (9), LICENCIADOROJAS (1), CASTROYSALAZAR (1) |
| low | `VegaCarpioLopede_CelosdeRodamonteLos` | ROMEROROQUE | 52 | 19/52 (36%) | 5.34 | ROMEROROQUE (19), CARVAJAL (5), GOMEZACOSTA (4), FAJARDOYACEVEDO (3), CALLE (2) |
| low | `FranciscodelaTorreySevil_TresnochesLas` | ROSETENINO | 58 | 28/58 (48%) | 5.33 | ROSETENINO (28), LEIVARAMIREZ (14), BELMONTE (4), MULSA (1), VARGAS (1) |
| low | `AgustindeSalazaryTorresAtribui_CasadelamorLa` | ROJASZORRILLA | 110 | 34/110 (31%) | 5.30 | ROJASZORRILLA (34), GILENRIQUEZ (28), LEIVARAMIREZ (26), BELMONTE (12), CALDERON (4) |
| low | `JuanBautistaDiamante_JuanillaladeJerezIndustriasdea` | CASTILLOSOLORZANO | 70 | 34/70 (49%) | 5.25 | CASTILLOSOLORZANO (34), FAJARDOYACEVEDO (10), CASTROYSALAZAR (4), GARCIAMARCOS (4), MELO (3) |
| low | `VelezdeGuevaraLuis_LunadelasierraLa` | BELMONTE | 55 | 24/55 (44%) | 5.23 | BELMONTE (24), ROJASZORRILLA (14), LEIVARAMIREZ (9), ROSETENINO (1), MONTALBAN (1) |
| low | `PedroFranciscodeLaniniySagredo_CumplirauntiempoquienamaconsuD` | MORETO | 68 | 22/68 (32%) | 5.22 | MORETO (22), SANDOVAL (11), LEIVARAMIREZ (11), CANIZARES (6), CASTROYSALAZAR (5) |
| low | `MatosFragosoJuande_Conamornohayamistad` | CONTRERAS | 87 | 40/87 (46%) | 5.21 | CONTRERAS (40), CALDERON (9), ALARCON (8), QUINONES (7), CARVAJAL (6) |
| low | `MALO_AmistadVenceAlRigor2` | LOPEZJACINTO | 80 | 17/80 (21%) | 5.21 | LOPEZJACINTO (17), LANINI (11), MELO (7), GARCIAMARCOS (7), MOLINAYMENDOZA (6) |
| low | `Elmejoresposo` | CASTILLOSOLORZANO | 64 | 28/64 (44%) | 5.20 | CASTILLOSOLORZANO (28), GARCIADEPRADO (24), BANCESCANDAMO (2), VIDALYSALVADOR (1) |
| low | `Elcapuchinoescoces` | ANDOSILLA | 68 | 13/68 (19%) | 5.17 | ANDOSILLA (13), LEIVARAMIREZ (13), JIMENEZSEDENO (9), MOLINAYMENDOZA (6), BELMONTE (3) |
| low | `LasMacarenas` | REMON | 102 | 36/102 (35%) | 5.17 | REMON (36), CLARAMONTE (28), SANTATERESA (9), MESA (9), ANDOSILLA (8) |
| low | `MontalbanJuanPerezde_MasconstantemujerLa` | CONTRERAS | 56 | 15/56 (27%) | 5.14 | CONTRERAS (15), ROJASZORRILLA (12), LEIVARAMIREZ (7), CALDERON (3), VELEZ (3) |
| low | `SebastianAntoniodeGadeayOviedo_ImagendelsacramentoSanJuandeDi` | ROMEROROQUE | 55 | 27/55 (49%) | 5.14 | ROMEROROQUE (27), FAJARDOYACEVEDO (10), GONZALEZDEBARCIA (7), MOLINAYMENDOZA (1), HURTADODEMENDOZA (1) |
| low | `AntonioCoelloyOchoa_CondedeEssexEl` | ANDOSILLA | 64 | 13/64 (20%) | 5.12 | ANDOSILLA (13), LEIVARAMIREZ (12), ROJASZORRILLA (8), CLARAMONTE (4), CANIZARES (3) |
| low | `ZAPATA_Conclusionesburlescas` | VIDALYSALVADOR | 15 | 7/15 (47%) | 5.10 | VIDALYSALVADOR (7), CERVANTES (5), HURTADODEMENDOZA (1), QUINONES (1) |
| low | `DiegodeRosasyArgomedo_Dondehayvalorhayhonor` | GARCIAMARCOS | 52 | 9/52 (17%) | 5.05 | GARCIAMARCOS (9), ALARCON (9), RUIZALCEO (7), CARVAJAL (6), AGUADOELVIEJO (3) |
| low | `ManueldeArriagaFeijooyRivadene_DosciudadesopuestasLas` | GARCIADEPRADO | 38 | 17/38 (45%) | 5.03 | GARCIADEPRADO (17), MORETO (2), MENESES (2), ALARCON (2), GONZALEZDEBARCIA (2) |
| low | `SaenzdeTejeraJuanFrancisco_CasasdeMadridLas` | LANINI | 14 | 5/14 (36%) | 5.02 | LANINI (5) |
| low | `Elpintordesudeshonra` | LEIVARAMIREZ | 77 | 25/77 (32%) | 5.01 | LEIVARAMIREZ (25), CALLE (22), FAJARDOYACEVEDO (16), GONZALEZDEBARCIA (1), AMESCUA (1) |
| low | `MonteserFranciscoAntoniode_PerdicesLas` | ROMEROROQUE | 16 | 6/16 (38%) | 5.01 | ROMEROROQUE (6), CASTROYSALAZAR (2) |
| low | `VegaCarpioLopede_TriunfodelaIglesiaEl` | BELMONTE | 22 | 8/22 (36%) | 4.99 | BELMONTE (8), SANDOVAL (4), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `DonPedroMiago` | ALARCON | 57 | 12/57 (21%) | 4.99 | ALARCON (12), ROSETENINO (12), GARCIADEPRADO (11), JIMENEZSEDENO (10), CALLE (2) |
| low | `MontalbanJuanPerezde_PrincipeesclavoEscanderbechEl` | ROJASZORRILLA | 33 | 12/33 (36%) | 4.97 | ROJASZORRILLA (12), GALLEGOS (4), CLARAMONTE (3), CARVAJAL (2), GONZALEZDETORRES (1) |
| low | `CEPEDA_EnredosMartin` | TORRESLORENZODE | 34 | 16/34 (47%) | 4.97 | TORRESLORENZODE (16), JUANDESOTO (14), MULSA (2) |
| low | `BANCESyVALLEJO_Afectomayorlealtadsangreamor_Novena` | MOLINAYMENDOZA | 76 | 36/76 (47%) | 4.94 | MOLINAYMENDOZA (36), GILENRIQUEZ (28), CALLE (4), CANIZARES (3), JIMENEZSEDENO (2) |
| low | `MoretoyCavanaAgustin_ParecidoEl` | CASTROYSALAZAR | 78 | 20/78 (26%) | 4.93 | CASTROYSALAZAR (20), SANDOVAL (11), GARCIAMARCOS (9), MOLINAYMENDOZA (8), QUINONES (7) |
| low | `AlfaroAlonso_HombredePortugalEl` | LEIVARAMIREZ | 62 | 15/62 (24%) | 4.90 | LEIVARAMIREZ (15), CALDERON (15), BATRES (11), GARCIADEPRADO (5), MENESES (2) |
| low | `MiradeAmescuaAntonio_PruebasdeCristoLas` | ROJASZORRILLA | 28 | 10/28 (36%) | 4.87 | ROJASZORRILLA (10), CLARAMONTE (2), BELMONTE (2), GONZALEZDEBARCIA (1), MORETO (1) |
| low | `AntoniodeSolisAtribuidoJeronim_Hacercadaunoloquedebe` | LEIVARAMIREZ | 55 | 18/55 (33%) | 4.81 | LEIVARAMIREZ (18), BELMONTE (16), GARCIAMARCOS (3), CALLE (2), MOLINAYMENDOZA (2) |
| low | `ArgensolaLupercioLeonardode_IsabelayLupercio` | MESA | 22 | 9/22 (41%) | 4.80 | MESA (9), CUEVAYSILVA (4), JIMENEZSEDENO (1), LICENCIADOROJAS (1), MEDINA (1) |
| low | `ElvalornotieneedadySansondeExtremadura` | MORETO | 71 | 24/71 (34%) | 4.79 | MORETO (24), GARCIADEPRADO (17), CALDERON (4), ALARCON (4), LEIVARAMIREZ (4) |
| low | `MoretoyCavanaAgustin_MerecerparaalcanzarLafortuname` | BATRES | 63 | 15/63 (24%) | 4.79 | BATRES (15), JIMENEZSEDENO (11), ALARCON (7), FAJARDOYACEVEDO (6), LEIVARAMIREZ (5) |
| low | `MatiasdeCastroAtribuido_TorosfingidosLos` | QUINONES | 17 | 3/17 (18%) | 4.77 | QUINONES (3), FAJARDOYACEVEDO (1), ROMEROROQUE (1), ANDOSILLA (1), HURTADODEMENDOZA (1) |
| low | `ElpobremspoderosoSanJuandeDios` | SANDOVAL | 52 | 17/52 (33%) | 4.76 | SANDOVAL (17), MEDINA (13), GILENRIQUEZ (9), LEONORCUEVA (3), LICENCIADOROJAS (1) |
| low | `MiradeAmescuaAntonio_Galanvalienteydiscreto` | LEIVARAMIREZ | 52 | 16/52 (31%) | 4.75 | LEIVARAMIREZ (16), BATRES (12), QUINONES (4), MORETO (3), GRACIAN (1) |
| low | `AnonimoMejiaAtribuido_NaturalextranjeraLa` | CASTILLOSOLORZANO | 43 | 11/43 (26%) | 4.72 | CASTILLOSOLORZANO (11), LOPE (9), ALARCON (5), BATRES (4), VILLEGASDELACRUZ (2) |
| low | `CanizaresySuarezdeToledoJosede_GranhistoriadelmundoComediaale` | MOLINAYMENDOZA | 28 | 12/28 (43%) | 4.72 | MOLINAYMENDOZA (12), JIMENEZSEDENO (3), CANIZARES (2), ANDOSILLA (2), LORENZANA (1) |
| low | `Comopadreycomorey2` | CALDERON | 55 | 24/55 (44%) | 4.71 | CALDERON (24), ROSETENINO (8), LEIVARAMIREZ (4), QUINONES (2), GARCIADEPRADO (2) |
| low | `CanizaresySuarezdeToledoJosede_Hombredemonioymujer` | GARCIAMARCOS | 82 | 27/82 (33%) | 4.69 | GARCIAMARCOS (27), GARCIADEPRADO (21), SANDOVAL (8), VERATASSIS (6), LANINI (5) |
| low | `TellezGabriel_TercerosdesanFranciscooLaterce` | BELMONTE | 50 | 23/50 (46%) | 4.67 | BELMONTE (23), ROJASZORRILLA (9), LEIVARAMIREZ (5), REMON (3), CAXESI (2) |
| low | `MigueldeCervantesSaavederaMigu_CercodeNumanciaEl` | AVELLANEDA | 40 | 7/40 (18%) | 4.62 | AVELLANEDA (7), SANDOVAL (5), CECILIANACIMIENTO (3), QUEVEDO (3), ENRIQUEZ (3) |
| low | `GarciaLorenzoAtribuido_Hadosyladoshacendichososydesdi` | SANDOVAL | 67 | 21/67 (31%) | 4.61 | SANDOVAL (21), BELMONTE (20), CLARAMONTE (10), MORETO (2), AGUADOELVIEJO (1) |
| low | `Poesiascastellanasvarias_v3` | VIDALYSALVADOR | 306 | 76/306 (25%) | 4.59 | VIDALYSALVADOR (76), CONTRERAS (26), BANCESCANDAMO (21), CECILIANACIMIENTO (19), LOPEZDELCAMPO (14) |
| low | `ArroyoJosede_SanJuandeDios` | ROSETENINO | 54 | 21/54 (39%) | 4.59 | ROSETENINO (21), GILENRIQUEZ (9), TORRESLORENZODE (6), LEIVARAMIREZ (5), ALARCON (2) |
| low | `CubillodeAragonAlvaro_BastardodeCastillaEl` | GARCIAMARCOS | 76 | 32/76 (42%) | 4.58 | GARCIAMARCOS (32), CALLE (17), FAJARDOYACEVEDO (8), LEIVARAMIREZ (4), MONTALBAN (2) |
| low | `MiguelSanchez_GuardacuidadosaLa` | CASTILLOSOLORZANO | 76 | 30/76 (40%) | 4.58 | CASTILLOSOLORZANO (30), MESA (12), DIAMANTE (5), MENESES (4), MORETO (4) |
| low | `CristobalAriasdeRiberaAtribuid_Espadacaballoypintura` | GARCIAMARCOS | 74 | 19/74 (26%) | 4.57 | GARCIAMARCOS (19), MELO (12), ANDOSILLA (9), MOLINAYMENDOZA (7), SANDOVAL (4) |
| low | `ClaramonteAndresde_InfeliceDoroteaLa` | PSEUDOHURTADODEMENDOZA | 145 | 36/145 (25%) | 4.55 | PSEUDOHURTADODEMENDOZA (36), QUINONES (22), LEIVARAMIREZ (14), BELMONTE (13), BATRES (13) |
| low | `JeronimoCifuentes_FamadelamejordamaLa` | ALARCON | 66 | 21/66 (32%) | 4.55 | ALARCON (21), MOLINAYMENDOZA (10), GARCIADEPRADO (8), FAJARDOYACEVEDO (5), LEIVARAMIREZ (4) |
| low | `VegaCarpioLopede_SuertedelosreyesLa` | CARVAJAL | 42 | 18/42 (43%) | 4.55 | CARVAJAL (18), CAXESI (12), CONTRERAS (5), BANCESCANDAMO (1), CERVANTES (1) |
| low | `JuanClaudiodelaHozyMota_InvisibleEl` | ALARCON | 14 | 4/14 (29%) | 4.54 | ALARCON (4), CANIZARES (1), MORETO (1) |
| low | `MontalbanJuanPerezde_Nohayvidacomolahonra` | BELMONTE | 42 | 18/42 (43%) | 4.53 | BELMONTE (18), ROJASZORRILLA (12), CASTILLOSOLORZANO (1), LEIVARAMIREZ (1), MONTALBAN (1) |
| low | `CastroyBellvisGuillendeAtribui_MaravillasdeBabiloniaLas` | MEDINA | 64 | 21/64 (33%) | 4.49 | MEDINA (21), SANDOVAL (12), ANDOSILLA (8), QUINONES (5), MESA (3) |
| low | `VegaCarpioLopede_MargaritapreciosaLa` | VILLEGASJUANBAUTISTA | 23 | 5/23 (22%) | 4.48 | VILLEGASJUANBAUTISTA (5), ROSETENINO (4), BELMONTE (4), LEIVARAMIREZ (1), ROJASZORRILLA (1) |
| low | `AntoniodeZamoraAtribuido_VerdadytiempoentiempoLa` | VIDALYSALVADOR | 229 | 74/229 (32%) | 4.48 | VIDALYSALVADOR (74), PAREDES (28), CECILIANACIMIENTO (19), VARGASMACHUCA (18), MARCHANTE (17) |
| low | `VegaCarpioLopedeAtribuido_CircuncisionysangriadeCristonu` | LEIVARAMIREZ | 37 | 15/37 (40%) | 4.44 | LEIVARAMIREZ (15), BELMONTE (7), ROJASZORRILLA (4), BANCESCANDAMO (1), GRACIAN (1) |
| low | `VegaCarpioLopede_Llegarenocasion` | QUINONES | 90 | 32/90 (36%) | 4.44 | QUINONES (32), LEIVARAMIREZ (15), LOPEZDELCAMPO (9), CONTRERAS (7), CAXESI (7) |
| low | `JuanCalderondelaBarcayCordoba_Dichamasmaslogradaporlaambicio` | RUANO | 70 | 34/70 (49%) | 4.40 | RUANO (34), GONZALEZDEBARCIA (9), VARGASMACHUCA (7), CASTILLOSOLORZANO (2), LANINI (2) |
| low | `GodinezManriqueFelipe_SanMateoenEtiopia` | CAXESI | 54 | 21/54 (39%) | 4.39 | CAXESI (21), ROJASZORRILLA (14), VILLEGASJUANBAUTISTA (2), MENESES (2), VARGASMACHUCA (1) |
| low | `FelixPardodelaCasta_Hallarlamuerteensuscelos` | LEIVARAMIREZ | 83 | 39/83 (47%) | 4.39 | LEIVARAMIREZ (39), FAJARDOYACEVEDO (14), CALLE (9), QUINONES (6), SAAVEDRAFAJARDO (1) |
| low | `JUANAINES_LibroProfesiones` | LEONORCUEVA | 386 | 56/386 (14%) | 4.38 | LEONORCUEVA (56), CERVANTES (51), AVELLANEDA (47), CECILIANACIMIENTO (44), VIDALYSALVADOR (32) |
| low | `ArboredaAlejandro_Enganoshayquesonjustosenlidesd` | BELMONTE | 69 | 33/69 (48%) | 4.38 | BELMONTE (33), LEONORCUEVA (19), MARCHANTE (7), REMON (1), VIDALYSALVADOR (1) |
| low | `TORRE_SentidosCorporales_Autografo` | PAREDES | 53 | 11/53 (21%) | 4.37 | PAREDES (11), MELO (3), SANDOVAL (3), CUENCAYARGUELLO (3), BOLEAYALVARADO (1) |
| low | `SebastianRodriguezdeVillavicio_SiylaalmonedaEl` | CLARAMONTE | 16 | 4/16 (25%) | 4.36 | CLARAMONTE (4), SALAZARYTORRES (2), LICENCIADOROJAS (1) |
| low | `JosedeValdivielso_LococuerdoEl` | TORRESLORENZODE | 72 | 19/72 (26%) | 4.34 | TORRESLORENZODE (19), ROMEROROQUE (14), GARCIAMARCOS (9), SANDOVAL (8), ONAVIEDMAYTORRES (3) |
| low | `FelipeLopez_EscanderbegComediaburlesca` | LORENZANA | 47 | 19/47 (40%) | 4.34 | LORENZANA (19), ALARCON (5), ROSETENINO (4), LEONORCUEVA (2), AVELLANEDA (2) |
| low | `Elpleitomatrimonialdelcuerpoyelalma2` | GONZALEZDEBARCIA | 37 | 10/37 (27%) | 4.34 | GONZALEZDEBARCIA (10), CANIZARES (9), CASTROYSALAZAR (4), VIDALYSALVADOR (2), SANDOVAL (1) |
| low | `CastroyVega_Floridasenectudyhonestidaddefe` | SANDOVAL | 38 | 15/38 (40%) | 4.33 | SANDOVAL (15), FAJARDOYACEVEDO (7), BELMONTE (4), CARVAJAL (1), GONZALEZDEBARCIA (1) |
| low | `VelezdeGuevaraLuis_Julianoapostata` | LANINI | 38 | 13/38 (34%) | 4.33 | LANINI (13), PAREDES (5), TORRESLORENZODE (3), ONAVIEDMAYTORRES (2), LICENCIADOROJAS (1) |
| low | `QuinonesdeBenaventeLuis_EntremesesdellicenciadoLuisQui` | BELMONTE | 88 | 25/88 (28%) | 4.32 | BELMONTE (25), LEIVARAMIREZ (13), MONTALBAN (13), ROJASZORRILLA (12), MENESES (6) |
| low | `Nohayserpadresiendore` | ROSETENINO | 61 | 23/61 (38%) | 4.32 | ROSETENINO (23), CALDERON (10), MORETO (9), BELMONTE (4), GARCIAMARCOS (2) |
| low | `CalderonArriagaFeijooyRivadene_DivinocazadorElLoayAuto` | VIDALYSALVADOR | 42 | 13/42 (31%) | 4.30 | VIDALYSALVADOR (13), GONZALEZDEBARCIA (10), PAREDES (7), CANIZARES (1) |
| low | `ElCondeLucanor` | BELMONTE | 82 | 38/82 (46%) | 4.29 | BELMONTE (38), MONTALBAN (9), ROJASZORRILLA (7), GILENRIQUEZ (6), GARCIADEPRADO (4) |
| low | `TellezGabriel_ComohandeserlosamigosNonplusul` | MESA | 60 | 21/60 (35%) | 4.29 | MESA (21), SALAZARYTORRES (9), ANDOSILLA (9), QUINONES (4), TORRESLORENZODE (3) |
| low | `MENDOZA_MaridohacemujerEl` | ROJASZORRILLA | 56 | 20/56 (36%) | 4.28 | ROJASZORRILLA (20), BELMONTE (10), CASTILLOSOLORZANO (7), MORETO (4), LEIVARAMIREZ (2) |
| low | `AntonioBiruegaZelaya_MasdichosoportalEl` | PAREDES | 28 | 13/28 (46%) | 4.24 | PAREDES (13), LOPEZJACINTO (3), MORETO (3), CUEVAYSILVA (1) |
| low | `FIGUEROA_FIGUEROA_ALARCON_MentirYMudarse_Autografo` | QUINONES | 141 | 36/141 (26%) | 4.23 | QUINONES (36), BARRIONUEVO (22), MORETO (16), MONTALBAN (14), LEIVARAMIREZ (8) |
| low | `Poesiascastellanasvarias_v4` | VIDALYSALVADOR | 322 | 132/322 (41%) | 4.23 | VIDALYSALVADOR (132), PAREDES (69), VARGASMACHUCA (20), AVELLANEDA (19), CASTILLOSOLORZANO (13) |
| low | `CastroMatiasdeAtribuido_AlcaldeytorosfingidosEl` | CLARAMONTE | 27 | 6/27 (22%) | 4.22 | CLARAMONTE (6), GALLEGOS (2), LICENCIADOROJAS (1), GODINEZMANRIQUE (1), CUENCAYARGUELLO (1) |
| low | `MontalbanJuanPerezde_MariscaldeVironEl` | MENESES | 48 | 12/48 (25%) | 4.21 | MENESES (12), TORRESLORENZODE (10), ROSETENINO (7), ROJASZORRILLA (6), LEIVARAMIREZ (3) |
| low | `OVANDO_Atalanta_Autografo` | SANDOVAL | 66 | 25/66 (38%) | 4.21 | SANDOVAL (25), BELMONTE (13), FAJARDOYACEVEDO (6), TORRESLORENZODE (6), GARCIAMARCOS (4) |
| low | `NuestraSenoradelaVargadelavilladeuceda` | ENRIQUEZ | 21 | 6/21 (29%) | 4.20 | ENRIQUEZ (6), CLARAMONTE (1), GONZALEZDEBARCIA (1), VILLEGASDELACRUZ (1), VARGAS (1) |
| low | `RojasZorrillaFranciscode_Numanciacercada` | BATRES | 72 | 13/72 (18%) | 4.20 | BATRES (13), CAXESI (11), CASTILLOSOLORZANO (8), QUINONES (4), GONZALEZDEBARCIA (3) |
| low | `DiegodeFigueroayCordobaJosedeF_MasheroicafinezayfortunasdeIsa` | ROJASZORRILLA | 147 | 73/147 (50%) | 4.20 | ROJASZORRILLA (73), MORETO (6), LEIVARAMIREZ (6), ROSETENINO (5), BATRES (5) |
| low | `VegaCarpioLopede_NuevossucesosdelgranduquedeMos` | SARAVIAYMENDOZA | 105 | 20/105 (19%) | 4.19 | SARAVIAYMENDOZA (20), CARVAJAL (19), VARGAS (17), AGUADOELVIEJO (12), CALLE (3) |
| low | `JuandeZabaleta_Osarmorirdalavida` | GILENRIQUEZ | 24 | 6/24 (25%) | 4.18 | GILENRIQUEZ (6), CANIZARES (6), SANDOVAL (3), BELMONTE (2), GONZALEZDEBARCIA (1) |
| low | `MatosFragosoJuandeAtribuido_FolionEl` | CARVAJAL | 14 | 3/14 (21%) | 4.18 | CARVAJAL (3), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), HURTADODEMENDOZA (1) |
| low | `ROSETE_MATOS_AllaSeVera` | PAREDES | 69 | 21/69 (30%) | 4.13 | PAREDES (21), MEDINA (12), AVELLANEDA (8), TORRESLORENZODE (5), VERATASSIS (2) |
| low | `JuanSanchezAtribuido_TomadeTunezylaGoletaporelEmper` | MATOSFRAGOSO | 44 | 11/44 (25%) | 4.11 | MATOSFRAGOSO (11), CUEVAYSILVA (6), LICENCIADOROJAS (5), MESA (4), BANCESCANDAMO (3) |
| low | `AntonioMartinezdeMeneses_CeloscontraloscelosLos` | LEIVARAMIREZ | 66 | 13/66 (20%) | 4.10 | LEIVARAMIREZ (13), JIMENEZSEDENO (9), MENESES (7), MOLINAYMENDOZA (6), FAJARDOYACEVEDO (5) |
| low | `CARO_Sonetosvarios` | CONTRERAS | 283 | 139/283 (49%) | 4.10 | CONTRERAS (139), ONAVIEDMAYTORRES (35), LOPEZJACINTO (21), AVELLANEDADELACUEVA (15), CARVAJAL (9) |
| low | `Lasnueces` | CALLE | 25 | 7/25 (28%) | 4.09 | CALLE (7), GILENRIQUEZ (3), VERATASSIS (1), GARCIAMARCOS (1) |
| low | `RemonAlonsode_HijoprodigoAutoEl` | MONTALBAN | 27 | 10/27 (37%) | 4.09 | MONTALBAN (10), CARVAJAL (2), BELMONTE (2), LEIVARAMIREZ (2), LICENCIADOROJAS (1) |
| low | `VALDES_GaleotasdeArgelLas` | CALDERON | 18 | 4/18 (22%) | 4.08 | CALDERON (4), LOPE (3), CARVAJAL (3), AMESCUA (3), QUINONES (2) |
| low | `JoseCastaneda_PazgeneralLa` | VIDALYSALVADOR | 74 | 29/74 (39%) | 4.07 | VIDALYSALVADOR (29), VERATASSIS (19), CASTROYSALAZAR (6), GARCIAMARCOS (3), LICENCIADOROJAS (1) |
| low | `VelezdeGuevaraLuis_Cumplirdosobligacionesyduquesa` | QUINONES | 64 | 24/64 (38%) | 4.05 | QUINONES (24), FAJARDOYACEVEDO (12), CALDERON (8), ALARCON (3), GILENRIQUEZ (2) |
| low | `ArboredaAlejandro_PrimertemplodeCristoEl` | GARCIADEPRADO | 76 | 36/76 (47%) | 4.04 | GARCIADEPRADO (36), CALDERON (13), CONTRERAS (4), ANDOSILLA (3), QUINONES (2) |
| low | `VegaCarpioLopede_Bobaparalosotrosydiscretaparas` | LEIVARAMIREZ | 115 | 39/115 (34%) | 4.02 | LEIVARAMIREZ (39), LICENCIADOROJAS (23), AVELLANEDA (22), MEDINA (12), CASTILLOSOLORZANO (3) |
| low | `VegaCarpioLopede_TusondelreydelcieloEl` | SANDOVAL | 24 | 10/24 (42%) | 4.01 | SANDOVAL (10), GONZALEZDEBARCIA (1), CUEVAYSILVA (1), MONTALBAN (1), VERATASSIS (1) |
| low | `MiradeAmescuaAntonioAtribuidoO_Loqueletocaalvalor` | GILENRIQUEZ | 103 | 41/103 (40%) | 4.00 | GILENRIQUEZ (41), BOLEAYALVARADO (26), CALLE (3), JIMENEZSEDENO (2), BELMONTE (2) |
| low | `AntoniodeSolis_MasdichosavenganzaLa` | MOLINAYMENDOZA | 72 | 15/72 (21%) | 3.98 | MOLINAYMENDOZA (15), HOZYMOTA (12), MULSA (12), CASTILLOSOLORZANO (6), LEIVARAMIREZ (4) |
| low | `JosedeValdivielsoAtribuidoLuis_Pruebasdellinajehumanooencomie` | ENRIQUEZ | 29 | 11/29 (38%) | 3.97 | ENRIQUEZ (11), QUEVEDO (5), LOPE (2), ROJASZORRILLA (2), GONZALEZDEBARCIA (1) |
| low | `Pedirjusticiaalculpado` | JIMENEZSEDENO | 60 | 18/60 (30%) | 3.97 | JIMENEZSEDENO (18), MOLINAYMENDOZA (10), GARCIAMARCOS (6), ENRIQUEZ (5), GARCIADEPRADO (4) |
| low | `AYALA_HechosyTravesuras1` | MEDINA | 70 | 30/70 (43%) | 3.97 | MEDINA (30), GILENRIQUEZ (19), MELO (11), LANINI (10) |
| low | `Castillo_amistadinfelice` | GILENRIQUEZ | 92 | 29/92 (32%) | 3.97 | GILENRIQUEZ (29), VIDALYSALVADOR (21), GARCIADEPRADO (16), QUEVEDO (8), LEIVARAMIREZ (8) |
| low | `MARTINEZDEMENESES_PedirJusticiaAlCulpado` | PAREDES | 110 | 26/110 (24%) | 3.97 | PAREDES (26), AVELLANEDA (22), ENRIQUEZ (15), VIDALYSALVADOR (11), SANDOVAL (7) |
| low | `RojasZorrillaFranciscode_TrabajosdeTobiasLos` | CASTROYSALAZAR | 79 | 23/79 (29%) | 3.97 | CASTROYSALAZAR (23), VIDALYSALVADOR (20), SANDOVAL (11), CANIZARES (6), SARAVIAYMENDOZA (2) |
| low | `QuirosFranciscoBernardode_MacilentoyastrologofingidoElTr` | ANDOSILLA | 15 | 4/15 (27%) | 3.93 | ANDOSILLA (4), SALAZARYTORRES (1), MENESES (1), FAJARDOYACEVEDO (1) |
| low | `PEREZ_AmparadoDeDios` | LICENCIADOROJAS | 38 | 15/38 (40%) | 3.92 | LICENCIADOROJAS (15), MESA (7), LOPEZDECARDENA (5), PAREDES (1), CUEVAYSILVA (1) |
| low | `RojasZorrillaFranciscode_Peligrarenlosremedios` | BATRES | 141 | 70/141 (50%) | 3.92 | BATRES (70), ROJASZORRILLA (7), CASTILLOSOLORZANO (6), QUINONES (3), ALARCON (3) |
| low | `COUTOPESTANA_ElSuenoEsVida` | BELMONTE | 47 | 20/47 (43%) | 3.91 | BELMONTE (20), LEIVARAMIREZ (7), GALLEGOS (7), BENAVIDES (5), JUANDESOTO (3) |
| low | `LosmartiresdeMadridydejarunreinoporotro2` | CASTROYSALAZAR | 65 | 23/65 (35%) | 3.90 | CASTROYSALAZAR (23), SANDOVAL (18), CUENCAYARGUELLO (4), MELO (2), ONAVIEDMAYTORRES (2) |
| low | `MiradeAmescuaAntonio_VidaymuertedeSanLazaro` | ROSETENINO | 127 | 49/127 (39%) | 3.89 | ROSETENINO (49), LEIVARAMIREZ (16), PAREDES (14), BELMONTE (7), VIDALYSALVADOR (6) |
| low | `LeonMerchanteoMarchanteJuanMan_PericonEl` | DAVILAYPALOMARES | 14 | 2/14 (14%) | 3.89 | DAVILAYPALOMARES (2), MARCHANTE (2), SANDOVAL (1) |
| low | `PabloPolopyValdesAtribuidoPedr_SitioysocorrodeVienaEl` | GARCIADEPRADO | 64 | 21/64 (33%) | 3.87 | GARCIADEPRADO (21), MORETO (21), LEIVARAMIREZ (4), QUINONES (2), GONZALEZDEBARCIA (1) |
| low | `AntoniodeZamora_Misticamonarquiaylasbodasdelco` | CAXESI | 35 | 8/35 (23%) | 3.87 | CAXESI (8), GARCIADEPRADO (6), ALARCON (3), ROJASVILLANDRANDO (2), ROSETENINO (2) |
| low | `CastroyBellvisGuillende_JusticiaenlapiedadLa` | TAMAYO | 65 | 21/65 (32%) | 3.86 | TAMAYO (21), MEDINA (14), SANTATERESA (7), MESA (6), CUEVAYSILVA (4) |
| low | `MEJIA_CERDA_PatriarcaPerseguido` | ENRIQUEZ | 59 | 29/59 (49%) | 3.85 | ENRIQUEZ (29), AVELLANEDA (10), CUEVAYSILVA (9), MEDINA (5), GARCIAMARCOS (4) |
| low | `LuisdeBelmonteBermudezAtribuid_RolloEl` | SANDOVAL | 16 | 4/16 (25%) | 3.85 | SANDOVAL (4) |
| low | `CristobaldeMoralesyGuerreroAtr_PeoresuntontoqueunrealdeaochoC` | RUANO | 91 | 41/91 (45%) | 3.83 | RUANO (41), CANIZARES (11), GONZALEZDEBARCIA (10), AVELLANEDADELACUEVA (3), LANINI (3) |
| low | `DamianSaluciodelPoyo_Reyperseguidoycoronapretendida` | CARVAJAL | 46 | 18/46 (39%) | 3.82 | CARVAJAL (18), SALAZARYTORRES (15), VARGAS (6), GONZALEZDEBARCIA (1), MESA (1) |
| low | `QuinonesdeBenaventeLuis_Despedidoyturrada` | ROMEROROQUE | 16 | 4/16 (25%) | 3.82 | ROMEROROQUE (4), FAJARDOYACEVEDO (2) |
| low | `VegaCarpioLopedeAtribuido_GatadeMariRamosLa` | MENESES | 37 | 13/37 (35%) | 3.81 | MENESES (13), CALDERON (4), MORETO (4), GARCIAMARCOS (2), ROSETENINO (2) |
| low | `TARREGA_Sangrelealdelasmontanesas_British` | GONZALEZDETORRES | 55 | 25/55 (46%) | 3.81 | GONZALEZDETORRES (25), HOZYMOTA (12), ROMEROROQUE (8), CASTILLOSOLORZANO (2), PAREDES (1) |
| low | `CristobaldeMoralesyGuerrero_DidoyEneas` | CARVAJAL | 50 | 16/50 (32%) | 3.79 | CARVAJAL (16), ROSETENINO (7), MESA (5), TORRESLORENZODE (3), QUINONES (2) |
| low | `CanizaresySuarezdeToledoJosede_Locurashayquedanjuicioyenganos` | CANIZARES | 55 | 16/55 (29%) | 3.78 | CANIZARES (16), CASTROYSALAZAR (14), GONZALEZDEBARCIA (8), GONGORA (4), LICENCIADOROJAS (1) |
| low | `DiegodeFigueroayCordobaJosedeF_Vencerseesmayorvalor` | LICENCIADOROJAS | 39 | 19/39 (49%) | 3.77 | LICENCIADOROJAS (19), CANIZARES (9), ROMEROROQUE (2), MORETO (1), GONZALEZDEBARCIA (1) |
| low | `Elsacristntarasca_Autografo` | MELO | 18 | 2/18 (11%) | 3.75 | MELO (2), CASTROYSALAZAR (2), ONAVIEDMAYTORRES (2), ROMEROROQUE (1), LANINI (1) |
| low | `FranciscodePaulaGonzalezdeBust_SantaOlalladeMerida` | ANDOSILLA | 63 | 20/63 (32%) | 3.75 | ANDOSILLA (20), ROJASZORRILLA (16), MORETO (10), CANIZARES (8), LEIVARAMIREZ (2) |
| low | `ElgranprincipedeFez` | JIMENEZSEDENO | 97 | 34/97 (35%) | 3.74 | JIMENEZSEDENO (34), PAREDES (20), CASTROYSALAZAR (20), AVELLANEDADELACUEVA (7), ROMEROROQUE (6) |
| low | `FranciscodeSoto_LoaparalafiestadeNuestraSenora` | ROSETENINO | 17 | 6/17 (35%) | 3.74 | ROSETENINO (6), LICENCIADOROJAS (1), ANDOSILLA (1) |
| low | `PedroFranciscodeLaniniySagredo_Labradorreyymonjeymejorreydelo` | CASTROYSALAZAR | 66 | 15/66 (23%) | 3.74 | CASTROYSALAZAR (15), ALARCON (10), RUANO (5), GONZALEZDEBARCIA (4), CASTILLOSOLORZANO (4) |
| low | `MiradeAmescuaAntonio_Loquepuedeeloirmisa` | CANIZARES | 26 | 11/26 (42%) | 3.74 | CANIZARES (11), GILENRIQUEZ (3), MORETO (3), CASTROYSALAZAR (2), ROJASZORRILLA (2) |
| low | `CansonerBaroc-BdC` | CALDERON | 593 | 254/593 (43%) | 3.73 | CALDERON (254), CONTRERAS (65), DIAMANTE (60), GILENRIQUEZ (37), CARVAJAL (34) |
| low | `JuanBautistadeVillegas_MentirosaverdadLa` | FAJARDOYACEVEDO | 54 | 24/54 (44%) | 3.72 | FAJARDOYACEVEDO (24), BELMONTE (8), BATRES (6), QUINONES (3), LICENCIADOROJAS (1) |
| low | `Colecciondevariaspoesiasv_1` | SANDOVAL | 329 | 116/329 (35%) | 3.72 | SANDOVAL (116), CASTROYSALAZAR (87), MELO (86), VARGASMACHUCA (10), LORENZANA (3) |
| low | `FranciscodelaTorreySevilJosede_AzucenadeEtiopia` | SANDOVAL | 28 | 7/28 (25%) | 3.72 | SANDOVAL (7), CASTROYSALAZAR (4), LANINI (3), GILENRIQUEZ (2), CARVAJAL (1) |
| low | `CastroyBellvisGuillende_Desenganodichoso` | RUIZALCEO | 49 | 13/49 (26%) | 3.72 | RUIZALCEO (13), SANDOVAL (9), ROMEROROQUE (4), CASTILLOSOLORZANO (3), MEDINA (3) |
| low | `VegaCarpioLopede_MontanesafamosaLaamistadpagada` | ROMEROROQUE | 49 | 11/49 (22%) | 3.67 | ROMEROROQUE (11), GOMEZACOSTA (8), CAXESI (7), ONAVIEDMAYTORRES (4), LORENZANA (2) |
| low | `Comopadreycomorey` | AVELLANEDADELACUEVA | 76 | 32/76 (42%) | 3.66 | AVELLANEDADELACUEVA (32), CALLE (11), QUINONES (10), ROMEROROQUE (4), SANDOVAL (2) |
| low | `LuisdeBelmonteBermudez_HortelanodeTordesillasEl` | ROJASZORRILLA | 50 | 17/50 (34%) | 3.65 | ROJASZORRILLA (17), BELMONTE (15), LOPEZDELCAMPO (7), ALARCON (1), TORRESLORENZODE (1) |
| low | `VelezdeGuevaraLuisAtribuido_ReymuertoEl` | PACHECO | 34 | 7/34 (21%) | 3.64 | PACHECO (7), MORETO (6), CANIZARES (4), TORRESLORENZODE (2), DAVILAYPALOMARES (2) |
| low | `VelezdeGuevaraLuis_CreaciondelmundoLa` | VALDIVIELSO | 51 | 21/51 (41%) | 3.63 | VALDIVIELSO (21), ROJASZORRILLA (8), AVELLANEDA (5), MESA (5), LICENCIADOROJAS (2) |
| low | `Elpleitodelmochuelo` | AGUADOELVIEJO | 15 | 5/15 (33%) | 3.62 | AGUADOELVIEJO (5), ANDOSILLA (1), CERVANTES (1) |
| low | `ElmariscaldeViron` | ENRIQUEZ | 55 | 14/55 (26%) | 3.62 | ENRIQUEZ (14), GARCIADEPRADO (8), ROJASZORRILLA (6), BELMONTE (6), QUEVEDO (4) |
| low | `GaspardeObregon_PerderparatenerEl` | ROJASZORRILLA | 62 | 14/62 (23%) | 3.62 | ROJASZORRILLA (14), CALDERON (11), BELMONTE (8), ALARCON (7), BATRES (3) |
| low | `VelezdeGuevaraLuis_HijosdelabarbudaLos` | LANINI | 84 | 29/84 (34%) | 3.60 | LANINI (29), PAREDES (26), SANDOVAL (5), MATOSFRAGOSO (2), ROMEROROQUE (1) |
| low | `HurtadodeMendozaAntonio_Cadalococonsutema` | RUIZALCEO | 60 | 24/60 (40%) | 3.60 | RUIZALCEO (24), GARCIAMARCOS (18), MEDINA (4), VARGAS (3), TORRESLORENZODE (3) |
| low | `VegaCarpioLopede_MarmoldeFelisardoEl` | AGUADOELVIEJO | 68 | 24/68 (35%) | 3.60 | AGUADOELVIEJO (24), MESA (18), QUINONES (9), CARVAJAL (2), LOPE (2) |
| low | `COUTOPESTANA_CamposElysiosDeAmor` | PAREDES | 46 | 15/46 (33%) | 3.60 | PAREDES (15), GOMEZACOSTA (11), TORRESLORENZODE (8), COELLO (4), CORDERO (2) |
| low | `LavidadeSanAnastasiofrailelegodelCarmen` | QUEVEDO | 21 | 7/21 (33%) | 3.60 | QUEVEDO (7), MONTALBAN (2), LOPE (2), BELMONTE (2), CONTRERAS (1) |
| low | `MarquesdeSanEstebantachadoAtri_DoslucerosdeOrienteLos` | LEIVARAMIREZ | 46 | 21/46 (46%) | 3.59 | LEIVARAMIREZ (21), GARCIAMARCOS (4), CASTILLOSOLORZANO (4), PAREDES (3), FAJARDOYACEVEDO (3) |
| low | `PoesiasVarias-II-1577` | GOMEZACOSTA | 173 | 29/173 (17%) | 3.59 | GOMEZACOSTA (29), GARCIAMARCOS (17), ROJASVILLANDRANDO (14), CASTILLOSOLORZANO (9), PAREDES (9) |
| low | `GodinezManriqueFelipe_Ludovicoelpiadoso` | SALAZARYTORRES | 75 | 17/75 (23%) | 3.59 | SALAZARYTORRES (17), TORRESLORENZODE (8), MEDINA (7), GRACIAN (6), ROMEROROQUE (5) |
| low | `JuanBautistaDiamante_VaquerodeGranadaEl` | LEIVARAMIREZ | 62 | 25/62 (40%) | 3.59 | LEIVARAMIREZ (25), FAJARDOYACEVEDO (9), CARVAJAL (8), CAXESI (3), GONZALEZDEBARCIA (1) |
| low | `AlfaroAlonso_VirgendelaSoledadLa` | LEIVARAMIREZ | 66 | 12/66 (18%) | 3.59 | LEIVARAMIREZ (12), BELMONTE (10), ROMEROROQUE (10), BATRES (5), CORDERO (5) |
| low | `VegaCarpioLopedeAtribuido_MayorhazanadeAlexandroMagnomay` | MORETO | 67 | 25/67 (37%) | 3.57 | MORETO (25), DIAMANTE (7), CALDERON (6), LOPEZDELCAMPO (4), GONZALEZDEBARCIA (2) |
| low | `AntonioFolchdeCardonaAlagon_Obrarcontrasuintencionytemplod` | MOLINAYMENDOZA | 62 | 18/62 (29%) | 3.57 | MOLINAYMENDOZA (18), BELMONTE (12), GALLEGOS (7), LEIVARAMIREZ (5), CASTROYSALAZAR (4) |
| low | `JosedeValdivielso_VillanoensurinconEl` | ROMEROROQUE | 37 | 15/37 (40%) | 3.57 | ROMEROROQUE (15), FAJARDOYACEVEDO (6), BELMONTE (4), LICENCIADOROJAS (1), ENRIQUEZ (1) |
| low | `BlasFernandezdeMesaAtribuidoTe_DonaBeatrizdeSilva` | BELMONTE | 58 | 16/58 (28%) | 3.57 | BELMONTE (16), LEIVARAMIREZ (10), ROSETENINO (5), ENRIQUEZ (4), JIMENEZSEDENO (3) |
| low | `CAIRASCODEFIGUEROA_Elalmaparaeldiadelcorpuschristi` | CECILIANACIMIENTO | 33 | 16/33 (48%) | 3.57 | CECILIANACIMIENTO (16), BENAVIDES (14), VARGASMACHUCA (3) |
| low | `VILLAIZAN_OfenderConLasFinezas` | CERVANTES | 16 | 6/16 (38%) | 3.56 | CERVANTES (6), CARVAJAL (4), HURTADODEMENDOZA (3), LORENZANA (2), MULSA (1) |
| low | `VARIOS_AutosSacramentalesCorte` | VIDALYSALVADOR | 358 | 111/358 (31%) | 3.54 | VIDALYSALVADOR (111), MORETO (53), TORRESLORENZODE (41), PAREDES (37), BANCESCANDAMO (25) |
| low | `RojasZorrillaFranciscode_PrimermarquesdeAstorgayfronter` | CARVAJAL | 60 | 10/60 (17%) | 3.53 | CARVAJAL (10), ROJASZORRILLA (8), CAXESI (6), GALLEGOS (5), GARCIADEPRADO (4) |
| low | `JUANDEQUIROS_Atribuido_ElRegistrador` | AVELLANEDADELACUEVA | 11 | 3/11 (27%) | 3.53 | AVELLANEDADELACUEVA (3), ROMEROROQUE (2), LEONORCUEVA (1), VARGASMACHUCA (1), FAJARDOYACEVEDO (1) |
| low | `VegaCarpioLopede_FrancesaLauraLa` | CONTRERAS | 66 | 14/66 (21%) | 3.52 | CONTRERAS (14), ALARCON (9), LEIVARAMIREZ (8), GALLEGOS (7), BATRES (5) |
| low | `DiegoRodriguezMontesinos_TrabajosdeAlaracheyavancedeGai` | GOMEZACOSTA | 33 | 12/33 (36%) | 3.50 | GOMEZACOSTA (12), LANINI (6), GONZALEZDETORRES (2), CONTRERAS (2), VARGASMACHUCA (1) |
| low | `QuinonesdeBenaventeLuis_NuecesLas` | GONGORA | 18 | 6/18 (33%) | 3.49 | GONGORA (6), CARVAJAL (1), MULSA (1), MELO (1) |
| low | `CARO_ElcondePartinuples` | BARRIONUEVO | 22 | 9/22 (41%) | 3.47 | BARRIONUEVO (9), CASTROYSALAZAR (2), LANINI (2), VERATASSIS (1), GILENRIQUEZ (1) |
| low | `ElcondePartinuples` | BARRIONUEVO | 22 | 9/22 (41%) | 3.47 | BARRIONUEVO (9), CASTROYSALAZAR (2), LANINI (2), VERATASSIS (1), GILENRIQUEZ (1) |
| low | `MoretoyCavanaAgustin_Trampaadelante` | ROJASZORRILLA | 64 | 20/64 (31%) | 3.45 | ROJASZORRILLA (20), ROSETENINO (9), CALDERON (8), LOPEZDELCAMPO (6), MORETO (3) |
| low | `MIRA_AnimalProfetaSanJulian2` | CALDERON | 65 | 16/65 (25%) | 3.45 | CALDERON (16), GARCIADEPRADO (12), GODINEZMANRIQUE (12), CASTILLOSOLORZANO (11), REMON (2) |
| low | `CubillodeAragonAlvaro_DesagraviosdeCristoLos` | GARCIAMARCOS | 67 | 29/67 (43%) | 3.44 | GARCIAMARCOS (29), SANDOVAL (15), MOLINAYMENDOZA (15), CAXESI (1), MIRACLESSOTOMAYOR (1) |
| low | `LuisdeBelmonteBermudez_CondedeFuentesenLisboaEl` | RUIZALCEO | 65 | 28/65 (43%) | 3.44 | RUIZALCEO (28), COELLO (12), MEDINA (7), QUINONES (2), DAVILAYPALOMARES (2) |
| low | `SoloenDioslaconfianza` | LEIVARAMIREZ | 61 | 13/61 (21%) | 3.44 | LEIVARAMIREZ (13), CALLE (11), MULSA (7), GARCIAMARCOS (6), VARGAS (5) |
| low | `GodinezManriqueFelipe_PastoresdeBelenAutosycoloquios` | COELLO | 37 | 16/37 (43%) | 3.43 | COELLO (16), PAREDES (10), GONZALEZDEBARCIA (1) |
| low | `MiradeAmescuaAntonio_CapitanBelisariooElejemplomayo` | GARCIADEPRADO | 56 | 13/56 (23%) | 3.41 | GARCIADEPRADO (13), ALARCON (7), SANDOVAL (6), PAREDES (3), BATRES (3) |
| low | `MIRA_AnimalProfetaSanJulian` | BATRES | 63 | 16/63 (25%) | 3.41 | BATRES (16), TAMAYO (11), CONTRERAS (8), CUEVAYSILVA (5), GRACIAN (2) |
| low | `JuanCrisostomoVelezdeGuevara_OlgonesLos` | CLARAMONTE | 16 | 4/16 (25%) | 3.39 | CLARAMONTE (4), LICENCIADOROJAS (1), HURTADODEMENDOZA (1), FBQUIROS (1), CARVAJAL (1) |
| low | `MoretoyCavanaAgustin_Industriacontrafinezas` | CLARAMONTE | 64 | 24/64 (38%) | 3.39 | CLARAMONTE (24), CAXESI (9), ANDOSILLA (5), LORENZANA (4), FBQUIROS (1) |
| low | `ARGUIJO_ObrasVariasPoeticas` | AVELLANEDA | 590 | 155/590 (26%) | 3.39 | AVELLANEDA (155), LICENCIADOROJAS (76), CORDERO (71), MESA (55), QUINONES (53) |
| low | `DamianSaluciodelPoyo_ProsperafortunadeRuyLopedeAval` | CARVAJAL | 53 | 8/53 (15%) | 3.39 | CARVAJAL (8), CASTILLOSOLORZANO (6), GONZALEZDEBARCIA (5), SARAVIAYMENDOZA (5), ROMEROROQUE (4) |
| low | `CASTROSALAZAR_Bobo` | CLARAMONTE | 8 | 2/8 (25%) | 3.38 | CLARAMONTE (2), GONGORA (1), LEIVARAMIREZ (1), ANDOSILLA (1) |
| low | `MALVEZZI_HistoriaDeEspana2` | CERVANTES | 154 | 65/154 (42%) | 3.38 | CERVANTES (65), BANCESCANDAMO (43), ENRIQUEZ (34), CECILIANACIMIENTO (10), VIDALYSALVADOR (1) |
| low | `VegaCarpioLopede_PuentedelmundoLa` | TAMAYO | 26 | 9/26 (35%) | 3.37 | TAMAYO (9), TORRESLORENZODE (7), MESA (2), ANDOSILLA (1) |
| low | `LaVirgendelPilar` | FAJARDOYACEVEDO | 70 | 17/70 (24%) | 3.37 | FAJARDOYACEVEDO (17), CASTILLOSOLORZANO (16), CALLE (8), ALARCON (5), CARVAJAL (3) |
| low | `LEON_Melchor_Vidagrantacano_Novena` | LEIVARAMIREZ | 55 | 24/55 (44%) | 3.37 | LEIVARAMIREZ (24), GARCIADEPRADO (9), MOLINAYMENDOZA (6), MENESES (5), BELMONTE (2) |
| low | `LoquevadelhombreaDios2` | MELO | 73 | 36/73 (49%) | 3.35 | MELO (36), AVELLANEDA (18), VARGASMACHUCA (3), TORRESLORENZODE (2), PAREDES (2) |
| low | `PedroAlvarezdeAyllonLuisHurtad_Tibalda` | SANTATERESA | 499 | 211/499 (42%) | 3.35 | SANTATERESA (211), LICENCIADOROJAS (112), CUEVAYSILVA (66), AVELLANEDA (31), CECILIANACIMIENTO (30) |
| low | `AntonioEnriquezGomez_NoblesiempreesvalienteEl` | QUEVEDO | 105 | 30/105 (29%) | 3.35 | QUEVEDO (30), MESA (17), BATRES (14), ENRIQUEZ (10), LEIVARAMIREZ (10) |
| low | `MELBURY_2` | SANDOVAL | 1000 | 193/1000 (19%) | 3.35 | SANDOVAL (193), GONGORA (153), SARAVIAYMENDOZA (110), VERATASSIS (108), LICENCIADOROJAS (99) |
| low | `Fierasafeminaamor` | SANDOVAL | 136 | 56/136 (41%) | 3.32 | SANDOVAL (56), VERATASSIS (48), GARCIAMARCOS (10), PAREDES (7), MONTALBAN (3) |
| low | `MIRA_ArpaDeDavid` | SANTATERESA | 72 | 11/72 (15%) | 3.32 | SANTATERESA (11), ROMEROROQUE (9), SANDOVAL (7), CLARAMONTE (5), TORRESLORENZODE (5) |
| low | `AntoniodeZamora_DonDomingodedonBlas` | LANINI | 90 | 33/90 (37%) | 3.32 | LANINI (33), GARCIADEPRADO (23), VIDALYSALVADOR (7), MOLINAYMENDOZA (7), LEIVARAMIREZ (2) |
| low | `ClaramonteAndresde_TaodeSanAntonEl` | BATRES | 69 | 20/69 (29%) | 3.31 | BATRES (20), SANDOVAL (12), LEIVARAMIREZ (8), CASTILLOSOLORZANO (5), CUEVAYSILVA (3) |
| low | `MELBURY_1` | MORETO | 968 | 151/968 (16%) | 3.31 | MORETO (151), CASTROYSALAZAR (74), SANDOVAL (66), ZABALETA (65), VILLEGASDELACRUZ (52) |
| low | `Extremosdeamorydehonor` | ROMEROROQUE | 32 | 14/32 (44%) | 3.31 | ROMEROROQUE (14), GARCIAMARCOS (5), GODINEZMANRIQUE (4), AVELLANEDADELACUEVA (3), CALLE (1) |
| low | `GuerreroAdrian_IgnorantediscretoEl` | HOZYMOTA | 66 | 18/66 (27%) | 3.31 | HOZYMOTA (18), ALARCON (16), GARCIADEPRADO (10), MOLINAYMENDOZA (5), CAXESI (3) |
| low | `VegaCarpioLopede_DamabobaLa` | CALLE | 145 | 53/145 (37%) | 3.30 | CALLE (53), LEIVARAMIREZ (43), GARCIAMARCOS (8), CASTILLOSOLORZANO (6), SANDOVAL (3) |
| low | `VegaCarpioLopedeAtribuido_HermanoFranciscodeAlcalaEl` | CASTILLOSOLORZANO | 48 | 11/48 (23%) | 3.30 | CASTILLOSOLORZANO (11), MESA (6), VALDIVIELSO (4), BATRES (2), QUINONES (2) |
| low | `VegaCarpioLopedeAtribuido_Mayordichaenelmonteylagloriaen` | BELMONTE | 64 | 18/64 (28%) | 3.29 | BELMONTE (18), CALDERON (8), MEDINA (7), DAVILAYPALOMARES (7), ROJASVILLANDRANDO (6) |
| low | `ROJO_JacaraConLaGlosaDeDoceJacaras_Autografo` | BELMONTE | 13 | 2/13 (15%) | 3.29 | BELMONTE (2), FAJARDOYACEVEDO (1) |
| low | `JuanCoelloAriasAntonioCoelloyO_DosFernandodeAustriaLos` | FAJARDOYACEVEDO | 71 | 24/71 (34%) | 3.28 | FAJARDOYACEVEDO (24), ALARCON (15), ANDOSILLA (10), GARCIADEPRADO (8), AVELLANEDADELACUEVA (2) |
| low | `Elrigorenlainocencia` | CASTROYSALAZAR | 26 | 7/26 (27%) | 3.25 | CASTROYSALAZAR (7), LOPEZDECASTRO (3), GOMEZACOSTA (2), ONAVIEDMAYTORRES (2), BARRIONUEVO (2) |
| low | `JuanCrisostomoVelezdeGuevaraJe_SieteinfantesdeLaraLos` | CALLE | 34 | 9/34 (26%) | 3.25 | CALLE (9), LEIVARAMIREZ (6), ROMEROROQUE (3), FAJARDOYACEVEDO (2), GARCIAMARCOS (2) |
| low | `FONTANELLA_poesia` | ENRIQUEZ | 183 | 72/183 (39%) | 3.23 | ENRIQUEZ (72), GARCIADEPRADO (19), CONTRERAS (18), VIDALYSALVADOR (17), CECILIANACIMIENTO (16) |
| low | `VegaCarpioLopede_MudanzasdefortunaSucesosdedBel` | MESA | 51 | 14/51 (28%) | 3.23 | MESA (14), DIAMANTE (13), LOPEZDECARDENA (6), LOPEZDELCAMPO (3), VIDALYSALVADOR (2) |
| low | `PedroRoseteNino_SantaCatalinamartirydoctora` | GARCIADEPRADO | 68 | 31/68 (46%) | 3.20 | GARCIADEPRADO (31), GILENRIQUEZ (9), CALDERON (9), SARAVIAYMENDOZA (4), MORETO (3) |
| low | `JuanBautistaDiamanteMatosFrago_Reinarporobedecer` | BELMONTE | 56 | 9/56 (16%) | 3.17 | BELMONTE (9), LEIVARAMIREZ (8), ALARCON (7), QUINONES (7), CUENCAYARGUELLO (3) |
| low | `SebastianMunoz_TeatrosdeDianaLos` | PAREDES | 94 | 43/94 (46%) | 3.15 | PAREDES (43), TAMAYO (10), TORRESLORENZODE (6), COELLO (5), VARGAS (4) |
| low | `VegaCarpioLopede_Hermosuraaborrecidaydesdichada` | TORRESLORENZODE | 56 | 19/56 (34%) | 3.15 | TORRESLORENZODE (19), PACHECO (12), LICENCIADOROJAS (11), LANINI (2), GONZALEZDEBARCIA (2) |
| low | `ElcaballerodelFebo2` | BELMONTE | 35 | 15/35 (43%) | 3.15 | BELMONTE (15), QUEVEDO (6), LEIVARAMIREZ (5), ROJASZORRILLA (4), LICENCIADOROJAS (1) |
| low | `CARO_Valoragravio1` | PAREDES | 58 | 21/58 (36%) | 3.13 | PAREDES (21), FAJARDOYACEVEDO (12), GONZALEZDEBARCIA (10), AVELLANEDADELACUEVA (3), HURTADODEMENDOZA (1) |
| low | `MallenSotoAnaCarode_Valoragravioymujer` | PAREDES | 58 | 21/58 (36%) | 3.13 | PAREDES (21), FAJARDOYACEVEDO (12), GONZALEZDEBARCIA (10), AVELLANEDADELACUEVA (3), HURTADODEMENDOZA (1) |
| low | `VARIOS_Entremeses2` | FAJARDOYACEVEDO | 111 | 15/111 (14%) | 3.13 | FAJARDOYACEVEDO (15), MELO (13), GARCIADEPRADO (10), LANINI (9), MOLINAYMENDOZA (8) |
| low | `MIRADEAMESCUA_MuerteDelPrincipeDeOrange` | BATRES | 106 | 49/106 (46%) | 3.13 | BATRES (49), LEIVARAMIREZ (32), VIDALYSALVADOR (7), GARCIADEPRADO (5), AMESCUA (2) |
| low | `TellezGabrielGodinezManriqueFe_FuerzadeTamarLa` | MENESES | 48 | 14/48 (29%) | 3.13 | MENESES (14), LEIVARAMIREZ (14), ROSETENINO (4), BELMONTE (3), VILLEGASJUANBAUTISTA (2) |
| low | `AntoniodeZamora_GitanillaLa` | LLOBREGATYESTEVE | 11 | 5/11 (46%) | 3.13 | LLOBREGATYESTEVE (5), PAREDES (1), CONTRERAS (1), LORENZANA (1) |
| low | `B2605_nos.1-2` | MARCHANTE | 42 | 16/42 (38%) | 3.12 | MARCHANTE (16), VIDALYSALVADOR (11), QUEVEDO (8), GILENRIQUEZ (6), HOZYMOTA (1) |
| low | `JoseGarces_MasdichosoensupatriaSanRaimund` | GILENRIQUEZ | 61 | 18/61 (30%) | 3.11 | GILENRIQUEZ (18), VERATASSIS (10), DAVILAYPALOMARES (9), SANDOVAL (5), LANINI (3) |
| low | `QuirosJuande_FamosatoledanaLa` | MEDINA | 154 | 76/154 (49%) | 3.10 | MEDINA (76), LOPEZDECASTRO (52), AVELLANEDA (10), LORENZANA (1), HURTADODEMENDOZA (1) |
| low | `VegaCarpioLopedeAtribuido_Melisendra` | VELEZ | 49 | 16/49 (33%) | 3.10 | VELEZ (16), VIDALYSALVADOR (6), BATRES (1), AMESCUA (1), HURTADODEMENDOZA (1) |
| low | `Obligadosyofendidos` | LEIVARAMIREZ | 74 | 29/74 (39%) | 3.08 | LEIVARAMIREZ (29), BELMONTE (12), GALLEGOS (8), FAJARDOYACEVEDO (4), SANDOVAL (4) |
| low | `Variosautores_Comediasloasjacarasysainetessu` | SANDOVAL | 328 | 62/328 (19%) | 3.07 | SANDOVAL (62), VIDALYSALVADOR (60), LANINI (39), PAREDES (35), ONAVIEDMAYTORRES (21) |
| low | `VegaCarpioLopede_Verynocreer` | SANDOVAL | 77 | 22/77 (29%) | 3.07 | SANDOVAL (22), ROMEROROQUE (10), FAJARDOYACEVEDO (7), ALARCON (5), VARGASMACHUCA (4) |
| low | `PEREZDEARAGON_Atribuido_LoaParaElDiaDeLaCircuncisionDelSenor` | CERVANTES | 4 | 1/4 (25%) | 3.07 | CERVANTES (1), SANDOVAL (1), TORRESLORENZODE (1), MELO (1) |
| low | `VegaCarpioLopedeAtribuidoVelez_NinodiabloPrimeraparteEl` | MOLINAYMENDOZA | 40 | 10/40 (25%) | 3.06 | MOLINAYMENDOZA (10), GILENRIQUEZ (8), SANDOVAL (5), VERATASSIS (3), VIDALYSALVADOR (2) |
| low | `LuisdeBelmonteBermudez_MayorcontrarioamigoEldemoniopo` | TORRESLORENZODE | 54 | 11/54 (20%) | 3.05 | TORRESLORENZODE (11), ROMEROROQUE (8), CANIZARES (8), SANDOVAL (7), FAJARDOYACEVEDO (4) |
| low | `JuanSalvo_VizcondezaCubielosylabodaLa` | GONZALEZDEBARCIA | 14 | 4/14 (29%) | 3.04 | GONZALEZDEBARCIA (4), LICENCIADOROJAS (1), CERVANTES (1), CASTILLOSOLORZANO (1) |
| low | `TellezGabrielAtribuidoBlasFern_Milagroporloscelosyexcelentepo` | CALLE | 60 | 12/60 (20%) | 3.04 | CALLE (12), ALARCON (12), LEIVARAMIREZ (6), VILLEGASJUANBAUTISTA (4), CASTILLOSOLORZANO (3) |
| low | `GONZALEZ_BUSTOS_MosqueteroenFlandes` | CASTROYSALAZAR | 54 | 25/54 (46%) | 3.03 | CASTROYSALAZAR (25), VIDALYSALVADOR (9), BANCESCANDAMO (7), CANIZARES (6), GONZALEZDEBARCIA (4) |
| low | `SimondeSanmateo_DonaJimenaGomez` | SANDOVAL | 22 | 9/22 (41%) | 3.03 | SANDOVAL (9), FAJARDOYACEVEDO (2), LICENCIADOROJAS (1), CASTILLOSOLORZANO (1) |
| low | `PusosemeelsolsaliomelalunaSantaTeodora` | CALLE | 69 | 33/69 (48%) | 3.02 | CALLE (33), TAMAYO (10), QUINONES (4), LEIVARAMIREZ (4), GARCIAMARCOS (2) |
| low | `LosmejoresperegrinosyJerusalnsitiadaautoalegrico` | ENRIQUEZ | 57 | 24/57 (42%) | 3.02 | ENRIQUEZ (24), ALARCON (14), GARCIADEPRADO (6), PAREDES (2), VIDALYSALVADOR (1) |
| low | `ReyDonPedro-FirmezaAmor_Fragmentos` | LICENCIADOROJAS | 7 | 2/7 (29%) | 3.01 | LICENCIADOROJAS (2), CERVANTES (2), GONGORA (2), SANDOVAL (1) |
| low | `MONTESER_Entremeses` | VARGASMACHUCA | 24 | 8/24 (33%) | 3.00 | VARGASMACHUCA (8), MELO (2), GONZALEZDEBARCIA (1), CECILIANACIMIENTO (1), JIMENEZSEDENO (1) |
| low | `ArcedelosReyesAmbriosio_CegarparavermejorsantaLucia` | LEIVARAMIREZ | 103 | 25/103 (24%) | 2.99 | LEIVARAMIREZ (25), FAJARDOYACEVEDO (20), AVELLANEDADELACUEVA (14), CALLE (9), MORETO (6) |
| low | `VARIOS_ComediasTragediasMexicanasBnF` | LANINI | 222 | 55/222 (25%) | 2.99 | LANINI (55), LORENZANA (53), GONZALEZDETORRES (29), LOPEZDECASTRO (16), CASTROYSALAZAR (11) |
| low | `PONCE_PremiarElMayorAgravio_Autografo` | VIDALYSALVADOR | 196 | 161/196 (82%) | 2.98 | VIDALYSALVADOR (161), VERATASSIS (5), CASTROYSALAZAR (5), MARCHANTE (4), CALDERON (2) |
| low | `Poesiascastellanasvarias_v5` | LOPEZDECASTRO | 336 | 29/336 (9%) | 2.98 | LOPEZDECASTRO (29), CASTILLOSOLORZANO (29), LORENZANA (27), GALLEGOS (25), AVELLANEDA (22) |
| low | `CristobaldeMonroyySilva_Nohayamordondenohaycelos` | ROJASZORRILLA | 57 | 14/57 (25%) | 2.97 | ROJASZORRILLA (14), ROSETENINO (8), BELMONTE (7), CAXESI (5), MONTALBAN (2) |
| low | `FranciscodeSoto_VidaymuertedeSanBlas` | SANDOVAL | 61 | 27/61 (44%) | 2.97 | SANDOVAL (27), MEDINA (10), LANINI (3), BELMONTE (2), PAREDES (2) |
| low | `CastroyBellvisGuillende_TragediaporloscelosLa` | CLARAMONTE | 131 | 70/131 (53%) | 2.96 | CLARAMONTE (70), JUANDESOTO (13), ANDOSILLA (3), MIRACLESSOTOMAYOR (2), MESA (2) |
| low | `MallenSotoAnaCarode_CondePartinuplesEl` | GONZALEZDEBARCIA | 52 | 33/52 (64%) | 2.96 | GONZALEZDEBARCIA (33), MULSA (2), CORDERO (2), DIAMANTE (2), HURTADODEMENDOZA (1) |
| low | `MarceloAntoniodeAyalayGuzman_RestauraciondeHungriaSegundapa` | LOPEZDELCAMPO | 80 | 36/80 (45%) | 2.96 | LOPEZDELCAMPO (36), GARCIADEPRADO (19), LEONORCUEVA (7), VIDALYSALVADOR (4), ZABALETA (3) |
| low | `ArboredaAlejandro_CatolicoPerseosanJorgeoElmarti` | FAJARDOYACEVEDO | 75 | 11/75 (15%) | 2.95 | FAJARDOYACEVEDO (11), MOLINAYMENDOZA (11), JIMENEZSEDENO (10), GARCIAMARCOS (8), CASTILLOSOLORZANO (7) |
| low | `ValdivielsoJosede_EscueladivinaAutosacramentalLa` | AGUADOELVIEJO | 40 | 20/40 (50%) | 2.95 | AGUADOELVIEJO (20), QUINONES (10), CARVAJAL (1), BELMONTE (1) |
| low | `QUINONESDEBENAVENTE_JuegoDeManos` | BELMONTE | 14 | 5/14 (36%) | 2.94 | BELMONTE (5), LEIVARAMIREZ (5) |
| low | `BANCES_AustriaEnJerusalen2` | CASTROYSALAZAR | 65 | 13/65 (20%) | 2.94 | CASTROYSALAZAR (13), SANDOVAL (13), GILENRIQUEZ (12), MARCHANTE (9), VERATASSIS (3) |
| low | `CastroyBellvisGuillendeAtribui_Canasenelpapelydudosoenlavenga` | LEIVARAMIREZ | 64 | 15/64 (23%) | 2.93 | LEIVARAMIREZ (15), BATRES (8), ALARCON (7), FAJARDOYACEVEDO (7), TORRESLORENZODE (5) |
| low | `Papelesvariosgongorinos_8` | LOPEZDECASTRO | 100 | 66/100 (66%) | 2.92 | LOPEZDECASTRO (66), GONZALEZDETORRES (16), LOPEZJACINTO (5), ROMEROROQUE (4), CALLE (3) |
| low | `LuisdeMargaritAtribuido_Estaesfarsahechaamaneradevisit` | AVELLANEDA | 759 | 661/759 (87%) | 2.92 | AVELLANEDA (661), VIDALYSALVADOR (6), LOPEZDECASTRO (6), VARGASMACHUCA (5), LOPE (2) |
| low | `PabloPolopyValdes_PerfeccioneseldesdenZarzuela` | QUINONES | 55 | 25/55 (46%) | 2.91 | QUINONES (25), CALDERON (6), LICENCIADOROJAS (4), AGUADOELVIEJO (4), CARVAJAL (1) |
| low | `MatosFragosoJuande_HijodelapiedraEl` | BELMONTE | 131 | 27/131 (21%) | 2.91 | BELMONTE (27), BATRES (17), CALLE (17), VERATASSIS (8), GILENRIQUEZ (8) |
| low | `JosedeValdivielso_LocosantoEllococuerdoEllocodel` | ANDOSILLA | 66 | 35/66 (53%) | 2.91 | ANDOSILLA (35), JUANDESOTO (9), SALAZARYTORRES (7), GALLEGOS (3), VARGAS (1) |
| low | `ESCOBAR_FavoresSantos` | VARGASMACHUCA | 435 | 42/435 (10%) | 2.90 | VARGASMACHUCA (42), HURTADODEMENDOZA (41), CLARAMONTE (31), CUEVAYSILVA (30), ROJASZORRILLA (21) |
| low | `Nohaycontraelhonorpoder` | MOLINAYMENDOZA | 36 | 9/36 (25%) | 2.89 | MOLINAYMENDOZA (9), LANINI (7), ENRIQUEZ (3), VERATASSIS (2), GARCIAMARCOS (2) |
| low | `MARIADOCEU_EscarmentosdeFlores` | MOLINAYMENDOZA | 14 | 4/14 (29%) | 2.89 | MOLINAYMENDOZA (4), VIDALYSALVADOR (1), LANINI (1), PAREDES (1), BELMONTE (1) |
| low | `FranciscoAntoniodeBancesCandam_EspanolmasamanteydesgraciadoMa` | ROSETENINO | 52 | 25/52 (48%) | 2.88 | ROSETENINO (25), HOZYMOTA (11), CANIZARES (3), MULSA (1), GONZALEZDEBARCIA (1) |
| low | `VegaCarpioLopede_SantoNinodelaGuardiaSegundoCri` | GARCIAMARCOS | 67 | 26/67 (39%) | 2.87 | GARCIAMARCOS (26), CALLE (6), LEIVARAMIREZ (5), FAJARDOYACEVEDO (5), MOLINAYMENDOZA (5) |
| low | `AntonioBarrientos_BeatasLas` | MOLINAYMENDOZA | 34 | 15/34 (44%) | 2.86 | MOLINAYMENDOZA (15), FAJARDOYACEVEDO (9), CARVAJAL (1), QUINONES (1), BELMONTE (1) |
| low | `OlivaresVadilloSebastiande_MurosdeJericoLos` | SANDOVAL | 65 | 22/65 (34%) | 2.86 | SANDOVAL (22), SARAVIAYMENDOZA (20), CASTROYSALAZAR (5), FAJARDOYACEVEDO (2), ENRIQUEZ (2) |
| low | `AutossacramentalesTomosegundo` | GONZALEZDEBARCIA | 408 | 128/408 (31%) | 2.86 | GONZALEZDEBARCIA (128), GARCIAMARCOS (71), ROMEROROQUE (53), PAREDES (39), SANDOVAL (31) |
| low | `VegaCarpioLopedeAtribuido_ValordeMaltaEl` | CUEVAYSILVA | 65 | 33/65 (51%) | 2.86 | CUEVAYSILVA (33), RUIZALCEO (21), TAMAYO (3), MULSA (2), REMON (1) |
| low | `TellezGabriel_MujerquemandaencasaytiranadeIs` | CANIZARES | 29 | 6/29 (21%) | 2.86 | CANIZARES (6), CLARAMONTE (5), MORETO (4), ROJASZORRILLA (3), SANDOVAL (3) |
| low | `BOCANGELYUNZUETA_NuevoOlimpoEl` | LOPEZDECASTRO | 86 | 40/86 (46%) | 2.85 | LOPEZDECASTRO (40), GONZALEZDETORRES (17), LORENZANA (6), JUANDESOTO (6), LANINI (4) |
| low | `TellezGabriel_QuinasdePortugalLas` | PAREDES | 123 | 31/123 (25%) | 2.83 | PAREDES (31), CALLE (29), GONZALEZDETORRES (13), GARCIAMARCOS (13), JIMENEZSEDENO (13) |
| low | `CubillodeAragonAlvaro_InvisibleprincipedelbaulEl` | ROMEROROQUE | 69 | 27/69 (39%) | 2.83 | ROMEROROQUE (27), ONAVIEDMAYTORRES (12), SANDOVAL (9), MELO (5), FAJARDOYACEVEDO (4) |
| low | `VelezdeGuevaraLuis_MesaredondaLa` | CONTRERAS | 40 | 11/40 (28%) | 2.82 | CONTRERAS (11), QUINONES (9), CARVAJAL (6), HURTADODEMENDOZA (5) |
| low | `RomanMonterodeEspinosa_CupidoyVenusmaestrosdeescuela` | TORRESLORENZODE | 14 | 3/14 (21%) | 2.81 | TORRESLORENZODE (3), CASTILLOSOLORZANO (1), ALARCON (1), JIMENEZSEDENO (1), AMESCUA (1) |
| low | `TellezGabriel_CelosoprudenteEl` | COELLO | 68 | 25/68 (37%) | 2.80 | COELLO (25), LEIVARAMIREZ (16), ONAVIEDMAYTORRES (5), ENRIQUEZ (4), TORRESLORENZODE (2) |
| low | `JoseAntonioGarciadePrado_PachecosyPalomequesoLosbandosd` | VIDALYSALVADOR | 132 | 100/132 (76%) | 2.79 | VIDALYSALVADOR (100), VERATASSIS (8), MORETO (6), LEIVARAMIREZ (3), GILENRIQUEZ (2) |
| low | `JuanPerezdeMontalban_PuertaMacarenaPrimeraparteLa` | QUINONES | 222 | 95/222 (43%) | 2.79 | QUINONES (95), GARCIADEPRADO (32), CALDERON (26), CONTRERAS (15), CASTILLOSOLORZANO (5) |
| low | `ARMENDARIZ_Burlasveras_Parma` | GARCIADEPRADO | 45 | 12/45 (27%) | 2.79 | GARCIADEPRADO (12), CALDERON (10), LEIVARAMIREZ (5), ROJASZORRILLA (4), LOPE (3) |
| low | `BERMUDEZCALDERON_DosAmantesCelosos_British` | VERATASSIS | 57 | 28/57 (49%) | 2.78 | VERATASSIS (28), LOPEZDECARDENA (22), LEONORCUEVA (2), GOMEZACOSTA (2), LANINI (1) |
| low | `Papelesvariosgongorinos_5` | SARAVIAYMENDOZA | 100 | 33/100 (33%) | 2.78 | SARAVIAYMENDOZA (33), TAMAYO (17), AVELLANEDADELACUEVA (13), MULSA (13), GRACIAN (12) |
| low | `ElcondedeSex` | LOPEZDELCAMPO | 75 | 20/75 (27%) | 2.78 | LOPEZDELCAMPO (20), BELMONTE (16), ENRIQUEZ (12), CALDERON (7), VIDALYSALVADOR (7) |
| low | `Lamalcontenta` | MOLINAYMENDOZA | 14 | 3/14 (21%) | 2.78 | MOLINAYMENDOZA (3), JIMENEZSEDENO (1), ALARCON (1) |
| low | `JuanBautistaDiamante_JuanSanchezdeTalavera` | AVELLANEDA | 72 | 33/72 (46%) | 2.76 | AVELLANEDA (33), LANINI (27), VERATASSIS (3), MESA (2), CUEVAYSILVA (1) |
| low | `RojasZorrillaFranciscode_LoquequeriaverelmarquesdeVille` | VERATASSIS | 254 | 107/254 (42%) | 2.76 | VERATASSIS (107), VIDALYSALVADOR (101), PAREDES (24), GONGORA (5), AVELLANEDA (4) |
| low | `JuanHidalgo_NinoDiosenEgiptoyelmasdichosol` | GARCIAMARCOS | 39 | 10/39 (26%) | 2.76 | GARCIAMARCOS (10), GOMEZACOSTA (7), MELO (4), VARGASMACHUCA (4), VERATASSIS (2) |
| low | `VegaCarpioLopede_BurgalesadeLermaLa` | ANDOSILLA | 72 | 34/72 (47%) | 2.76 | ANDOSILLA (34), LEIVARAMIREZ (9), BELMONTE (8), TORRESLORENZODE (6), MESA (2) |
| low | `MONTESER_Manzana` | VIDALYSALVADOR | 22 | 15/22 (68%) | 2.75 | VIDALYSALVADOR (15), PAREDES (2), GARCIADEPRADO (1), DIAMANTE (1) |
| low | `Ladespreciadaquerida` | BELMONTE | 104 | 57/104 (55%) | 2.75 | BELMONTE (57), LEIVARAMIREZ (28), MESA (4), BATRES (2), PAREDES (1) |
| low | `MIRADEAMESCUA_ProdigiosdelavaraLos_British` | CASTROYSALAZAR | 144 | 34/144 (24%) | 2.75 | CASTROYSALAZAR (34), FAJARDOYACEVEDO (26), SANDOVAL (20), MELO (15), AVELLANEDADELACUEVA (15) |
| low | `MonterodeEspinosaRoman_MiliciaLa` | PAREDES | 16 | 5/16 (31%) | 2.75 | PAREDES (5), GARCIAMARCOS (2), BANCESCANDAMO (1), CASTILLOSOLORZANO (1), VIDALYSALVADOR (1) |
| low | `VILLAMEDIANA_Obras` | VARGASMACHUCA | 138 | 71/138 (51%) | 2.74 | VARGASMACHUCA (71), MELO (49), ROMEROROQUE (8), LICENCIADOROJAS (1), CERVANTES (1) |
| low | `RojasZorrillaFranciscode_PleitodeldemonioconlaVirgenEl` | CALDERON | 103 | 35/103 (34%) | 2.74 | CALDERON (35), GARCIADEPRADO (20), ALARCON (20), CONTRERAS (5), VIDALYSALVADOR (4) |
| low | `JuandeCigorondo_ComediaalagloriosaMagdalenaLos` | RUIZALCEO | 392 | 108/392 (28%) | 2.74 | RUIZALCEO (108), CUEVAYSILVA (74), CORDERO (64), GOMEZACOSTA (30), ENRIQUEZ (23) |
| low | `PERALTA_AfectosVencenFinezas_British` | SANDOVAL | 185 | 90/185 (49%) | 2.74 | SANDOVAL (90), CASTROYSALAZAR (64), MELO (10), CANIZARES (6), GILENRIQUEZ (3) |
| low | `Elmayorcontrarioamigo` | MULSA | 56 | 12/56 (21%) | 2.74 | MULSA (12), CANIZARES (8), MORETO (8), ROSETENINO (6), AGUADOELVIEJO (4) |
| low | `Elsastredelcampillo` | GONZALEZDEBARCIA | 54 | 20/54 (37%) | 2.73 | GONZALEZDEBARCIA (20), CANIZARES (15), CASTILLOSOLORZANO (5), CAXESI (4), CASTROYSALAZAR (1) |
| low | `VegaCarpioLopedeAtribuido_PalomadeToledoLa` | FAJARDOYACEVEDO | 64 | 36/64 (56%) | 2.73 | FAJARDOYACEVEDO (36), CALLE (5), LEIVARAMIREZ (4), GARCIAMARCOS (3), LICENCIADOROJAS (1) |
| low | `MiradeAmescuaAntonioAtribuido_Obligarcontrasusangre` | CASTILLOSOLORZANO | 56 | 20/56 (36%) | 2.72 | CASTILLOSOLORZANO (20), BATRES (20), GARCIADEPRADO (12), BELMONTE (1) |
| low | `DiegoPablodeVelasco_SanAtilano` | ENRIQUEZ | 90 | 28/90 (31%) | 2.72 | ENRIQUEZ (28), BELMONTE (19), CASTILLOSOLORZANO (12), CALLE (7), MONTALBAN (4) |
| low | `BERMUDEZ_PrimerasTragediasEspanolas` | SANDOVAL | 263 | 136/263 (52%) | 2.72 | SANDOVAL (136), AVELLANEDA (87), LEONORCUEVA (18), CASTILLOSOLORZANO (2), VIDALYSALVADOR (2) |
| low | `TellezGabriel_PrivarcontrasugustoElprivadopo` | LEIVARAMIREZ | 74 | 34/74 (46%) | 2.72 | LEIVARAMIREZ (34), BATRES (8), CALLE (6), FAJARDOYACEVEDO (5), GARCIAMARCOS (3) |
| low | `AntonioEnriquezGomez_Margaritadeloscielosymasfirmep` | CASTILLOSOLORZANO | 52 | 27/52 (52%) | 2.72 | CASTILLOSOLORZANO (27), VIDALYSALVADOR (6), LANINI (5), HURTADODEMENDOZA (1), HOZYMOTA (1) |
| low | `BERMUDEZCALDERON_AmorDesprecio_British` | LOPEZDECARDENA | 93 | 65/93 (70%) | 2.71 | LOPEZDECARDENA (65), VERATASSIS (21), DAVILAYPALOMARES (4), QUEVEDO (1), SANDOVAL (1) |
| low | `RojasZorrillaFranciscodeAtribu_JerusalencastigadaporVespasian` | PACHECO | 48 | 24/48 (50%) | 2.71 | PACHECO (24), MEDINA (3), TORRESLORENZODE (3), RUIZALCEO (2), CUEVAYSILVA (2) |
| low | `ENRIQUEZGOMEZ_GranMedicoYPintor` | AMESCUA | 106 | 66/106 (62%) | 2.71 | AMESCUA (66), MATOSFRAGOSO (7), DIAMANTE (5), VIDALYSALVADOR (4), HOZYMOTA (3) |
| low | `CerveroCrescencio_Extremosdeamoryhonor` | GONGORA | 36 | 17/36 (47%) | 2.70 | GONGORA (17), AVELLANEDADELACUEVA (3), FAJARDOYACEVEDO (2), ROMEROROQUE (2), HURTADODEMENDOZA (1) |
| low | `FrancisodeAvellanedadelaCuevay_PrimeroustedElsargentoGanchill` | BOLEAYALVARADO | 15 | 3/15 (20%) | 2.70 | BOLEAYALVARADO (3), GONZALEZDETORRES (2), VIDALYSALVADOR (1), CUENCAYARGUELLO (1) |
| low | `AntoniodeZamora_GigantonesLos` | MOLINAYMENDOZA | 10 | 3/10 (30%) | 2.70 | MOLINAYMENDOZA (3), CASTROYSALAZAR (2), GONZALEZDEBARCIA (1), CANIZARES (1) |
| low | `DiegoJuandeVeraTassisyVillarro_Sinarmasvenceelamoroelmayortri` | FAJARDOYACEVEDO | 76 | 23/76 (30%) | 2.70 | FAJARDOYACEVEDO (23), MOLINAYMENDOZA (22), CASTROYSALAZAR (5), ROMEROROQUE (5), JIMENEZSEDENO (3) |
| low | `VIDAL_AlamedaDeValenciaYConfusionDeUnPaseo` | ENRIQUEZ | 156 | 46/156 (30%) | 2.67 | ENRIQUEZ (46), VIDALYSALVADOR (44), CERVANTES (42), LOPEZDECARDENA (5), LICENCIADOROJAS (4) |
| low | `JuanCrisostomoVelezdeGuevara_MelindrosaLa` | CANIZARES | 13 | 4/13 (31%) | 2.67 | CANIZARES (4), CERVANTES (1), ANDOSILLA (1) |
| low | `Elvergonzosoenpalacio` | QUEVEDO | 71 | 21/71 (30%) | 2.66 | QUEVEDO (21), LOPE (10), MEDINA (10), MONTALBAN (7), FAJARDOYACEVEDO (3) |
| low | `MoretoyCavanaAgustin_PoetaEl` | GARCIAMARCOS | 14 | 2/14 (14%) | 2.66 | GARCIAMARCOS (2), CERVANTES (1), MELO (1), PAREDES (1), TORRESLORENZODE (1) |
| low | `QUINONESDEBENAVENTE_Mariones` | MATOSFRAGOSO | 12 | 6/12 (50%) | 2.65 | MATOSFRAGOSO (6), VIDALYSALVADOR (1), LICENCIADOROJAS (1), MESA (1) |
| low | `ALVAREZ_NoHayPoderContraLaFe` | VIDALYSALVADOR | 125 | 91/125 (73%) | 2.65 | VIDALYSALVADOR (91), MOLINAYMENDOZA (11), CANIZARES (7), JIMENEZSEDENO (5), VERATASSIS (3) |
| low | `ClaramonteAndresde_ValientenegroenFlandesDJuandeA` | CLARAMONTE | 127 | 30/127 (24%) | 2.64 | CLARAMONTE (30), GALLEGOS (30), AGUADOELVIEJO (11), VELEZ (11), QUINONES (5) |
| low | `LoasparalasfiestasdeNuestraSeoradelaPenaSacra` | GONZALEZDEBARCIA | 66 | 8/66 (12%) | 2.64 | GONZALEZDEBARCIA (8), ANDOSILLA (8), MORETO (4), ROMEROROQUE (4), SARAVIAYMENDOZA (4) |
| low | `SIGLERDEHUERTA_Competidoresyamigos` | CERVANTES | 61 | 28/61 (46%) | 2.64 | CERVANTES (28), GONGORA (20), LICENCIADOROJAS (8), CECILIANACIMIENTO (3), BATRES (1) |
| low | `JeronimodeCancer_ReganonayfiestadetorosLa` | LEIVARAMIREZ | 23 | 7/23 (30%) | 2.63 | LEIVARAMIREZ (7), CALLE (6), CASTILLOSOLORZANO (2), PAREDES (1) |
| low | `FERNANDEZ_FundadoraSantaConcepcionPrimera` | MELO | 71 | 26/71 (37%) | 2.63 | MELO (26), CASTROYSALAZAR (15), GONZALEZDETORRES (11), LANINI (8), ONAVIEDMAYTORRES (3) |
| low | `Papelesvariosgongorinos_012` | CALLE | 100 | 34/100 (34%) | 2.63 | CALLE (34), MELO (19), FAJARDOYACEVEDO (13), VARGASMACHUCA (13), GILENRIQUEZ (6) |
| low | `Porsureyyporsudama` | VIDALYSALVADOR | 54 | 29/54 (54%) | 2.63 | VIDALYSALVADOR (29), GILENRIQUEZ (11), CASTROYSALAZAR (3), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `BaezaAndresde_Hastalasatisfaccion` | TORRESLORENZODE | 58 | 13/58 (22%) | 2.63 | TORRESLORENZODE (13), GARCIAMARCOS (13), ROMEROROQUE (13), PAREDES (2), MOLINAYMENDOZA (2) |
| low | `ParisSanzMatiasde_Jacaradeesdrujulos_Autografo` | LEIVARAMIREZ | 14 | 3/14 (21%) | 2.62 | LEIVARAMIREZ (3), CASTILLOSOLORZANO (1), SANDOVAL (1), BATRES (1) |
| low | `GIL_NoPuedeMentirElCielo` | CARVAJAL | 46 | 23/46 (50%) | 2.62 | CARVAJAL (23), LEIVARAMIREZ (17), REMON (2), QUEVEDO (1), LORENZANA (1) |
| low | `Elparecido` | SANDOVAL | 75 | 19/75 (25%) | 2.62 | SANDOVAL (19), ROJASZORRILLA (14), LOPEZDELCAMPO (11), MORETO (9), CUENCAYARGUELLO (3) |
| low | `Laninfadelcielo` | GARCIAMARCOS | 62 | 18/62 (29%) | 2.61 | GARCIAMARCOS (18), TORRESLORENZODE (12), ROMEROROQUE (3), JIMENEZSEDENO (3), FAJARDOYACEVEDO (3) |
| low | `FranciscoLopezdeZarate_Galeotareforzadaquetomoconsusd` | ROMEROROQUE | 80 | 24/80 (30%) | 2.60 | ROMEROROQUE (24), PAREDES (21), MELO (18), BARREDA (4), GONZALEZDEBARCIA (1) |
| low | `ENRIQUEZGOMEZ_Enganarparareinar_Hisp` | VIDALYSALVADOR | 53 | 28/53 (53%) | 2.60 | VIDALYSALVADOR (28), COELLO (6), AVELLANEDADELACUEVA (4), PAREDES (4), JIMENEZSEDENO (2) |
| low | `ROSETE_RayoYTerrorDeItalia` | MONTALBAN | 136 | 79/136 (58%) | 2.59 | MONTALBAN (79), VIDALYSALVADOR (22), LEIVARAMIREZ (14), VERATASSIS (6), MESA (4) |
| low | `OtazoAlonsode_SuertesdedamasygalanesLas` | RUANO | 16 | 5/16 (31%) | 2.59 | RUANO (5), CARVAJAL (1), VIDALYSALVADOR (1), HURTADODEMENDOZA (1) |
| low | `MENDOZA_QuererporsoloquererBnF` | TORRESLORENZODE | 126 | 46/126 (36%) | 2.59 | TORRESLORENZODE (46), LORENZANA (29), ALARCON (13), CAXESI (10), CARVAJAL (5) |
| low | `ReyesMatiasdelosAtribuido_NacimientodeNuestroSenorJesucr` | CASTILLOSOLORZANO | 63 | 28/63 (44%) | 2.58 | CASTILLOSOLORZANO (28), CALLE (7), SANDOVAL (4), ROMEROROQUE (3), VARGAS (2) |
| low | `MONTESER_Naciones` | ROJASZORRILLA | 26 | 15/26 (58%) | 2.58 | ROJASZORRILLA (15), VIDALYSALVADOR (2), BELMONTE (1), QUINONES (1) |
| low | `PedrodeSoriaAtribuidoLorenzode_SitiodeLeridaEl` | FAJARDOYACEVEDO | 62 | 23/62 (37%) | 2.58 | FAJARDOYACEVEDO (23), CASTILLOSOLORZANO (12), BATRES (4), BELMONTE (4), ENRIQUEZ (3) |
| low | `Lasucesindelpecado` | GALLEGOS | 24 | 10/24 (42%) | 2.57 | GALLEGOS (10), LEIVARAMIREZ (4), BELMONTE (2), BATRES (1), GARCIADEPRADO (1) |
| low | `AntonioMartinezdeMeneses_EsforciasdeMilanJuanGaleazoLos` | MENESES | 113 | 38/113 (34%) | 2.56 | MENESES (38), MORETO (19), ANDOSILLA (10), ROSETENINO (10), CLARAMONTE (6) |
| low | `MoretoyCavanaAgustin_RelojylosorganosEl` | CALDERON | 27 | 5/27 (18%) | 2.56 | CALDERON (5), LOPEZDELCAMPO (2), CAXESI (2), GONZALEZDETORRES (1), ROJASZORRILLA (1) |
| low | `RojasZorrillaFranciscode_Cadacualloqueletoca` | FAJARDOYACEVEDO | 75 | 30/75 (40%) | 2.55 | FAJARDOYACEVEDO (30), ROMEROROQUE (13), GARCIAMARCOS (5), ALARCON (5), CASTILLOSOLORZANO (4) |
| low | `Elparecido2` | GILENRIQUEZ | 46 | 9/46 (20%) | 2.55 | GILENRIQUEZ (9), VIDALYSALVADOR (8), LANINI (8), CASTROYSALAZAR (4), AVELLANEDA (4) |
| low | `PRADO_CosasDeVicenteYCasildilla` | ENRIQUEZ | 6 | 3/6 (50%) | 2.54 | ENRIQUEZ (3), QUINONES (1), VIDALYSALVADOR (1) |
| low | `VegaCarpioLopedeAtribuido_SoldadilloEl` | ANDOSILLA | 17 | 3/17 (18%) | 2.54 | ANDOSILLA (3), LICENCIADOROJAS (1), QUINONES (1), GONGORA (1), GALLEGOS (1) |
| low | `Lafuerzadelacostumbre2` | CORDERO | 39 | 10/39 (26%) | 2.54 | CORDERO (10), VARGAS (9), MULSA (8), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `QuevedoyVillegasFranciscode_MaridofantasmaEl` | HURTADODEMENDOZA | 17 | 4/17 (24%) | 2.54 | HURTADODEMENDOZA (4), LICENCIADOROJAS (1), FAJARDOYACEVEDO (1), QUINONES (1), CASTILLOSOLORZANO (1) |
| low | `QuinonesdeBenaventeLuis_JusticiademujerLa` | ROMEROROQUE | 17 | 4/17 (24%) | 2.53 | ROMEROROQUE (4), GRACIAN (1), ONAVIEDMAYTORRES (1), AVELLANEDADELACUEVA (1), TAMAYO (1) |
| low | `MOTASILVA_NascimentodeChristo` | MEDINA | 122 | 68/122 (56%) | 2.53 | MEDINA (68), SANDOVAL (49), GONGORA (1), TAMAYO (1), TORRESLORENZODE (1) |
| low | `JuandeBenavides_Loquepiensastehago` | GALLEGOS | 141 | 81/141 (57%) | 2.52 | GALLEGOS (81), MIRACLESSOTOMAYOR (21), AGUADOELVIEJO (4), VARGAS (3), GARCIADEPRADO (2) |
| low | `ElgrancardenaldeEspanadonGildeAlbornoz` | ROMEROROQUE | 68 | 12/68 (18%) | 2.52 | ROMEROROQUE (12), FAJARDOYACEVEDO (8), LEIVARAMIREZ (7), MOLINAYMENDOZA (7), JUANDESOTO (4) |
| low | `POEMAS_CairascoFigueroayDesconocido` | BENAVIDES | 79 | 59/79 (75%) | 2.52 | BENAVIDES (59), AVELLANEDA (10), ENRIQUEZ (5), SANDOVAL (2), CECILIANACIMIENTO (1) |
| low | `SimonAguadoelViejo_NinosdelaRollonayloquepasaenla` | DIAMANTE | 14 | 3/14 (21%) | 2.52 | DIAMANTE (3), ANDOSILLA (3), VIDALYSALVADOR (1) |
| low | `CAMARA_BabiloniaDeAmor` | HURTADODEMENDOZA | 38 | 37/38 (97%) | 2.51 | HURTADODEMENDOZA (37), VELEZ (1) |
| low | `ElAdemar` | CASTROYSALAZAR | 218 | 50/218 (23%) | 2.51 | CASTROYSALAZAR (50), CALLE (30), MOLINAYMENDOZA (25), FAJARDOYACEVEDO (13), SANDOVAL (13) |
| low | `ClaramonteAndresde_SanCarlos` | BELMONTE | 63 | 32/63 (51%) | 2.51 | BELMONTE (32), ROJASZORRILLA (8), VELEZ (4), GALLEGOS (3), CLARAMONTE (2) |
| low | `GabrieldeRoa_BatalladelamorLa` | CANIZARES | 26 | 8/26 (31%) | 2.50 | CANIZARES (8), GONZALEZDEBARCIA (3), HURTADODEMENDOZA (2), LICENCIADOROJAS (1), AVELLANEDA (1) |
| low | `MariadeZayas_TraicionenlaamistadLa` | CASTILLOSOLORZANO | 117 | 49/117 (42%) | 2.50 | CASTILLOSOLORZANO (49), TORRESLORENZODE (27), AVELLANEDA (10), ENRIQUEZ (5), PAREDES (3) |
| low | `MiradeAmescuaAntonio_Nohaydichanidesdichahastalamue` | CORDERO | 66 | 14/66 (21%) | 2.50 | CORDERO (14), LEIVARAMIREZ (13), BATRES (7), CASTILLOSOLORZANO (5), FAJARDOYACEVEDO (4) |
| low | `Papelesvariosgongorinos_4` | SARAVIAYMENDOZA | 100 | 51/100 (51%) | 2.49 | SARAVIAYMENDOZA (51), GRACIAN (10), VARGAS (10), CALLE (5), RUIZALCEO (5) |
| low | `ALBORNOZ_Muerteyentierrohonrasdelafamosa` | LOPEZDECASTRO | 48 | 22/48 (46%) | 2.49 | LOPEZDECASTRO (22), CECILIANACIMIENTO (12), TORRESLORENZODE (5), GOMEZACOSTA (3), AVELLANEDA (1) |
| low | `CristobaldeMonroyySilvaAtribui_PleitosdeHernanCortesLos` | CALDERON | 71 | 30/71 (42%) | 2.49 | CALDERON (30), LOPEZDELCAMPO (8), BELMONTE (5), ROJASZORRILLA (5), ENRIQUEZ (3) |
| low | `MonroyySilvaCristobalde_Celosindustriayamor` | LOPE | 121 | 40/121 (33%) | 2.48 | LOPE (40), CAXESI (22), ROJASVILLANDRANDO (16), MENESES (9), CASTILLOSOLORZANO (5) |
| low | `Rosette_TodoSucedeAlReves` | CARVAJAL | 100 | 54/100 (54%) | 2.48 | CARVAJAL (54), MORETO (8), LEIVARAMIREZ (6), MENESES (5), AVELLANEDADELACUEVA (3) |
| low | `SOARES_CantosEHistoriasTragicasDeFilos` | CERVANTES | 192 | 70/192 (36%) | 2.47 | CERVANTES (70), QUEVEDO (68), GONGORA (40), VARGASMACHUCA (7), BENAVIDES (3) |
| low | `LosnoviosdeHornachuelos` | GARCIAMARCOS | 64 | 14/64 (22%) | 2.47 | GARCIAMARCOS (14), PSEUDOHURTADODEMENDOZA (6), BATRES (6), CANIZARES (5), MOLINAYMENDOZA (4) |
| low | `MatosFragosoJuandeMoretoyCavan_MartiresdeMadridydejarunreinop` | CASTILLOSOLORZANO | 46 | 11/46 (24%) | 2.46 | CASTILLOSOLORZANO (11), HOZYMOTA (9), CANIZARES (6), CASTROYSALAZAR (6), MOLINAYMENDOZA (3) |
| low | `MatosFragosoJuande_BastardodeAragonydelincuentesi` | BELMONTE | 75 | 35/75 (47%) | 2.45 | BELMONTE (35), MONTALBAN (8), ROJASZORRILLA (7), QUINONES (4), MESA (3) |
| low | `EldivinoportugusSanAntoniodePadua` | AVELLANEDA | 74 | 30/74 (40%) | 2.45 | AVELLANEDA (30), VIDALYSALVADOR (24), LANINI (6), CASTROYSALAZAR (3), PAREDES (1) |
| low | `GongoraLuisde_FirmezasdeIsabelaLas` | MEDINA | 578 | 283/578 (49%) | 2.45 | MEDINA (283), TORRESLORENZODE (106), MELO (101), LANINI (46), AVELLANEDA (6) |
| low | `CalderonAtribuido_CondeLucanorEl` | DIAMANTE | 76 | 19/76 (25%) | 2.44 | DIAMANTE (19), SANDOVAL (19), ANDOSILLA (14), CALDERON (4), BELMONTE (3) |
| low | `LahonraporlamujerImgenes91a137` | MIRACLESSOTOMAYOR | 47 | 26/47 (55%) | 2.44 | MIRACLESSOTOMAYOR (26), CLARAMONTE (8), REMON (1), MESA (1), ANDOSILLA (1) |
| low | `AntonioEnriquezGomez_Mayormalhayenlavida` | PAREDES | 88 | 39/88 (44%) | 2.44 | PAREDES (39), CECILIANACIMIENTO (12), GOMEZACOSTA (9), AVELLANEDA (7), CORDERO (5) |
| low | `VegaCarpioLopedeAtribuidoJeron_Dinerossoncalidad` | REMON | 59 | 20/59 (34%) | 2.43 | REMON (20), ANDOSILLA (17), TAMAYO (5), MESA (3), SALAZARYTORRES (2) |
| low | `GodinezManriqueFelipe_Debuenmorobuencristiano` | ROJASZORRILLA | 127 | 20/127 (16%) | 2.43 | ROJASZORRILLA (20), BATRES (19), CALDERON (14), CECILIANACIMIENTO (7), VARGASMACHUCA (7) |
| low | `ZARATEFERNANDO_SantaPelagiaMargarita_Novena` | ROSETENINO | 43 | 11/43 (26%) | 2.43 | ROSETENINO (11), CANIZARES (8), LANINI (4), LEIVARAMIREZ (4), QUEVEDO (4) |
| low | `HEREDIA_ALARCON_MENDOZA_Ganarperdiendo` | CALLE | 67 | 31/67 (46%) | 2.43 | CALLE (31), JIMENEZSEDENO (14), FAJARDOYACEVEDO (8), VIDALYSALVADOR (5), CASTILLOSOLORZANO (3) |
| low | `ObrasDramaticasYPapelesVarios-II-462` | PACHECO | 288 | 75/288 (26%) | 2.42 | PACHECO (75), LOPEZDECASTRO (46), GONZALEZDETORRES (28), TORRESLORENZODE (28), VARGAS (26) |
| low | `OlmedoAlonsode_TitulosdecomediasLos` | JIMENEZSEDENO | 6 | 3/6 (50%) | 2.42 | JIMENEZSEDENO (3), BANCESCANDAMO (1), VIDALYSALVADOR (1) |
| low | `SebastianRodriguezdeVillavicio_VirgendelaFuencislaLa` | GARCIAMARCOS | 79 | 22/79 (28%) | 2.41 | GARCIAMARCOS (22), PAREDES (19), VIDALYSALVADOR (14), VERATASSIS (8), CASTROYSALAZAR (3) |
| low | `AntoniodeSolis_NinocaballeroEntremesEl` | VIDALYSALVADOR | 10 | 2/10 (20%) | 2.41 | VIDALYSALVADOR (2), BANCESCANDAMO (1), AMESCUA (1), PAREDES (1) |
| low | `VelezdeGuevaraLuis_NoviosdeHornachuelosLos` | CAXESI | 55 | 10/55 (18%) | 2.41 | CAXESI (10), BATRES (10), ALARCON (6), BELMONTE (5), CASTILLOSOLORZANO (4) |
| low | `CanizaresySuarezdeToledoJosede_MasvalienteextremenoBernardode` | MOLINAYMENDOZA | 49 | 16/49 (33%) | 2.41 | MOLINAYMENDOZA (16), GALLEGOS (11), SANDOVAL (5), MELO (2), QUEVEDO (2) |
| low | `ENCISO_TravesurasDeCarlos_SegundaParte` | CERVANTES | 58 | 23/58 (40%) | 2.41 | CERVANTES (23), CARVAJAL (16), REMON (16), LICENCIADOROJAS (1), LORENZANA (1) |
| low | `VegaCarpioLopede_Mujeresycriados` | SANTATERESA | 130 | 49/130 (38%) | 2.40 | SANTATERESA (49), MESA (31), QUINONES (13), AMESCUA (8), VIDALYSALVADOR (3) |
| low | `VegaCarpioLopede_VidaymuertedeSantaTeresadeJesu` | JIMENEZSEDENO | 79 | 27/79 (34%) | 2.40 | JIMENEZSEDENO (27), CALLE (15), CLARAMONTE (10), GARCIAMARCOS (4), PAREDES (4) |
| low | `CastroMatiasde_PardilloEl` | ANDOSILLA | 14 | 2/14 (14%) | 2.40 | ANDOSILLA (2), QUINONES (2), LICENCIADOROJAS (1), LEONORCUEVA (1), GALLEGOS (1) |
| low | `ElvizcondedelaCorchuela` | LEIVARAMIREZ | 61 | 35/61 (57%) | 2.39 | LEIVARAMIREZ (35), CASTILLOSOLORZANO (7), CARVAJAL (5), TORRESLORENZODE (2), CALLE (2) |
| low | `RojasZorrillaFranciscode_GranpatiodepalacioAutosacramen` | FAJARDOYACEVEDO | 27 | 11/27 (41%) | 2.39 | FAJARDOYACEVEDO (11), ALARCON (4), BOLEAYALVARADO (4), CARVAJAL (2), LICENCIADOROJAS (1) |
| low | `CASTRO_AntojoDeLaGallega_Autografo` | SANDOVAL | 18 | 3/18 (17%) | 2.39 | SANDOVAL (3), MOLINAYMENDOZA (2), HURTADODEMENDOZA (1), CASTROYSALAZAR (1), CANIZARES (1) |
| low | `RojasZorrillaFranciscode_VinadeNabotLa` | BARREDA | 41 | 11/41 (27%) | 2.38 | BARREDA (11), GARCIAMARCOS (6), ROMEROROQUE (5), FAJARDOYACEVEDO (3), LICENCIADOROJAS (1) |
| low | `BARBADELACUEVA_Competenciasdelamor` | MARCHANTE | 27 | 7/27 (26%) | 2.38 | MARCHANTE (7), VARGASMACHUCA (5), CASTROYSALAZAR (5), PAREDES (4), VIDALYSALVADOR (3) |
| low | `FranciscodeRojasySandovalAtrib_ValientePedroPonceEl` | GARCIAMARCOS | 77 | 30/77 (39%) | 2.38 | GARCIAMARCOS (30), PAREDES (27), FAJARDOYACEVEDO (4), CASTROYSALAZAR (2), VIDALYSALVADOR (2) |
| low | `GilLopezdeArmestoyCastro_CantaricoEl` | MELO | 11 | 5/11 (46%) | 2.38 | MELO (5), GONZALEZDEBARCIA (1), VARGASMACHUCA (1) |
| low | `NicolasdeVillarroelAtribuidoDi_FelipeQuintoenItalia` | VIDALYSALVADOR | 97 | 46/97 (47%) | 2.38 | VIDALYSALVADOR (46), MOLINAYMENDOZA (23), GONZALEZDEBARCIA (12), FAJARDOYACEVEDO (2), HURTADODEMENDOZA (1) |
| low | `VegaCarpioLopede_ContiendadeGarciadeParedesyelc` | BATRES | 47 | 23/47 (49%) | 2.38 | BATRES (23), LEIVARAMIREZ (8), QUEVEDO (2), LICENCIADOROJAS (1), HURTADODEMENDOZA (1) |
| low | `FernandodeAnguloyCarcamo_Nosiempreofendenloscelos` | MELO | 92 | 25/92 (27%) | 2.37 | MELO (25), GARCIAMARCOS (15), TAMAYO (15), SANDOVAL (9), AVELLANEDA (7) |
| low | `CALDERONCOELLO_SOLIS_PastorFido` | VERATASSIS | 144 | 126/144 (88%) | 2.36 | VERATASSIS (126), SARAVIAYMENDOZA (2), LORENZANA (2), CERVANTES (1), VIDALYSALVADOR (1) |
| low | `MoretoyCavanaAgustinAtribuido_CelosdeEscarramanLos` | JIMENEZSEDENO | 49 | 14/49 (29%) | 2.35 | JIMENEZSEDENO (14), CALDERON (5), AVELLANEDADELACUEVA (5), FAJARDOYACEVEDO (5), GARCIADEPRADO (5) |
| low | `ElpastorFido2` | GONZALEZDEBARCIA | 71 | 17/71 (24%) | 2.35 | GONZALEZDEBARCIA (17), VIDALYSALVADOR (17), PAREDES (12), CASTROYSALAZAR (6), ONAVIEDMAYTORRES (2) |
| low | `GabrielFeijoodeAraujoLicenciad_ContiendadeloslabradoresdeCald` | LANINI | 16 | 3/16 (19%) | 2.35 | LANINI (3), CASTILLOSOLORZANO (1), GONZALEZDETORRES (1) |
| low | `VegaCarpioLopede_SegundoDavidAutosacramentalEl` | BELMONTE | 23 | 6/23 (26%) | 2.34 | BELMONTE (6), QUEVEDO (3), LOPE (2), MONTALBAN (2), LICENCIADOROJAS (1) |
| low | `Comediasvariasmanuscritas` | CASTROYSALAZAR | 270 | 51/270 (19%) | 2.34 | CASTROYSALAZAR (51), AVELLANEDA (29), GONZALEZDEBARCIA (23), VERATASSIS (20), CERVANTES (19) |
| low | `JuanCrisostomoVelezdeGuevara_BobayelvizcainoLa` | ANDOSILLA | 62 | 25/62 (40%) | 2.34 | ANDOSILLA (25), MENESES (12), LORENZANA (4), CARVAJAL (3), ALARCON (3) |
| low | `ARBOREDA_CatolicoPerseo` | MORETO | 141 | 76/141 (54%) | 2.33 | MORETO (76), VIDALYSALVADOR (26), CANIZARES (9), LEIVARAMIREZ (8), MONTALBAN (7) |
| low | `FranciscodeSandovalAtribuidoCr_RigorhastalamuerteEl` | SANDOVAL | 74 | 29/74 (39%) | 2.33 | SANDOVAL (29), FAJARDOYACEVEDO (10), ROMEROROQUE (8), CASTILLOSOLORZANO (4), QUINONES (2) |
| low | `RojasZorrillaFranciscodeAtribu_FeySanAgustinAutoLa` | FAJARDOYACEVEDO | 26 | 9/26 (35%) | 2.33 | FAJARDOYACEVEDO (9), TORRESLORENZODE (5), CALLE (2), SANDOVAL (2), CLARAMONTE (1) |
| low | `NuestraSenoradeAtocha` | SANDOVAL | 73 | 20/73 (27%) | 2.32 | SANDOVAL (20), FAJARDOYACEVEDO (12), PAREDES (8), LOPEZJACINTO (7), CALLE (3) |
| low | `MontalbanJuanPerezdeAtribuido_MartiresdeValenciaLos` | MIRACLESSOTOMAYOR | 95 | 41/95 (43%) | 2.32 | MIRACLESSOTOMAYOR (41), BELMONTE (22), LOPE (9), ANDOSILLA (5), VILLEGASDELACRUZ (3) |
| low | `FranciscoLopezdeZarate_GaleotadelcondedeNieblaLa` | CASTILLOSOLORZANO | 70 | 21/70 (30%) | 2.32 | CASTILLOSOLORZANO (21), GARCIAMARCOS (14), TORRESLORENZODE (10), ROMEROROQUE (9), PAREDES (5) |
| low | `QUIROS_Sobregustosnohaydisputa` | CASTILLOSOLORZANO | 49 | 24/49 (49%) | 2.32 | CASTILLOSOLORZANO (24), ENRIQUEZ (12), JIMENEZSEDENO (6), PAREDES (3), CERVANTES (1) |
| low | `RUIZ_JuanCazuela` | LOPEZDECARDENA | 15 | 9/15 (60%) | 2.31 | LOPEZDECARDENA (9), VERATASSIS (4), MORETO (2) |
| low | `VARIOS_AntiocoYSeleuco` | CAXESI | 39 | 10/39 (26%) | 2.31 | CAXESI (10), CARVAJAL (9), GARCIADEPRADO (4), LORENZANA (3), CONTRERAS (2) |
| low | `Papelesvariosgongorinos` | LOPEZDECASTRO | 100 | 29/100 (29%) | 2.31 | LOPEZDECASTRO (29), AVELLANEDA (21), FAJARDOYACEVEDO (9), SANDOVAL (8), GODINEZMANRIQUE (7) |
| low | `TellezGabrielAtribuidoMiradeAm_DonAlvarodeLunaoadversafortuna` | CLARAMONTE | 47 | 24/47 (51%) | 2.31 | CLARAMONTE (24), HURTADODEMENDOZA (4), QUINONES (2), REMON (2), LICENCIADOROJAS (1) |
| low | `JuandeQuevedoyArjona_MejorreydeBorgonaEl` | VIDALYSALVADOR | 59 | 17/59 (29%) | 2.31 | VIDALYSALVADOR (17), COELLO (13), PAREDES (12), GONZALEZDEBARCIA (5), GODINEZMANRIQUE (3) |
| low | `LoshijosdelaBarbuda` | RUANO | 62 | 24/62 (39%) | 2.29 | RUANO (24), CANIZARES (10), CASTROYSALAZAR (9), GONZALEZDEBARCIA (3), SANDOVAL (3) |
| low | `VegaCarpioLopede_EldesenganodelmundoAutoLosdosg` | JUANDESOTO | 24 | 5/24 (21%) | 2.29 | JUANDESOTO (5), CARVAJAL (2), GALLEGOS (2), CASTILLOSOLORZANO (1), MESA (1) |
| low | `RojasZorrillaFranciscode_ObligadosyofendidosyGorrondeSa` | ANDOSILLA | 111 | 68/111 (61%) | 2.29 | ANDOSILLA (68), MENESES (12), GARCIADEPRADO (9), AGUADOELVIEJO (6), MORETO (2) |
| low | `VegaCarpioLopedeAtribuido_GallardoJaciminyelhidalgoAbenc` | ENRIQUEZ | 73 | 25/73 (34%) | 2.29 | ENRIQUEZ (25), CASTILLOSOLORZANO (16), GOMEZACOSTA (9), CORDERO (3), COELLO (2) |
| low | `CanizaresySuarezdeToledoJosede_YomeentiendoyDiosmeentiende` | CASTROYSALAZAR | 69 | 21/69 (30%) | 2.27 | CASTROYSALAZAR (21), SANDOVAL (9), LANINI (9), MELO (7), VERATASSIS (6) |
| low | `MatosFragosoJuande_MasimpropioverdugoComediadecha` | CALDERON | 34 | 10/34 (29%) | 2.25 | CALDERON (10), CARVAJAL (7), LOPEZDELCAMPO (4), GARCIADEPRADO (2), VIDALYSALVADOR (1) |
| low | `Elprincipeperfecto` | CONTRERAS | 51 | 14/51 (28%) | 2.25 | CONTRERAS (14), CECILIANACIMIENTO (12), LOPEZDECARDENA (5), VIDALYSALVADOR (2), LOPEZDELCAMPO (2) |
| low | `POLOPEYVALDES_ProfetisaCasandra` | QUINONES | 167 | 75/167 (45%) | 2.25 | QUINONES (75), GARCIADEPRADO (26), HURTADODEMENDOZA (14), CALDERON (11), AGUADOELVIEJO (11) |
| low | `VelezdeGuevaraLuis_NegrodelserafinElsantonegroRos` | GARCIAMARCOS | 77 | 19/77 (25%) | 2.24 | GARCIAMARCOS (19), ROMEROROQUE (13), FAJARDOYACEVEDO (12), ALARCON (12), GARCIADEPRADO (3) |
| low | `VegaCarpioLopede_LabradordelaManchaVillanodelaM` | ROMEROROQUE | 38 | 18/38 (47%) | 2.24 | ROMEROROQUE (18), MEDINA (4), GONGORA (3), MELO (2), AVELLANEDADELACUEVA (1) |
| low | `LaculpamsprovechosayvidaymuertedePoncioPilatos` | GARCIAMARCOS | 63 | 27/63 (43%) | 2.24 | GARCIAMARCOS (27), CASTROYSALAZAR (16), SANDOVAL (8), GILENRIQUEZ (2), CERVANTES (1) |
| low | `AgustindeSalazaryTorres_JuezquefuedesimismoEl` | TORRESLORENZODE | 52 | 14/52 (27%) | 2.24 | TORRESLORENZODE (14), LORENZANA (13), CAXESI (6), ROJASZORRILLA (3), CONTRERAS (3) |
| low | `Papelesvariosgongorinos_7` | LOPEZDECASTRO | 100 | 68/100 (68%) | 2.24 | LOPEZDECASTRO (68), ROMEROROQUE (14), GONZALEZDETORRES (6), RUANO (5), LOPEZJACINTO (2) |
| low | `VegaCarpioLopede_Dosgeniosyesclavosdelsantisimo` | AGUADOELVIEJO | 28 | 15/28 (54%) | 2.23 | AGUADOELVIEJO (15), MENESES (3), CARVAJAL (1), BANCESCANDAMO (1), SANDOVAL (1) |
| low | `AntonioFolchdeCardonaAlagon_JuanyJuana` | BELMONTE | 13 | 2/13 (15%) | 2.23 | BELMONTE (2), FAJARDOYACEVEDO (2), PACHECO (1) |
| low | `ZAMORA_CASTRO_PESIA_VizcondedelaCorchuelaEl` | SARAVIAYMENDOZA | 142 | 90/142 (63%) | 2.23 | SARAVIAYMENDOZA (90), CALLE (23), GARCIAMARCOS (8), MOLINAYMENDOZA (5), GONZALEZDEBARCIA (4) |
| low | `Elportugues` | GARCIAMARCOS | 18 | 7/18 (39%) | 2.23 | GARCIAMARCOS (7), BARREDA (2), LICENCIADOROJAS (1) |
| low | `FranciscoBueno_Robertoeldiablo` | CANIZARES | 52 | 18/52 (35%) | 2.23 | CANIZARES (18), BOLEAYALVARADO (9), GILENRIQUEZ (6), HOZYMOTA (4), CASTROYSALAZAR (2) |
| low | `JuanPerezdeMontalban_Comopadreycomorey` | CASTILLOSOLORZANO | 66 | 21/66 (32%) | 2.22 | CASTILLOSOLORZANO (21), GARCIADEPRADO (7), PAREDES (6), VARGAS (6), ENRIQUEZ (2) |
| low | `GUZMANYHARO_LoQuePasaEnLaCorte` | PAREDES | 26 | 6/26 (23%) | 2.22 | PAREDES (6), VIDALYSALVADOR (3), CASTILLOSOLORZANO (2) |
| low | `MiradeAmescuaAntonioAtribuido_GuardacuidadosaAutoLa` | BELMONTE | 25 | 7/25 (28%) | 2.22 | BELMONTE (7), MONTALBAN (5), QUEVEDO (3), LOPEZDELCAMPO (1), LEIVARAMIREZ (1) |
| low | `DamiandeMenesesAtribuido_Morirporvivirconhonra` | GONZALEZDEBARCIA | 84 | 27/84 (32%) | 2.21 | GONZALEZDEBARCIA (27), ROMEROROQUE (25), FAJARDOYACEVEDO (9), GODINEZMANRIQUE (9), PAREDES (2) |
| low | `VegaCarpioLopede_SanJulian` | FAJARDOYACEVEDO | 72 | 47/72 (65%) | 2.20 | FAJARDOYACEVEDO (47), LEIVARAMIREZ (3), BELMONTE (2), JIMENEZSEDENO (2), GONZALEZDEBARCIA (1) |
| low | `AntonioEnriquezGomez_ReymasperfectoprimeraparteEl` | HURTADODEMENDOZA | 55 | 17/55 (31%) | 2.19 | HURTADODEMENDOZA (17), FAJARDOYACEVEDO (8), QUINONES (6), BATRES (3), CLARAMONTE (3) |
| low | `NAJERA_Aguadelavida` | VIDALYSALVADOR | 14 | 9/14 (64%) | 2.19 | VIDALYSALVADOR (9), BELMONTE (2), LORENZANA (1) |
| low | `ElplatodeGenova` | MEDINA | 56 | 17/56 (30%) | 2.18 | MEDINA (17), SANDOVAL (12), FAJARDOYACEVEDO (8), VILLEGASJUANBAUTISTA (4), LOPEZDECASTRO (3) |
| low | `GONZALEZ_CUNEDO_AunTraidor` | CAXESI | 52 | 15/52 (29%) | 2.17 | CAXESI (15), MEDINA (8), LICENCIADOROJAS (6), QUEVEDO (4), VIDALYSALVADOR (4) |
| low | `LATRE_AventurasDeTelemaco` | AVELLANEDA | 90 | 74/90 (82%) | 2.17 | AVELLANEDA (74), LICENCIADOROJAS (8), VALDIVIELSO (2), LOPEZDECARDENA (2), CECILIANACIMIENTO (1) |
| low | `JuandeVelascoyGuzman_Ramadelmejorarbolypasmodepenit` | CANIZARES | 73 | 22/73 (30%) | 2.16 | CANIZARES (22), BOLEAYALVARADO (10), CAXESI (10), CLARAMONTE (5), MORETO (4) |
| low | `CubillodeAragonAlvaro_MuertedeFrislanAutosacramental` | CASTILLOSOLORZANO | 28 | 12/28 (43%) | 2.16 | CASTILLOSOLORZANO (12), ROMEROROQUE (4), GARCIADEPRADO (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1) |
| low | `FOLCH_NoSiempreMientenSenales` | VIDALYSALVADOR | 254 | 171/254 (67%) | 2.16 | VIDALYSALVADOR (171), VARGASMACHUCA (51), LEONORCUEVA (3), PAREDES (2), CARVAJAL (1) |
| low | `VelezdeGuevaraLuisAtribuidoRoj_DonPedroMiago` | GOMEZACOSTA | 29 | 9/29 (31%) | 2.15 | GOMEZACOSTA (9), GONZALEZDETORRES (8), LICENCIADOROJAS (2), PAREDES (1), BARRIONUEVO (1) |
| low | `AntonioEnriquezGomez_FernanMendezPintoenlaChina` | SANDOVAL | 71 | 20/71 (28%) | 2.15 | SANDOVAL (20), FAJARDOYACEVEDO (17), LEIVARAMIREZ (9), GALLEGOS (6), ROMEROROQUE (5) |
| low | `FERNANDEZ_FundadoraSantaConcepcionSegunda_Autografo` | PAREDES | 77 | 13/77 (17%) | 2.14 | PAREDES (13), LANINI (12), GONZALEZDETORRES (10), CASTROYSALAZAR (8), GARCIAMARCOS (8) |
| low | `SOLIS_Amoresartedeamar` | GARCIADEPRADO | 74 | 42/74 (57%) | 2.14 | GARCIADEPRADO (42), QUEVEDO (18), CASTILLOSOLORZANO (3), GONGORA (3), VIDALYSALVADOR (2) |
| low | `QuinonesdeBenaventeLuis_MayordomoEl` | SANDOVAL | 13 | 2/13 (15%) | 2.14 | SANDOVAL (2), CANIZARES (2) |
| low | `QuinonesdeBenaventeLuis_HonradaLa` | SANDOVAL | 31 | 4/31 (13%) | 2.14 | SANDOVAL (4), GARCIAMARCOS (2), CALLE (2), CASTROYSALAZAR (2), VERATASSIS (1) |
| low | `QuinonesdeBenaventeLuis_RetablodelasmaravillasEl` | MESA | 17 | 3/17 (18%) | 2.13 | MESA (3), MORETO (1), QUINONES (1), ROJASZORRILLA (1), SANDOVAL (1) |
| low | `TellezGabrielAtribuidoVegaCarp_CaballerodeGraciaEl` | LEIVARAMIREZ | 55 | 20/55 (36%) | 2.13 | LEIVARAMIREZ (20), BATRES (7), PAREDES (3), BELMONTE (3), VIDALYSALVADOR (2) |
| low | `NAJERA_DIEGO_LoasacramentalparaelautodeElaguademejorvida` | ANDOSILLA | 8 | 5/8 (62%) | 2.13 | ANDOSILLA (5), CANIZARES (1) |
| low | `CubillodeAragonAlvaro_CondedeSaldanayHechosdeBernard` | SARAVIAYMENDOZA | 65 | 23/65 (35%) | 2.12 | SARAVIAYMENDOZA (23), GARCIAMARCOS (13), PAREDES (7), FAJARDOYACEVEDO (5), CALLE (2) |
| low | `VelezdeGuevaraLuis_HambrientoEl` | FAJARDOYACEVEDO | 16 | 5/16 (31%) | 2.12 | FAJARDOYACEVEDO (5), RUANO (1) |
| low | `VelezdeGuevaraLuis_HijodelaguilaEl` | FAJARDOYACEVEDO | 64 | 15/64 (23%) | 2.11 | FAJARDOYACEVEDO (15), ROMEROROQUE (13), GONZALEZDEBARCIA (9), PAREDES (6), VARGAS (3) |
| low | `VegaCarpioLopedeAtribuido_PerdidasdelquejuegaLa` | GALLEGOS | 50 | 21/50 (42%) | 2.11 | GALLEGOS (21), SANDOVAL (10), LICENCIADOROJAS (2), ENRIQUEZ (2), ROMEROROQUE (2) |
| low | `OrtizdeTorresJuanAtribuido_HechosdelduquedeOsunaSegundapa` | BELMONTE | 147 | 53/147 (36%) | 2.09 | BELMONTE (53), FAJARDOYACEVEDO (25), MEDINA (14), CALLE (11), SANDOVAL (10) |
| low | `Nuncamuchocostpoco` | BATRES | 76 | 14/76 (18%) | 2.09 | BATRES (14), BELMONTE (13), SANDOVAL (13), TORRESLORENZODE (5), FAJARDOYACEVEDO (4) |
| low | `PabloPolopyValdes_Tresmayoresimperioselcieloelma` | ROMEROROQUE | 68 | 26/68 (38%) | 2.08 | ROMEROROQUE (26), MOLINAYMENDOZA (11), GONZALEZDEBARCIA (10), FAJARDOYACEVEDO (7), ALARCON (6) |
| low | `Colecciondevariaspoesiasv_2` | MELO | 364 | 176/364 (48%) | 2.08 | MELO (176), CASTROYSALAZAR (108), SANDOVAL (45), ROMEROROQUE (7), GARCIAMARCOS (1) |
| low | `VegaCarpioLopedeAtribuido_ToledanovengadoycelosovengadoE` | ENRIQUEZ | 43 | 8/43 (19%) | 2.07 | ENRIQUEZ (8), RUIZALCEO (7), CASTILLOSOLORZANO (4), CUEVAYSILVA (2), LOPEZDECASTRO (2) |
| low | `VegaCarpioLopede_PrincipeperfectoSegundaparteCo` | BELMONTE | 127 | 48/127 (38%) | 2.07 | BELMONTE (48), SARAVIAYMENDOZA (17), LEIVARAMIREZ (12), MONTALBAN (7), SANDOVAL (4) |
| low | `Variosautores_Colecciondebailesmojigangasent` | GARCIAMARCOS | 212 | 129/212 (61%) | 2.06 | GARCIAMARCOS (129), TAMAYO (27), PAREDES (23), SANDOVAL (14), LEIVARAMIREZ (3) |
| low | `LeonMerchanteoMarchanteJuanMan_PajesgolososLos` | RUANO | 12 | 3/12 (25%) | 2.05 | RUANO (3), MOLINAYMENDOZA (3), LEONORCUEVA (1), CASTILLOSOLORZANO (1), SANTATERESA (1) |
| low | `CASTRO_QuienMascaAhi` | ROMEROROQUE | 14 | 5/14 (36%) | 2.05 | ROMEROROQUE (5), LICENCIADOROJAS (1) |
| low | `Nuestraseoradelosremedios` | VILLEGASDELACRUZ | 32 | 15/32 (47%) | 2.04 | VILLEGASDELACRUZ (15), MONTALBAN (4), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), TORRESLORENZODE (1) |
| low | `VegaCarpioLopedeAtribuidoMirad_InquisicionLa` | ROMEROROQUE | 32 | 9/32 (28%) | 2.04 | ROMEROROQUE (9), SANDOVAL (6), FAJARDOYACEVEDO (5), GARCIAMARCOS (2), GONZALEZDEBARCIA (1) |
| low | `VICENTE_Autodasciganas` | LEONORCUEVA | 3 | 2/3 (67%) | 2.04 | LEONORCUEVA (2) |
| low | `QUINONESDEBENAVENTE_Ronda` | MATOSFRAGOSO | 14 | 6/14 (43%) | 2.03 | MATOSFRAGOSO (6), LEONORCUEVA (1), REMON (1), VELEZ (1), LICENCIADOROJAS (1) |
| low | `DiegoVillegasdelaCruzyBerrioAt_LocadelcieloSantaPelagiaLa` | QUINONES | 121 | 44/121 (36%) | 2.03 | QUINONES (44), BELMONTE (15), ROJASZORRILLA (8), MONTALBAN (7), CALDERON (6) |
| low | `OrtizdeTorresJuanAtribuido_RemedioenelenganoEl` | JUANDESOTO | 127 | 48/127 (38%) | 2.01 | JUANDESOTO (48), CALLE (23), LEIVARAMIREZ (11), BELMONTE (6), GALLEGOS (5) |
| low | `QuinonesdeBenaventeLuisAtribui_NegroEl` | CUEVAYSILVA | 15 | 3/15 (20%) | 2.01 | CUEVAYSILVA (3), ENRIQUEZ (2), QUINONES (1) |
| low | `MiradeAmescuaAntonio_PastoresdeBelenAutoalnacimient` | CALLE | 40 | 12/40 (30%) | 2.00 | CALLE (12), FAJARDOYACEVEDO (8), CASTILLOSOLORZANO (4), GARCIAMARCOS (3), MOLINAYMENDOZA (2) |
| low | `AntoniodeZamoraAtribuido_VerdadyeltiempoentiempoLa` | SANDOVAL | 29 | 10/29 (34%) | 2.00 | SANDOVAL (10), ROMEROROQUE (7), MELO (2), LICENCIADOROJAS (1), FAJARDOYACEVEDO (1) |
| low | `BelmonteBermudezLuisdeRojasZor_MejoramigoelmuertoyFortunasded` | GARCIADEPRADO | 70 | 22/70 (31%) | 1.99 | GARCIADEPRADO (22), CASTILLOSOLORZANO (10), JIMENEZSEDENO (9), LEIVARAMIREZ (5), CALLE (5) |
| low | `LoaparalafiestadeNuestraSenoradelaPena` | GONZALEZDEBARCIA | 14 | 3/14 (21%) | 1.99 | GONZALEZDEBARCIA (3), FAJARDOYACEVEDO (1), CANIZARES (1), AVELLANEDADELACUEVA (1) |
| low | `Papelesvariosgongorinos_3` | SARAVIAYMENDOZA | 100 | 23/100 (23%) | 1.99 | SARAVIAYMENDOZA (23), VARGAS (19), MULSA (19), GRACIAN (10), MONTALBAN (9) |
| low | `SILVA_ColoquioentrePortugalyCastilla` | JIMENEZSEDENO | 14 | 5/14 (36%) | 1.99 | JIMENEZSEDENO (5), GARCIADEPRADO (3), CALDERON (1), GODINEZMANRIQUE (1), CASTILLOSOLORZANO (1) |
| low | `Elduelocontrasudama2` | CANIZARES | 61 | 25/61 (41%) | 1.98 | CANIZARES (25), GONZALEZDEBARCIA (9), ROSETENINO (4), CORDERO (3), ALARCON (3) |
| low | `SOTO_VeamosSiPuedeHaberComediaSinMujer` | GONZALEZDEBARCIA | 97 | 70/97 (72%) | 1.98 | GONZALEZDEBARCIA (70), ROMEROROQUE (13), MELO (6), SARAVIAYMENDOZA (4), LORENZANA (2) |
| low | `VILLAVICIOSA_RetratoJuanRana` | MOLINAYMENDOZA | 10 | 4/10 (40%) | 1.98 | MOLINAYMENDOZA (4), CERVANTES (1), ROMEROROQUE (1), CANIZARES (1), LEONORCUEVA (1) |
| low | `CASTROYBELLVIS_CondeGrimaldosynacimientodeMontesinosEl` | GILENRIQUEZ | 63 | 12/63 (19%) | 1.97 | GILENRIQUEZ (12), CALDERON (10), ENRIQUEZ (8), ROJASZORRILLA (4), BELMONTE (3) |
| low | `CastroyBellvisGuillende_FuerzadelacostumbreLa` | AGUADOELVIEJO | 109 | 37/109 (34%) | 1.97 | AGUADOELVIEJO (37), CLARAMONTE (19), GARCIAMARCOS (13), VILLEGASJUANBAUTISTA (7), CALLE (6) |
| low | `MALO_AmistadVenceAlRigor` | MOLINAYMENDOZA | 85 | 26/85 (31%) | 1.97 | MOLINAYMENDOZA (26), CASTILLOSOLORZANO (18), GALLEGOS (9), FAJARDOYACEVEDO (7), GONZALEZDEBARCIA (6) |
| low | `QuirosFranciscoBernardode_SordoEl` | FAJARDOYACEVEDO | 10 | 3/10 (30%) | 1.97 | FAJARDOYACEVEDO (3), SANDOVAL (2), GONZALEZDEBARCIA (1), RUANO (1) |
| low | `MATAMOROS_AmarilisYAdonis` | QUINONES | 28 | 10/28 (36%) | 1.97 | QUINONES (10), CALLE (2), LICENCIADOROJAS (1), AMESCUA (1), ROMEROROQUE (1) |
| low | `MonroyySilvaCristobalde_Nohaymassaberquesabersesalvar` | BELMONTE | 99 | 34/99 (34%) | 1.96 | BELMONTE (34), TORRESLORENZODE (15), LOPE (12), ROJASZORRILLA (12), MORETO (3) |
| low | `SAENZTEJERA_LascasasdeMadrid_Autografo` | AGUADOELVIEJO | 31 | 7/31 (23%) | 1.96 | AGUADOELVIEJO (7), ANDOSILLA (2), LICENCIADOROJAS (1), GALLEGOS (1), CLARAMONTE (1) |
| low | `AmbriosioArcedelosReyes_MayorvictoriadeConstantinoMagn` | SARAVIAYMENDOZA | 39 | 8/39 (20%) | 1.95 | SARAVIAYMENDOZA (8), FAJARDOYACEVEDO (6), ENRIQUEZ (3), LANINI (2), TORRESLORENZODE (2) |
| low | `COUTOPESTANA_COPIAAMENO_CamposElysiosDeAmor` | CASTILLOSOLORZANO | 175 | 128/175 (73%) | 1.95 | CASTILLOSOLORZANO (128), VIDALYSALVADOR (24), PAREDES (7), GONZALEZDEBARCIA (4), ROMEROROQUE (4) |
| low | `OsunaAlonsode_Fingirlapropiaverdad` | GILENRIQUEZ | 68 | 13/68 (19%) | 1.95 | GILENRIQUEZ (13), ENRIQUEZ (7), JIMENEZSEDENO (7), PAREDES (5), CORDERO (5) |
| low | `FranciscoMartinezAtribuidoJero_SiElEntremes` | MELO | 18 | 4/18 (22%) | 1.95 | MELO (4), LICENCIADOROJAS (1), CUEVAYSILVA (1), CASTROYSALAZAR (1), ROMEROROQUE (1) |
| low | `ElGranCardenaldeEspanaFrayFranciscoJimnezdeCisneros` | AVELLANEDA | 62 | 19/62 (31%) | 1.94 | AVELLANEDA (19), PACHECO (12), CUEVAYSILVA (8), MEDINA (5), MELO (1) |
| low | `CristobaldeMonroyySilva_LoquepasaenunmesonoElmeson` | LEIVARAMIREZ | 121 | 41/121 (34%) | 1.94 | LEIVARAMIREZ (41), CALLE (33), BELMONTE (12), ROSETENINO (3), MIRACLESSOTOMAYOR (2) |
| low | `Mentirymudarseauntiempo` | FAJARDOYACEVEDO | 56 | 14/56 (25%) | 1.93 | FAJARDOYACEVEDO (14), GONZALEZDEBARCIA (9), ALARCON (4), GARCIAMARCOS (3), ANDOSILLA (3) |
| low | `MiradeAmescuaAntonioVegaCarpio_MartiresdelJaponLos` | MONTALBAN | 82 | 24/82 (29%) | 1.93 | MONTALBAN (24), QUINONES (20), BELMONTE (11), SANDOVAL (7), LEIVARAMIREZ (5) |
| low | `MatiasdeParisSanz_Jacaraenesdrujulos` | FAJARDOYACEVEDO | 14 | 2/14 (14%) | 1.93 | FAJARDOYACEVEDO (2), LICENCIADOROJAS (1), CASTILLOSOLORZANO (1), ROMEROROQUE (1), BATRES (1) |
| low | `Papelesvariosgongorinos_2` | SARAVIAYMENDOZA | 100 | 19/100 (19%) | 1.93 | SARAVIAYMENDOZA (19), FAJARDOYACEVEDO (12), ONAVIEDMAYTORRES (7), LOPEZDECASTRO (6), RUIZALCEO (6) |
| low | `HURTADO_PoesiaYObras` | LOPEZDECASTRO | 455 | 185/455 (41%) | 1.93 | LOPEZDECASTRO (185), CECILIANACIMIENTO (113), CASTILLOSOLORZANO (31), QUEVEDO (30), BENAVIDES (25) |
| low | `Cepeda_Delamigoelenemigoyalasveceslle` | TORRESLORENZODE | 68 | 16/68 (24%) | 1.91 | TORRESLORENZODE (16), BATRES (11), CASTILLOSOLORZANO (10), JUANDESOTO (9), ENRIQUEZ (2) |
| low | `MontalbanJuanPerezde_FormasdeAlcaladeAlcalaLas` | LEIVARAMIREZ | 71 | 17/71 (24%) | 1.90 | LEIVARAMIREZ (17), PAREDES (8), BELMONTE (6), GARCIAMARCOS (4), MESA (3) |
| low | `GASPARDEAVILA_FulleriasDeAmorTerceraJornada` | QUINONES | 23 | 13/23 (56%) | 1.89 | QUINONES (13), BATRES (2), BELMONTE (1), FAJARDOYACEVEDO (1), GARCIADEPRADO (1) |
| low | `MiguelBermudezdeCastro_Primeroalreyquealhonor` | CALLE | 73 | 22/73 (30%) | 1.89 | CALLE (22), LEIVARAMIREZ (15), GARCIAMARCOS (5), CALDERON (5), FAJARDOYACEVEDO (5) |
| low | `RojasZorrillaFranciscodeGabrie_TrompetadeljuicioLa` | SARAVIAYMENDOZA | 70 | 15/70 (21%) | 1.89 | SARAVIAYMENDOZA (15), GARCIADEPRADO (14), CASTILLOSOLORZANO (10), ENRIQUEZ (8), VERATASSIS (5) |
| low | `PedroFranciscodeLaniniySagredo_GrancardenaldeEspanafrFrancisc` | LOPEZDECASTRO | 65 | 13/65 (20%) | 1.89 | LOPEZDECASTRO (13), AVELLANEDA (10), MELO (10), MEDINA (9), ONAVIEDMAYTORRES (6) |
| low | `ArroyoJosede_PobremaspoderosoSanJuandeDiosE` | CANIZARES | 52 | 31/52 (60%) | 1.89 | CANIZARES (31), HOZYMOTA (7), BOLEAYALVARADO (4), BELMONTE (1), CASTROYSALAZAR (1) |
| low | `ClaramonteAndresdeAtribuido_InfanzondeIllescaselreydPedroe` | ENRIQUEZ | 136 | 101/136 (74%) | 1.88 | ENRIQUEZ (101), CERVANTES (4), QUEVEDO (4), LOPE (2), BANCESCANDAMO (1) |
| low | `LOPEZDEARMESTO_TresPotenciasDelAlma` | CONTRERAS | 21 | 18/21 (86%) | 1.88 | CONTRERAS (18), VALDIVIELSO (1), ROJASVILLANDRANDO (1), LOPEZJACINTO (1) |
| low | `TELLEZ_AmorYCelosHacenDiscretos` | CASTILLOSOLORZANO | 67 | 19/67 (28%) | 1.88 | CASTILLOSOLORZANO (19), ALARCON (13), GARCIADEPRADO (12), GODINEZMANRIQUE (3), CONTRERAS (2) |
| low | `JoseRodriguezCornejoAtribuidoA_MejoresperegrinosyJerusalensit` | CAXESI | 44 | 16/44 (36%) | 1.87 | CAXESI (16), VIDALYSALVADOR (6), ALARCON (5), GARCIADEPRADO (4), CERVANTES (1) |
| low | `Varios_Colecciondebailesentremesesyja` | TAMAYO | 192 | 104/192 (54%) | 1.87 | TAMAYO (104), GARCIAMARCOS (48), LEIVARAMIREZ (10), PAREDES (7), MULSA (6) |
| low | `FernandezdeMesaBlas_SilvasylosAyalasLos` | FAJARDOYACEVEDO | 164 | 59/164 (36%) | 1.87 | FAJARDOYACEVEDO (59), CALLE (29), GARCIAMARCOS (12), MELO (10), MULSA (4) |
| low | `QUEVEDO-FRANCISCO-GOMEZ_Perinola` | LANINI | 87 | 23/87 (26%) | 1.87 | LANINI (23), CASTROYSALAZAR (23), VIDALYSALVADOR (10), LEONORCUEVA (8), MELO (7) |
| low | `QuinonesdeBenaventeLuis_Cuatrogalanes` | LEIVARAMIREZ | 17 | 5/17 (29%) | 1.86 | LEIVARAMIREZ (5), ROMEROROQUE (1), ANDOSILLA (1), CASTILLOSOLORZANO (1) |
| low | `AntonGarciaAtribuidoPeroDiazAt_Comediaalopastorilparalanoched` | CUEVAYSILVA | 24 | 6/24 (25%) | 1.84 | CUEVAYSILVA (6), SANTATERESA (2), LICENCIADOROJAS (1), MEDINA (1), LOPEZDECASTRO (1) |
| low | `ElReyEnriqueelEnfermo` | BELMONTE | 79 | 24/79 (30%) | 1.84 | BELMONTE (24), MOLINAYMENDOZA (12), FAJARDOYACEVEDO (7), LEIVARAMIREZ (5), VIDALYSALVADOR (5) |
| low | `JeronimodelaFuentePierola_Enganarconlaverdad` | LANINI | 9 | 3/9 (33%) | 1.83 | LANINI (3), SANDOVAL (1), ROMEROROQUE (1) |
| low | `ENRIQUEZGOMEZ_CardenaldeEspanadongilsegundaparte` | CERVANTES | 63 | 50/63 (79%) | 1.83 | CERVANTES (50), ENRIQUEZ (5), BATRES (4), GONGORA (3), CARVAJAL (1) |
| low | `QuirosJuande_LajuventuddeToledo` | CASTILLOSOLORZANO | 89 | 52/89 (58%) | 1.82 | CASTILLOSOLORZANO (52), GONZALEZDETORRES (5), BENAVIDES (4), ROMEROROQUE (4), ENRIQUEZ (4) |
| low | `MiradeAmescuaAntonio_Examinarsederey` | LEIVARAMIREZ | 61 | 36/61 (59%) | 1.82 | LEIVARAMIREZ (36), JUANDESOTO (12), CASTILLOSOLORZANO (5), LICENCIADOROJAS (1), QUINONES (1) |
| low | `LucasJustiniano_OjosdelcieloymartiriodeSantaLu` | ANDOSILLA | 60 | 18/60 (30%) | 1.81 | ANDOSILLA (18), BATRES (14), AGUADOELVIEJO (7), ALARCON (4), CARVAJAL (3) |
| low | `CastroyBellvisGuillende_DidoyEneasonohaymalqueporbienn` | ENRIQUEZ | 55 | 30/55 (55%) | 1.81 | ENRIQUEZ (30), VERATASSIS (5), LOPEZDECARDENA (5), LANINI (3), VIDALYSALVADOR (2) |
| low | `DiegoFernandezdeSolana_Loquevaleunespanol` | SANDOVAL | 89 | 15/89 (17%) | 1.81 | SANDOVAL (15), GARCIADEPRADO (12), ROSETENINO (12), MULSA (7), GILENRIQUEZ (4) |
| low | `VegaCarpioLopede_GrancolumnafogosaSanBasilioelM` | TORRESLORENZODE | 67 | 35/67 (52%) | 1.80 | TORRESLORENZODE (35), AVELLANEDA (6), CUEVAYSILVA (4), VARGAS (4), RUIZALCEO (3) |
| low | `MOTASILVA_Enelaguavidaymuerte` | MEDINA | 150 | 97/150 (65%) | 1.80 | MEDINA (97), SANDOVAL (30), TORRESLORENZODE (11), JUANDESOTO (5), REMON (1) |
| low | `CastroyBellvisGuillende_FuerzadelasangreLa` | ENRIQUEZ | 56 | 28/56 (50%) | 1.78 | ENRIQUEZ (28), GARCIAMARCOS (8), VIDALYSALVADOR (4), GONZALEZDEBARCIA (2), CORDERO (2) |
| low | `VegaCarpioLopedeAtribuido_HijoporenganocercodeToledoyrey` | CAXESI | 68 | 15/68 (22%) | 1.78 | CAXESI (15), ROMEROROQUE (14), CASTILLOSOLORZANO (10), ROJASVILLANDRANDO (8), MULSA (5) |
| low | `MoretoyCavanaAgustin_EneasdeDiosElcaballerodelsacra` | ROJASZORRILLA | 81 | 17/81 (21%) | 1.78 | ROJASZORRILLA (17), BELMONTE (9), SANDOVAL (6), LEONORCUEVA (6), REMON (6) |
| low | `Llegarenocasion` | BATRES | 78 | 20/78 (26%) | 1.77 | BATRES (20), BELMONTE (16), MENESES (14), TORRESLORENZODE (5), GALLEGOS (4) |
| low | `SebastianRodriguezdeVillavicio_RetratodeJuanRanaEl` | CARVAJAL | 16 | 3/16 (19%) | 1.75 | CARVAJAL (3), HURTADODEMENDOZA (1), BELMONTE (1), CAXESI (1), ANDOSILLA (1) |
| low | `VegaCarpioLopede_DiablopredicadorEl` | ALARCON | 66 | 32/66 (48%) | 1.75 | ALARCON (32), ROMEROROQUE (9), GARCIADEPRADO (8), GONZALEZDEBARCIA (3), CARVAJAL (3) |
| low | `MEJIADELACERDA_AmorDesventurado` | MESA | 128 | 40/128 (31%) | 1.74 | MESA (40), VELEZ (27), CARVAJAL (13), ROJASZORRILLA (9), BATRES (6) |
| low | `VegaCarpioLopede_SecretariodesimismoEl` | LORENZANA | 45 | 15/45 (33%) | 1.74 | LORENZANA (15), CLARAMONTE (8), SALAZARYTORRES (6), TAMAYO (2), MELO (1) |
| low | `VelezdeGuevaraLuis_RenegadodeJerusalenEl` | AGUADOELVIEJO | 56 | 29/56 (52%) | 1.74 | AGUADOELVIEJO (29), QUINONES (9), MESA (4), CARVAJAL (2), CLARAMONTE (2) |
| low | `MatosFragosoJuande_Verycreer` | GARCIAMARCOS | 56 | 12/56 (21%) | 1.73 | GARCIAMARCOS (12), CORDERO (9), TORRESLORENZODE (8), BELMONTE (5), VIDALYSALVADOR (3) |
| low | `PsiquisyCupido` | MELO | 53 | 15/53 (28%) | 1.73 | MELO (15), SANDOVAL (12), AVELLANEDA (8), GONZALEZDEBARCIA (2), CANIZARES (2) |
| low | `MoretoyCavanaAgustin_OrganosyelrelojLos` | LEIVARAMIREZ | 10 | 2/10 (20%) | 1.72 | LEIVARAMIREZ (2), GONZALEZDEBARCIA (1), BELMONTE (1), MOLINAYMENDOZA (1), ROJASZORRILLA (1) |
| low | `CASTRO_Ayo_TragediaPorLosCelos_TBP` | SANTATERESA | 216 | 140/216 (65%) | 1.72 | SANTATERESA (140), GONGORA (41), SANDOVAL (11), LOPEZJACINTO (2), GONZALEZDETORRES (2) |
| low | `CristobaldeMonroyySilva_Loquepuedeeldesenganoymemoriad` | VIDALYSALVADOR | 54 | 21/54 (39%) | 1.72 | VIDALYSALVADOR (21), BELMONTE (7), CASTILLOSOLORZANO (6), MOLINAYMENDOZA (4), HOZYMOTA (4) |
| low | `GilLopezdeArmestoyCastro_SacristanberenjenoEl` | FAJARDOYACEVEDO | 17 | 3/17 (18%) | 1.72 | FAJARDOYACEVEDO (3), MOLINAYMENDOZA (2), ROMEROROQUE (2), LICENCIADOROJAS (1), SANDOVAL (1) |
| low | `Enganarparareinar` | VIDALYSALVADOR | 51 | 25/51 (49%) | 1.71 | VIDALYSALVADOR (25), GARCIADEPRADO (7), CASTILLOSOLORZANO (2), CAXESI (2), CONTRERAS (1) |
| low | `CanizaresySuarezdeToledoJosede_SoldeOccidenteSanBenitoEl` | VIDALYSALVADOR | 161 | 38/161 (24%) | 1.71 | VIDALYSALVADOR (38), VERATASSIS (37), CANIZARES (37), SARAVIAYMENDOZA (7), GONGORA (6) |
| low | `CALLES_ReyesDeLaCampana` | CARVAJAL | 43 | 12/43 (28%) | 1.71 | CARVAJAL (12), VIDALYSALVADOR (9), CERVANTES (8), HURTADODEMENDOZA (4), CASTROYSALAZAR (3) |
| low | `Lahidalga` | RUANO | 17 | 4/17 (24%) | 1.71 | RUANO (4), VIDALYSALVADOR (3) |
| low | `SebastianRodriguezdeVillavicio_VirgendelPilarLa` | CONTRERAS | 66 | 32/66 (48%) | 1.70 | CONTRERAS (32), LOPEZDELCAMPO (11), ENRIQUEZ (5), MESA (4), QUINONES (2) |
| low | `VIRUES_ContraReosPoderosos` | LEIVARAMIREZ | 122 | 50/122 (41%) | 1.70 | LEIVARAMIREZ (50), MORETO (15), GILENRIQUEZ (13), BELMONTE (12), TORRESLORENZODE (9) |
| low | `BANCES_AustriaEnJerusalen` | VIDALYSALVADOR | 58 | 26/58 (45%) | 1.69 | VIDALYSALVADOR (26), GARCIADEPRADO (12), MONTALBAN (7), CASTILLOSOLORZANO (4), HURTADODEMENDOZA (2) |
| low | `MELBURY_3` | SANDOVAL | 953 | 139/953 (15%) | 1.69 | SANDOVAL (139), CERVANTES (97), CASTILLOSOLORZANO (96), LOPEZDECASTRO (62), TORRESLORENZODE (58) |
| low | `AVILA_HistoriaNinives` | CASTILLOSOLORZANO | 86 | 41/86 (48%) | 1.69 | CASTILLOSOLORZANO (41), ENRIQUEZ (30), CERVANTES (8), CORDERO (7) |
| low | `MonteserFranciscoAntoniode_RegistrosLos` | SANDOVAL | 11 | 4/11 (36%) | 1.69 | SANDOVAL (4), CASTILLOSOLORZANO (1), BATRES (1), VIDALYSALVADOR (1) |
| low | `LeonMerchanteoMarchanteJuanMan_PullasequivocadasPrimeraparteL` | GARCIAMARCOS | 14 | 4/14 (29%) | 1.68 | GARCIAMARCOS (4), CASTILLOSOLORZANO (1), PAREDES (1) |
| low | `VegaCarpioLopedeAtribuido_BarlaanyJosafatlosdossoldadosd` | GONZALEZDEBARCIA | 62 | 20/62 (32%) | 1.68 | GONZALEZDEBARCIA (20), FAJARDOYACEVEDO (14), TAMAYO (8), PAREDES (7), VARGAS (3) |
| low | `VelezdeGuevaraLuis_CondedonPeroVelezydonSanchoDes` | JIMENEZSEDENO | 83 | 39/83 (47%) | 1.68 | JIMENEZSEDENO (39), FAJARDOYACEVEDO (14), GARCIAMARCOS (9), CALLE (6), PAREDES (3) |
| low | `MIRADEAMESCUA_AmorIngenioyMujer` | HURTADODEMENDOZA | 18 | 15/18 (83%) | 1.67 | HURTADODEMENDOZA (15), QUEVEDO (1), VARGASMACHUCA (1), GARCIADEPRADO (1) |
| low | `MorirencruzdalavidaoVidadeDimasyGestas` | CANIZARES | 56 | 15/56 (27%) | 1.67 | CANIZARES (15), CASTROYSALAZAR (13), HOZYMOTA (10), GONZALEZDEBARCIA (6), VIDALYSALVADOR (2) |
| low | `MatosFragosoJuandeMoretoyCavan_Oponersealasestrellas` | ANDOSILLA | 76 | 20/76 (26%) | 1.67 | ANDOSILLA (20), QUINONES (8), ROMEROROQUE (6), VARGAS (6), TAMAYO (5) |
| low | `CalderonAtribuido_UniversalredencionLa` | GONZALEZDEBARCIA | 343 | 105/343 (31%) | 1.65 | GONZALEZDEBARCIA (105), CASTILLOSOLORZANO (56), HOZYMOTA (48), CANIZARES (46), ALARCON (17) |
| low | `RojasZorrillaFranciscodeAtribu_RobodeElenaydestrucciondeTroya` | GOMEZACOSTA | 20 | 5/20 (25%) | 1.65 | GOMEZACOSTA (5), LOPEZDECASTRO (2), GONZALEZDEBARCIA (1), SARAVIAYMENDOZA (1), PACHECO (1) |
| low | `VEGABELTRAN_CulpaAmor` | HURTADODEMENDOZA | 41 | 34/41 (83%) | 1.64 | HURTADODEMENDOZA (34), VELEZ (2), GARCIADEPRADO (1), LOPE (1), GALLEGOS (1) |
| low | `Papelesvariosgongorinos_011` | CONTRERAS | 100 | 37/100 (37%) | 1.64 | CONTRERAS (37), GRACIAN (22), FAJARDOYACEVEDO (7), MELO (6), GONZALEZDETORRES (4) |
| low | `CorderoJacinto_SecretarioconfusoEl` | GARCIAMARCOS | 69 | 26/69 (38%) | 1.63 | GARCIAMARCOS (26), BELMONTE (11), PAREDES (6), COELLO (6), MONTALBAN (5) |
| low | `VegaCarpioLopede_PrivanzadelhombreLa` | CUEVAYSILVA | 37 | 19/37 (51%) | 1.63 | CUEVAYSILVA (19), MESA (3), TIRSO (2), BANCESCANDAMO (1), BELMONTE (1) |
| low | `MontalbanJuanPerezde_DoncelladelaborLa` | CORDERO | 58 | 25/58 (43%) | 1.63 | CORDERO (25), VARGAS (14), GARCIAMARCOS (7), ENRIQUEZ (2), GARCIADEPRADO (1) |
| low | `FranciscoRicodeUrrietaAtribuid_DiabloEl` | TORRESLORENZODE | 10 | 2/10 (20%) | 1.62 | TORRESLORENZODE (2), GONZALEZDEBARCIA (1), VIDALYSALVADOR (1), SANDOVAL (1), ROMEROROQUE (1) |
| low | `FernandodeOrbea_ConquistadeSantaFedeBogotaLa` | PAREDES | 86 | 31/86 (36%) | 1.61 | PAREDES (31), GARCIAMARCOS (16), MONTALBAN (6), AVELLANEDA (5), CASTILLOSOLORZANO (5) |
| low | `CorderoJacinto_DonDuartePacheco` | CALDERON | 74 | 17/74 (23%) | 1.61 | CALDERON (17), ALARCON (13), BATRES (12), BELMONTE (5), CARVAJAL (3) |
| low | `VegaCarpioLopede_Quientodoloquiere` | PAREDES | 56 | 18/56 (32%) | 1.60 | PAREDES (18), ROMEROROQUE (17), GARCIAMARCOS (6), FAJARDOYACEVEDO (2), TORRESLORENZODE (2) |
| low | `JuanPerezdeMontalban_CaballerodeFeboEl` | ROMEROROQUE | 36 | 9/36 (25%) | 1.59 | ROMEROROQUE (9), FAJARDOYACEVEDO (5), VARGAS (3), CASTILLOSOLORZANO (2), JIMENEZSEDENO (2) |
| low | `CubillodeAragonAlvaro_GenizarodeEspanaElmasvalientea` | CALDERON | 100 | 20/100 (20%) | 1.59 | CALDERON (20), CONTRERAS (20), ROJASZORRILLA (13), VALDIVIELSO (7), MORETO (6) |
| low | `MatosFragosoJuandeJeronimodeCa_BrutodeBabiloniaEl` | FAJARDOYACEVEDO | 82 | 29/82 (35%) | 1.59 | FAJARDOYACEVEDO (29), CALLE (21), GARCIAMARCOS (12), QUINONES (5), ANDOSILLA (2) |
| low | `FranciscoAntoniodeBancesCandam_MesasdelafortunaLas` | GONZALEZDEBARCIA | 39 | 11/39 (28%) | 1.58 | GONZALEZDEBARCIA (11), HOZYMOTA (8), CANIZARES (6), VIDALYSALVADOR (3), CASTILLOSOLORZANO (1) |
| low | `ClaramonteAndresde_DotedelrosarioEl` | LEIVARAMIREZ | 34 | 10/34 (29%) | 1.57 | LEIVARAMIREZ (10), QUINONES (7), FAJARDOYACEVEDO (6), RUIZALCEO (2), LICENCIADOROJAS (1) |
| low | `ARGENSOLA_IsabelaTBP` | VARGASMACHUCA | 99 | 62/99 (63%) | 1.57 | VARGASMACHUCA (62), GONGORA (20), HURTADODEMENDOZA (7), ENRIQUEZ (5), CALLE (1) |
| low | `VegaCarpioLopede_RuisenordeSevillaEl` | PSEUDOHURTADODEMENDOZA | 69 | 11/69 (16%) | 1.56 | PSEUDOHURTADODEMENDOZA (11), CARVAJAL (9), VELEZ (9), ANDOSILLA (6), MENESES (5) |
| low | `CALEDERON_AntesQueTodoEsMiDama` | VERATASSIS | 153 | 46/153 (30%) | 1.56 | VERATASSIS (46), PAREDES (44), AVELLANEDADELACUEVA (10), MELO (9), GARCIAMARCOS (4) |
| low | `AntoniodeSolis_EuridiceyOrfeo` | GONZALEZDEBARCIA | 52 | 16/52 (31%) | 1.56 | GONZALEZDEBARCIA (16), HOZYMOTA (11), CASTILLOSOLORZANO (4), ALARCON (4), CAXESI (2) |
| low | `OlmedoHipolitode_LadronesyelalfanjeLos` | ENRIQUEZ | 15 | 4/15 (27%) | 1.56 | ENRIQUEZ (4), QUINONES (1), VIDALYSALVADOR (1) |
| low | `CubillodeAragonAlvaro_PerfectacasadaLa` | CASTILLOSOLORZANO | 64 | 15/64 (23%) | 1.55 | CASTILLOSOLORZANO (15), LEIVARAMIREZ (11), GARCIAMARCOS (9), GONZALEZDEBARCIA (4), ROMEROROQUE (4) |
| low | `JosedeValdivielso_LocuraFarsasacramentaldelmaest` | FAJARDOYACEVEDO | 85 | 38/85 (45%) | 1.55 | FAJARDOYACEVEDO (38), SARAVIAYMENDOZA (10), CALLE (6), CASTILLOSOLORZANO (3), LEIVARAMIREZ (3) |
| low | `PAULAGONZALEZ_MosqueterodeFlandesEl` | GARCIADEPRADO | 68 | 20/68 (29%) | 1.55 | GARCIADEPRADO (20), VIDALYSALVADOR (11), CALDERON (7), ROJASZORRILLA (6), GONGORA (4) |
| low | `EltemplovivodeDios` | GARCIADEPRADO | 49 | 23/49 (47%) | 1.54 | GARCIADEPRADO (23), GONZALEZDEBARCIA (14), VIDALYSALVADOR (3), CECILIANACIMIENTO (1), COELLO (1) |
| low | `FERNANDEZ_VARGAS_AgranDano` | CARVAJAL | 57 | 17/57 (30%) | 1.54 | CARVAJAL (17), CASTILLOSOLORZANO (9), ENRIQUEZ (9), ALARCON (7), GARCIADEPRADO (3) |
| low | `VegaCarpioLopede_JuventuddeSanIsidroLabradorLa` | GALLEGOS | 36 | 14/36 (39%) | 1.54 | GALLEGOS (14), CLARAMONTE (7), VELEZ (4), QUEVEDO (3), HURTADODEMENDOZA (1) |
| low | `SALAZAR_VERATASSIS_MasTriunfaElAmorRendido` | GARCIADEPRADO | 125 | 37/125 (30%) | 1.52 | GARCIADEPRADO (37), ENRIQUEZ (35), VIDALYSALVADOR (34), COELLO (6), GODINEZMANRIQUE (4) |
| low | `MatiasdeCastro_Entremesfamosoalnacimientodelr` | GALLEGOS | 17 | 4/17 (24%) | 1.52 | GALLEGOS (4), GONGORA (2), CASTILLOSOLORZANO (1), PSEUDOHURTADODEMENDOZA (1) |
| low | `Elduelocontrasudama3` | CANIZARES | 57 | 23/57 (40%) | 1.52 | CANIZARES (23), GILENRIQUEZ (9), HOZYMOTA (5), GONZALEZDEBARCIA (4), ALARCON (3) |
| low | `AntonioTellodeMeneses_Mayordelosmilagrosporpremiodeu` | CANIZARES | 67 | 31/67 (46%) | 1.51 | CANIZARES (31), CARVAJAL (10), MOLINAYMENDOZA (8), GARCIADEPRADO (2), DIAMANTE (2) |
| low | `Laduca` | MOLINAYMENDOZA | 14 | 2/14 (14%) | 1.51 | MOLINAYMENDOZA (2), FAJARDOYACEVEDO (2), GALLEGOS (1) |
| low | `LahonraporlamujerImgenes46a90` | CLARAMONTE | 45 | 19/45 (42%) | 1.51 | CLARAMONTE (19), MIRACLESSOTOMAYOR (11), ROJASZORRILLA (4), REMON (3), GONZALEZDEBARCIA (1) |
| low | `BelmonteBermudezLuisde_SastredelCampilloEl` | CANIZARES | 53 | 39/53 (74%) | 1.51 | CANIZARES (39), GONGORA (3), HURTADODEMENDOZA (2), LICENCIADOROJAS (1), HOZYMOTA (1) |
| low | `CASTRO_FuerzaDeLaCostumbre` | ENRIQUEZ | 55 | 33/55 (60%) | 1.50 | ENRIQUEZ (33), REMON (8), QUEVEDO (4), MEDINA (3), AVELLANEDA (1) |
| low | `ZAYAS_CartaDuquesaLemos` | CERVANTES | 4 | 2/4 (50%) | 1.49 | CERVANTES (2), HURTADODEMENDOZA (1) |
| low | `VicenteEximenezyLloris_MaldicioncontrasiLa` | PAREDES | 73 | 21/73 (29%) | 1.49 | PAREDES (21), CASTILLOSOLORZANO (21), SARAVIAYMENDOZA (9), CONTRERAS (4), CORDERO (3) |
| low | `AntonioValladaresdeSotomayor_Dosfamososmanchegosymascarasde` | ROMEROROQUE | 26 | 8/26 (31%) | 1.49 | ROMEROROQUE (8), GONGORA (4), LEONORCUEVA (1), CASTROYSALAZAR (1) |
| low | `VegaCarpioLopedeAtribuido_NohayvidacomolahonraoNohayvida` | LOPEZDECASTRO | 42 | 17/42 (40%) | 1.49 | LOPEZDECASTRO (17), GONZALEZDETORRES (10), LANINI (3), ONAVIEDMAYTORRES (2), CASTROYSALAZAR (1) |
| low | `AntoniodeZamoraJuanCarlosAmatA_GuitarraLa` | MOLINAYMENDOZA | 9 | 3/9 (33%) | 1.48 | MOLINAYMENDOZA (3), CASTILLOSOLORZANO (1), LEIVARAMIREZ (1), ANDOSILLA (1), ROSETENINO (1) |
| low | `FranciscoAntoniodeBancesCandam_PrimerduelodelmundoEl` | VARGASMACHUCA | 48 | 33/48 (69%) | 1.48 | VARGASMACHUCA (33), CASTILLOSOLORZANO (4), RUANO (3), LICENCIADOROJAS (1), ROMEROROQUE (1) |
| low | `CUNHABROCHADO_LaMasDudosaEvidencia` | VIDALYSALVADOR | 3 | 2/3 (67%) | 1.48 | VIDALYSALVADOR (2), PAREDES (1) |
| low | `JuanSalvo_SanAntoniodePadua` | RUANO | 98 | 35/98 (36%) | 1.48 | RUANO (35), GARCIAMARCOS (17), SARAVIAYMENDOZA (9), FAJARDOYACEVEDO (8), MOLINAYMENDOZA (4) |
| low | `QuevedoyVillegasFranciscodeAtr_DesposadoenmantillasEl` | SANDOVAL | 61 | 28/61 (46%) | 1.47 | SANDOVAL (28), JUANDESOTO (6), MEDINA (5), GALLEGOS (3), TORRESLORENZODE (2) |
| low | `MULET_PrincesaTallina` | CARVAJAL | 27 | 15/27 (56%) | 1.47 | CARVAJAL (15), GONGORA (4), AVELLANEDADELACUEVA (3), GARCIADEPRADO (2), VERATASSIS (1) |
| low | `VILLEGAS_BatallaDelAlbis1` | ENRIQUEZ | 98 | 20/98 (20%) | 1.47 | ENRIQUEZ (20), MESA (20), BATRES (13), GILENRIQUEZ (6), BELMONTE (6) |
| low | `ACEVEDO_MargaritaDelTajo` | TORRESLORENZODE | 854 | 122/854 (14%) | 1.46 | TORRESLORENZODE (122), ROJASVILLANDRANDO (121), LOPEZDECASTRO (105), CECILIANACIMIENTO (88), JUANDESOTO (80) |
| low | `TellezGabriel_VergonzosoenpalacioEl` | MEDINA | 76 | 17/76 (22%) | 1.46 | MEDINA (17), GOMEZACOSTA (10), VILLEGASJUANBAUTISTA (9), DAVILAYPALOMARES (8), GILENRIQUEZ (6) |
| low | `VegaCarpioLopede_Sembrarenbuenatierra` | FAJARDOYACEVEDO | 85 | 29/85 (34%) | 1.45 | FAJARDOYACEVEDO (29), ROMEROROQUE (18), CALLE (14), MONTALBAN (5), SANDOVAL (2) |
| low | `ZAMORA_AngelicaYMedoro` | GONZALEZDEBARCIA | 68 | 25/68 (37%) | 1.45 | GONZALEZDEBARCIA (25), AVELLANEDADELACUEVA (22), MULSA (10), CANIZARES (3), GRACIAN (2) |
| low | `VegaCarpioLopede_AveMariayRosariodeNuestraSenor` | CLARAMONTE | 29 | 8/29 (28%) | 1.44 | CLARAMONTE (8), BELMONTE (8), REMON (1), AGUADOELVIEJO (1), MIRACLESSOTOMAYOR (1) |
| low | `VegaCarpioLopede_BautismodeCristo` | BATRES | 25 | 10/25 (40%) | 1.44 | BATRES (10), ENRIQUEZ (5), QUEVEDO (2), CASTILLOSOLORZANO (1) |
| low | `RIVERA_RobertoElDiablo` | CASTROYSALAZAR | 101 | 74/101 (73%) | 1.44 | CASTROYSALAZAR (74), JIMENEZSEDENO (10), VIDALYSALVADOR (4), CANIZARES (4), GILENRIQUEZ (3) |
| low | `LeonMerchanteoMarchanteJuanMan_EstafetaLa` | AVELLANEDADELACUEVA | 31 | 2/31 (6%) | 1.44 | AVELLANEDADELACUEVA (2), CANIZARES (2), CASTILLOSOLORZANO (1), MULSA (1), MORETO (1) |
| low | `LuisMejiadelaCerda_JuegodelhombreAutosacramentalE` | VILLEGASDELACRUZ | 57 | 17/57 (30%) | 1.44 | VILLEGASDELACRUZ (17), VARGAS (11), MEDINA (3), MIRACLESSOTOMAYOR (3), GONZALEZDEBARCIA (2) |
| low | `SOTODEZALDIBAR_GodoreyLeovigildo` | SARAVIAYMENDOZA | 143 | 87/143 (61%) | 1.44 | SARAVIAYMENDOZA (87), GILENRIQUEZ (18), CASTROYSALAZAR (13), VERATASSIS (12), MELO (6) |
| low | `CARO_Valoragravio2` | FAJARDOYACEVEDO | 41 | 13/41 (32%) | 1.42 | FAJARDOYACEVEDO (13), VARGAS (7), CUEVAYSILVA (4), LOPEZDECASTRO (2), ENRIQUEZ (2) |
| low | `Valoragravioymujer` | FAJARDOYACEVEDO | 41 | 13/41 (32%) | 1.42 | FAJARDOYACEVEDO (13), VARGAS (7), CUEVAYSILVA (4), LOPEZDECASTRO (2), ENRIQUEZ (2) |
| low | `CALDERONROSETE_ElioSeyano` | COELLO | 108 | 22/108 (20%) | 1.42 | COELLO (22), LEIVARAMIREZ (12), PAREDES (9), BATRES (9), VIDALYSALVADOR (8) |
| low | `MontalbanJuanPerezde_HijodelserafinsanPedrodeAlcant` | GONZALEZDEBARCIA | 51 | 10/51 (20%) | 1.41 | GONZALEZDEBARCIA (10), CASTROYSALAZAR (9), CANIZARES (7), CASTILLOSOLORZANO (4), CAXESI (4) |
| low | `MatiasdeCastro_Olalla` | CALLE | 15 | 8/15 (53%) | 1.41 | CALLE (8), AVELLANEDADELACUEVA (2), CASTILLOSOLORZANO (1), VARGASMACHUCA (1), VIDALYSALVADOR (1) |
| low | `VegaCarpioLopede_DivinavencedoraLa` | CALLE | 25 | 9/25 (36%) | 1.40 | CALLE (9), CASTILLOSOLORZANO (2), ALARCON (2), LEIVARAMIREZ (2), JUANDESOTO (1) |
| low | `LUPERCIO_Alejandra_TBP` | VARGASMACHUCA | 820 | 427/820 (52%) | 1.40 | VARGASMACHUCA (427), GONGORA (115), HURTADODEMENDOZA (109), CERVANTES (66), ENRIQUEZ (15) |
| low | `Florinea-II-340` | CERVANTES | 912 | 432/912 (47%) | 1.39 | CERVANTES (432), GONGORA (101), LEONORCUEVA (100), AVELLANEDADELACUEVA (89), VERATASSIS (82) |
| low | `FONTANELLA_teatreipoesia` | VARGASMACHUCA | 161 | 99/161 (62%) | 1.38 | VARGASMACHUCA (99), ENRIQUEZ (45), VIDALYSALVADOR (8), PAREDES (8), CERVANTES (1) |
| low | `SIGLERDEHUERTA_Nohaybiensindanoajeno` | CERVANTES | 63 | 45/63 (71%) | 1.38 | CERVANTES (45), ENRIQUEZ (7), CASTILLOSOLORZANO (4), GILENRIQUEZ (2), QUEVEDO (2) |
| low | `RomanMonterodeEspinosa_MiserableenamoradoEl` | CANIZARES | 16 | 4/16 (25%) | 1.37 | CANIZARES (4), CLARAMONTE (2) |
| low | `VELA_PerdidadeEspanaLa` | VERATASSIS | 151 | 33/151 (22%) | 1.37 | VERATASSIS (33), MULSA (29), AGUADOELVIEJO (27), MENESES (18), HURTADODEMENDOZA (18) |
| low | `Elduelocontrasudama` | HOZYMOTA | 58 | 22/58 (38%) | 1.37 | HOZYMOTA (22), CANIZARES (11), MOLINAYMENDOZA (10), GONZALEZDEBARCIA (3), LEIVARAMIREZ (2) |
| low | `JuanSalvo_IntroduccionparalacontradanzaY` | BELMONTE | 8 | 2/8 (25%) | 1.37 | BELMONTE (2), LEONORCUEVA (1), CASTILLOSOLORZANO (1), SANDOVAL (1), MOLINAYMENDOZA (1) |
| low | `QUINONESDEBENAVENTE_SacristanTorrijos` | REMON | 22 | 7/22 (32%) | 1.36 | REMON (7), ROJASZORRILLA (7), MESA (3), MATOSFRAGOSO (3), VIDALYSALVADOR (1) |
| low | `RUIZDEALARCON_ParedesOyen` | AVELLANEDA | 130 | 78/130 (60%) | 1.36 | AVELLANEDA (78), CORDERO (23), CASTILLOSOLORZANO (6), CECILIANACIMIENTO (1), AMESCUA (1) |
| low | `CalderonAtribuido_EsclavadesumaridoLa` | ENRIQUEZ | 75 | 30/75 (40%) | 1.35 | ENRIQUEZ (30), BELMONTE (9), QUINONES (4), MONTALBAN (3), VIDALYSALVADOR (2) |
| low | `LeonMerchanteoMarchanteJuanMan_SaineteparalafiestadelaZarzuel` | MARCHANTE | 14 | 2/14 (14%) | 1.35 | MARCHANTE (2), SANDOVAL (1), GONGORA (1), PSEUDOHURTADODEMENDOZA (1) |
| low | `NAJERA_Aguademejorvida` | CERVANTES | 107 | 102/107 (95%) | 1.35 | CERVANTES (102), LICENCIADOROJAS (5) |
| low | `Loslatines` | QUINONES | 13 | 3/13 (23%) | 1.34 | QUINONES (3), LICENCIADOROJAS (1), GRACIAN (1), SALAZARYTORRES (1) |
| low | `CASTILLA_NietoDeSuPadre` | SANDOVAL | 46 | 15/46 (33%) | 1.33 | SANDOVAL (15), MEDINA (12), LEONORCUEVA (6), GILENRIQUEZ (4), MELO (3) |
| low | `LosbalconesdeMadridcomedia` | QUINONES | 66 | 16/66 (24%) | 1.33 | QUINONES (16), ENRIQUEZ (8), VARGAS (6), BELMONTE (5), BATRES (4) |
| low | `JuanCaxesi_DesposoriosdelaVirgenLos` | ENRIQUEZ | 26 | 7/26 (27%) | 1.32 | ENRIQUEZ (7), ALARCON (5), CASTILLOSOLORZANO (3), CECILIANACIMIENTO (2), COELLO (2) |
| low | `ARGENSOLA_Versos` | ENRIQUEZ | 621 | 317/621 (51%) | 1.32 | ENRIQUEZ (317), CERVANTES (156), VARGASMACHUCA (34), QUEVEDO (13), LOPE (8) |
| low | `Papelesvariosgongorinos_010` | LOPEZDECASTRO | 100 | 47/100 (47%) | 1.31 | LOPEZDECASTRO (47), GONZALEZDETORRES (12), RUANO (10), CASTILLOSOLORZANO (7), CERVANTES (5) |
| low | `CastroyBellvisGuillende_Enganarseenganado` | SANTATERESA | 62 | 19/62 (31%) | 1.31 | SANTATERESA (19), BELMONTE (10), GALLEGOS (5), LEONORCUEVA (5), SANDOVAL (2) |
| low | `VegaCarpioLopedeAtribuidoMirad_SantaInquisicionLa` | ROJASZORRILLA | 52 | 12/52 (23%) | 1.30 | ROJASZORRILLA (12), CALLE (10), BELMONTE (7), MORETO (5), LEIVARAMIREZ (2) |
| low | `CEU_Cartas` | BELMONTE | 109 | 80/109 (73%) | 1.30 | BELMONTE (80), ENRIQUEZ (11), SANDOVAL (10), QUEVEDO (4), PAREDES (2) |
| low | `MONTORO_EntremesAbamino` | GONGORA | 27 | 13/27 (48%) | 1.30 | GONGORA (13), CERVANTES (12), CASTILLOSOLORZANO (1), HURTADODEMENDOZA (1) |
| low | `MiradeAmescuaAntonio_TerceradesimismaLa` | AGUADOELVIEJO | 77 | 16/77 (21%) | 1.30 | AGUADOELVIEJO (16), CONTRERAS (13), ROSETENINO (7), LEIVARAMIREZ (7), ALARCON (6) |
| low | `FranciscoAntoniodeBancesCandam_MesasdelafortunaAutosacramenta` | GALLEGOS | 36 | 8/36 (22%) | 1.29 | GALLEGOS (8), GARCIADEPRADO (4), HOZYMOTA (4), CARVAJAL (2), MULSA (2) |
| low | `VILLEGAS_BatallaDelAlbis` | HURTADODEMENDOZA | 39 | 22/39 (56%) | 1.28 | HURTADODEMENDOZA (22), GARCIADEPRADO (5), CASTILLOSOLORZANO (3), CERVANTES (3), HOZYMOTA (3) |
| low | `VegaCarpioLopede_VueltadeEgiptoalsantonacimient` | GARCIAMARCOS | 40 | 14/40 (35%) | 1.28 | GARCIAMARCOS (14), MELO (10), SANDOVAL (4), MOLINAYMENDOZA (2), LICENCIADOROJAS (1) |
| low | `LOZANO_poemaJanvico` | VARGASMACHUCA | 62 | 29/62 (47%) | 1.27 | VARGASMACHUCA (29), MELO (12), ROMEROROQUE (6), RUANO (2), CALLE (2) |
| low | `Amistadyobligacion` | MULSA | 73 | 21/73 (29%) | 1.27 | MULSA (21), CONTRERAS (17), AMESCUA (16), CASTILLOSOLORZANO (4), MENESES (4) |
| low | `LOA_AmoryObligacion` | PAREDES | 9 | 6/9 (67%) | 1.26 | PAREDES (6), JIMENEZSEDENO (2), MELO (1) |
| low | `ClaramonteAndresde_PandeVallecasEl` | LEIVARAMIREZ | 23 | 6/23 (26%) | 1.25 | LEIVARAMIREZ (6), BELMONTE (3), MENESES (2), BATRES (2), CONTRERAS (1) |
| low | `AntoniodeSolis_Triunfosdeamoryfortuna` | LANINI | 64 | 21/64 (33%) | 1.24 | LANINI (21), ONAVIEDMAYTORRES (13), BANCESCANDAMO (13), SALAZARYTORRES (5), LOPEZJACINTO (5) |
| low | `LareinaSevillaycarbonerosdeFrancia` | GARCIAMARCOS | 27 | 9/27 (33%) | 1.24 | GARCIAMARCOS (9), PAREDES (9), VERATASSIS (3), MELO (2), CASTROYSALAZAR (1) |
| low | `ExpedienteFELICIANA` | MIRACLESSOTOMAYOR | 12 | 5/12 (42%) | 1.24 | MIRACLESSOTOMAYOR (5), TIRSO (2), MULSA (1), ANDOSILLA (1), CARVAJAL (1) |
| low | `JuanBautistaDiamanteAtribuido_PedrodeUrdemalas` | CALLE | 167 | 57/167 (34%) | 1.24 | CALLE (57), SARAVIAYMENDOZA (29), VERATASSIS (16), GARCIAMARCOS (8), MONTALBAN (8) |
| low | `AVILA_ColoquiodelaNatividad` | ENRIQUEZ | 48 | 25/48 (52%) | 1.23 | ENRIQUEZ (25), CASTILLOSOLORZANO (12), CORDERO (8), CERVANTES (3) |
| low | `CanceryVelascoJeronimode_Lazarzuelaentremesparaunafiest` | VIDALYSALVADOR | 10 | 4/10 (40%) | 1.23 | VIDALYSALVADOR (4), SARAVIAYMENDOZA (2), JIMENEZSEDENO (1), CORDERO (1) |
| low | `DiegodeNajerayZegri_DuenasLas` | ROMEROROQUE | 10 | 5/10 (50%) | 1.23 | ROMEROROQUE (5), LOPEZDECASTRO (1), AGUADOELVIEJO (1) |
| low | `TORRE_Zarzuela` | CASTILLOSOLORZANO | 74 | 17/74 (23%) | 1.22 | CASTILLOSOLORZANO (17), GARCIADEPRADO (17), CERVANTES (15), HURTADODEMENDOZA (8), PAREDES (7) |
| low | `LeonMerchanteoMarchanteJuanMan_GargollaJacaraentremesada` | SALAZARYTORRES | 14 | 2/14 (14%) | 1.22 | SALAZARYTORRES (2), AVELLANEDADELACUEVA (1), CARVAJAL (1), LOPEZJACINTO (1) |
| low | `Elgalanfantasma2` | BATRES | 66 | 22/66 (33%) | 1.22 | BATRES (22), CASTILLOSOLORZANO (13), GALLEGOS (8), BELMONTE (5), LEIVARAMIREZ (4) |
| low | `GodinezManriqueFelipe_TrabajosdeJobLos` | GARCIAMARCOS | 23 | 5/23 (22%) | 1.21 | GARCIAMARCOS (5), TORRESLORENZODE (4), RUIZALCEO (2), GONZALEZDEBARCIA (1), JIMENEZSEDENO (1) |
| low | `ArboredaAlejandro_MasdivinoremedioyauroradeSanGi` | CASTROYSALAZAR | 53 | 22/53 (42%) | 1.21 | CASTROYSALAZAR (22), GONZALEZDEBARCIA (8), VIDALYSALVADOR (3), CAXESI (2), CANIZARES (2) |
| low | `SonetoANAMARIAMOURA` | CERVANTES | 1 | 1/1 (100%) | 1.20 | CERVANTES (1) |
| low | `ClaramonteAndresde_Delovivoalopintado` | JIMENEZSEDENO | 67 | 36/67 (54%) | 1.20 | JIMENEZSEDENO (36), CALLE (12), MELO (2), HURTADODEMENDOZA (1), GILENRIQUEZ (1) |
| low | `RojasZorrillaFranciscodeAtribu_DonGildelaMancha` | LICENCIADOROJAS | 56 | 32/56 (57%) | 1.19 | LICENCIADOROJAS (32), CERVANTES (8), LORENZANA (5), REMON (1), TORRESLORENZODE (1) |
| low | `VegaCarpioLopede_HijodelaiglesiaEl` | SANTATERESA | 34 | 9/34 (26%) | 1.18 | SANTATERESA (9), MONTALBAN (4), LOPE (2), CLARAMONTE (2), HURTADODEMENDOZA (2) |
| low | `PedroRoseteNino_TorredelorbeLa` | ROMEROROQUE | 62 | 29/62 (47%) | 1.18 | ROMEROROQUE (29), MOLINAYMENDOZA (10), GARCIAMARCOS (3), FAJARDOYACEVEDO (3), LICENCIADOROJAS (1) |
| low | `RojasZorrillaFranciscode_SantaIsabelreinadePortugal` | CARVAJAL | 50 | 10/50 (20%) | 1.17 | CARVAJAL (10), GALLEGOS (8), LEIVARAMIREZ (7), JUANDESOTO (7), QUEVEDO (4) |
| low | `VALLES_SantoNinoGuardia` | LANINI | 61 | 14/61 (23%) | 1.17 | LANINI (14), LICENCIADOROJAS (13), VARGAS (12), MEDINA (11), PACHECO (3) |
| low | `VALLES_ContraLaFeNoHayRespeto` | LICENCIADOROJAS | 72 | 45/72 (62%) | 1.16 | LICENCIADOROJAS (45), REMON (13), GONGORA (4), SANDOVAL (4), MEDINA (3) |
| low | `QuirosFranciscoBernardode_MacilentoyastrologofingidoElmu` | GARCIAMARCOS | 16 | 2/16 (12%) | 1.16 | GARCIAMARCOS (2), FAJARDOYACEVEDO (2), GALLEGOS (1), JIMENEZSEDENO (1), GARCIADEPRADO (1) |
| low | `VegaCarpioLopede_AventurasdelhombreLas` | SANDOVAL | 35 | 8/35 (23%) | 1.15 | SANDOVAL (8), MONTALBAN (5), GARCIAMARCOS (4), QUINONES (2), VARGAS (2) |
| low | `NAJERA_AguaDeMejorVidaElMojiganga` | CAXESI | 14 | 2/14 (14%) | 1.15 | CAXESI (2), LEIVARAMIREZ (2), CECILIANACIMIENTO (1), DIAMANTE (1), BATRES (1) |
| low | `ElordendeMelchisedech` | GONZALEZDEBARCIA | 56 | 8/56 (14%) | 1.15 | GONZALEZDEBARCIA (8), LANINI (8), MULSA (8), CANIZARES (7), CAXESI (4) |
| low | `JuanBautistaLopez_MilagrosoimposibleySantaRitade` | GOMEZACOSTA | 70 | 12/70 (17%) | 1.14 | GOMEZACOSTA (12), VIDALYSALVADOR (12), CASTROYSALAZAR (8), GILENRIQUEZ (8), CASTILLOSOLORZANO (4) |
| low | `GaspardeMesa_Niniveysuconversion` | MIRACLESSOTOMAYOR | 81 | 15/81 (18%) | 1.12 | MIRACLESSOTOMAYOR (15), TAMAYO (13), ROJASVILLANDRANDO (12), MESA (10), AVELLANEDA (3) |
| low | `SALAZAR_JuegosOlimpicos` | SANDOVAL | 116 | 35/116 (30%) | 1.11 | SANDOVAL (35), VERATASSIS (31), LEIVARAMIREZ (27), BATRES (6), BELMONTE (4) |
| low | `PAZ_HijaDelSerafinYTerceraDeToledo` | CALLE | 139 | 32/139 (23%) | 1.10 | CALLE (32), VIDALYSALVADOR (30), GARCIAMARCOS (28), PAREDES (7), GONGORA (5) |
| low | `POLOP_CALDERON_Pandera` | CASTILLOSOLORZANO | 22 | 8/22 (36%) | 1.10 | CASTILLOSOLORZANO (8), GARCIADEPRADO (7), VIDALYSALVADOR (2), CERVANTES (1), HOZYMOTA (1) |
| low | `VILLAIZAN_CallarloQueNoDecirlo` | HURTADODEMENDOZA | 41 | 25/41 (61%) | 1.10 | HURTADODEMENDOZA (25), VELEZ (3), GARCIADEPRADO (3), QUINONES (2), QUEVEDO (2) |
| low | `FernandodeLudena_RelojesLos` | JIMENEZSEDENO | 14 | 2/14 (14%) | 1.10 | JIMENEZSEDENO (2), MOLINAYMENDOZA (2), ROMEROROQUE (1), GARCIADEPRADO (1), CECILIANACIMIENTO (1) |
| low | `COUTOPESTANA_COPIAAMENO_HechizoDeAmorLosCelos` | CASTILLOSOLORZANO | 151 | 60/151 (40%) | 1.09 | CASTILLOSOLORZANO (60), VIDALYSALVADOR (48), ROMEROROQUE (11), PAREDES (9), CASTROYSALAZAR (7) |
| low | `CubillodeAragonAlvaro_MuertedeFrislanLa` | GARCIAMARCOS | 29 | 11/29 (38%) | 1.09 | GARCIAMARCOS (11), CORDERO (5), ROMEROROQUE (2), TAMAYO (1), PAREDES (1) |
| low | `VIDAL_PacesDeIngenioYBelleza` | CASTILLOSOLORZANO | 128 | 52/128 (41%) | 1.09 | CASTILLOSOLORZANO (52), PAREDES (34), GARCIAMARCOS (6), ENRIQUEZ (6), LANINI (5) |
| low | `FelipeSanchezCarralero_Loaalnacimientodenuestroredent` | GARCIAMARCOS | 18 | 7/18 (39%) | 1.08 | GARCIAMARCOS (7), GONZALEZDEBARCIA (2), PAREDES (2), LEONORCUEVA (1), MELO (1) |
| low | `SEPULVEDA_ComediadeSepulveda` | LICENCIADOROJAS | 101 | 33/101 (33%) | 1.08 | LICENCIADOROJAS (33), SANTATERESA (23), MESA (8), REMON (7), AVELLANEDADELACUEVA (5) |
| low | `TomasManueldePazAtribuido_JuegodelamantaEl` | PAREDES | 16 | 3/16 (19%) | 1.07 | PAREDES (3), GONZALEZDEBARCIA (2), LEONORCUEVA (1) |
| low | `LuisdeBelmonteBermudezMoretoyC_RenegadadeValladolidLacautivad` | LEIVARAMIREZ | 68 | 28/68 (41%) | 1.06 | LEIVARAMIREZ (28), BATRES (14), ROSETENINO (3), TORRESLORENZODE (3), ROJASZORRILLA (2) |
| low | `ClaramonteAndresde_Escarraman` | ENRIQUEZ | 44 | 29/44 (66%) | 1.06 | ENRIQUEZ (29), CERVANTES (4), CASTILLOSOLORZANO (3), BATRES (2), QUINONES (2) |
| low | `HURTADO_Quererporsoloquerer_acto1y3` | GONGORA | 186 | 55/186 (30%) | 1.05 | GONGORA (55), MELO (43), CASTROYSALAZAR (43), AVELLANEDADELACUEVA (16), SARAVIAYMENDOZA (13) |
| low | `CuadernoDeNotas-II-1586` | LOPEZDECASTRO | 264 | 81/264 (31%) | 1.05 | LOPEZDECASTRO (81), GONZALEZDETORRES (41), AGUADOELVIEJO (18), MULSA (18), MIRACLESSOTOMAYOR (16) |
| low | `JosedelVillar_RondadelalcaldeLa` | LEIVARAMIREZ | 16 | 3/16 (19%) | 1.05 | LEIVARAMIREZ (3), BELMONTE (2), LICENCIADOROJAS (1), SANDOVAL (1) |
| low | `SaenzdeTejeraJuanFrancisco_MinuefrancesEl` | ANDOSILLA | 14 | 1/14 (7%) | 1.04 | ANDOSILLA (1), CLARAMONTE (1), VELEZ (1), GONZALEZDEBARCIA (1) |
| low | `AVILA_Sintitulo` | AVELLANEDA | 52 | 15/52 (29%) | 1.04 | AVELLANEDA (15), CECILIANACIMIENTO (10), ENRIQUEZ (9), BARREDA (5), VARGASMACHUCA (5) |
| low | `ENRIQUEZGOMEZ_SantaTaez1` | CARVAJAL | 68 | 13/68 (19%) | 1.04 | CARVAJAL (13), ROJASVILLANDRANDO (11), LOPEZDECARDENA (8), CASTILLOSOLORZANO (7), VALDIVIELSO (4) |
| low | `MORALES_Academiasdeamor` | LOPEZDELCAMPO | 23 | 15/23 (65%) | 1.02 | LOPEZDELCAMPO (15), GOMEZACOSTA (3), VIDALYSALVADOR (1), VARGASMACHUCA (1), BANCESCANDAMO (1) |
| low | `LuisdeBelmonteBermudez_Darlesconlaentretenida` | ENRIQUEZ | 56 | 23/56 (41%) | 1.02 | ENRIQUEZ (23), MEDINA (6), TORRESLORENZODE (2), FAJARDOYACEVEDO (2), VARGAS (2) |
| low | `TELLEZ_ArbolDeMejorFruto` | HOZYMOTA | 61 | 8/61 (13%) | 1.01 | HOZYMOTA (8), PSEUDOHURTADODEMENDOZA (7), LEIVARAMIREZ (6), BATRES (6), MULSA (4) |
| low | `MiradeAmescuaAntonio_FedeHungriaLa` | GARCIAMARCOS | 33 | 14/33 (42%) | 1.01 | GARCIAMARCOS (14), LEIVARAMIREZ (8), SANDOVAL (2), LICENCIADOROJAS (1), JIMENEZSEDENO (1) |
| low | `AntonioFranciscodeFlores_Nohayquecreerenaguerosylasestr` | GARCIAMARCOS | 84 | 33/84 (39%) | 1.01 | GARCIAMARCOS (33), VIDALYSALVADOR (15), JIMENEZSEDENO (6), MOLINAYMENDOZA (5), SANDOVAL (4) |
| low | `MiradeAmescuaAntonio_RicoavarientoAutosacramentalEl` | ANDOSILLA | 29 | 9/29 (31%) | 1.01 | ANDOSILLA (9), QUINONES (9), CARVAJAL (2), LORENZANA (1), FAJARDOYACEVEDO (1) |
| low | `SAMATHEO_DonaJimena` | CONTRERAS | 23 | 11/23 (48%) | 1.00 | CONTRERAS (11), AGUADOELVIEJO (6), MORETO (2), SANTATERESA (1), MULSA (1) |
| low | `AgustindeSalazaryTorres_CircunstanciaLa` | GONGORA | 54 | 25/54 (46%) | 1.00 | GONGORA (25), ROMEROROQUE (7), HURTADODEMENDOZA (6), CANIZARES (4), CASTROYSALAZAR (3) |
| low | `ARGENSOLA_Codigo` | VARGASMACHUCA | 277 | 122/277 (44%) | 1.00 | VARGASMACHUCA (122), QUEVEDO (71), BENAVIDES (34), BATRES (15), CERVANTES (8) |
| low | `FranciscoAntoniodeCastroySalaz_RetooeldesafioEl` | LICENCIADOROJAS | 12 | 2/12 (17%) | 1.00 | LICENCIADOROJAS (2), HURTADODEMENDOZA (1), GALLEGOS (1), MOLINAYMENDOZA (1), ROMEROROQUE (1) |
| low | `PEREZ_PuertoDeSanLucar_British` | CASTILLOSOLORZANO | 32 | 13/32 (41%) | 0.99 | CASTILLOSOLORZANO (13), MORETO (10), LEIVARAMIREZ (5), ZABALETA (1), BOLEAYALVARADO (1) |
| low | `GodinezManriqueFelipeAtribuido_SoldadodelcieloEl` | CERVANTES | 109 | 25/109 (23%) | 0.99 | CERVANTES (25), CARVAJAL (17), CASTILLOSOLORZANO (15), AMESCUA (12), GARCIADEPRADO (10) |
| low | `FERNANDEZ_PatronadeToledoSantaLeocadiaLa` | GARCIADEPRADO | 48 | 20/48 (42%) | 0.95 | GARCIADEPRADO (20), VIDALYSALVADOR (13), CANIZARES (4), CALDERON (4), HURTADODEMENDOZA (2) |
| low | `CASTRO_NuncaElBienHacer` | ENRIQUEZ | 114 | 46/114 (40%) | 0.95 | ENRIQUEZ (46), BELMONTE (30), QUEVEDO (12), CECILIANACIMIENTO (3), VIDALYSALVADOR (2) |
| low | `ORTIZ_NuestraSenoraDeSopetran` | CARVAJAL | 43 | 15/43 (35%) | 0.95 | CARVAJAL (15), ENRIQUEZ (13), ROMEROROQUE (6), CERVANTES (5), CASTILLOSOLORZANO (1) |
| low | `BARQUEZ_SalvajeamericanoEl` | JUANDESOTO | 69 | 27/69 (39%) | 0.95 | JUANDESOTO (27), CALLE (12), TORRESLORENZODE (9), LEIVARAMIREZ (6), LLOBREGATYESTEVE (6) |
| low | `AVILA_Eglogainterlocutoria` | GONGORA | 40 | 29/40 (72%) | 0.94 | GONGORA (29), CERVANTES (9), SARAVIAYMENDOZA (2) |
| low | `GOMEZDETEJADA_NinoPerdido` | LOPEZDECASTRO | 21 | 4/21 (19%) | 0.91 | LOPEZDECASTRO (4), TORRESLORENZODE (3), MEDINA (3), JUANDESOTO (2), CONTRERAS (1) |
| low | `VegaCarpioLopede_ViudavalencianaLa` | JUANDESOTO | 127 | 38/127 (30%) | 0.91 | JUANDESOTO (38), CALLE (21), LEIVARAMIREZ (14), CASTILLOSOLORZANO (13), BENAVIDES (6) |
| low | `MojigangadeRojillas` | VIDALYSALVADOR | 12 | 2/12 (17%) | 0.90 | VIDALYSALVADOR (2), BANCESCANDAMO (1), GONZALEZDEBARCIA (1), GODINEZMANRIQUE (1), CERVANTES (1) |
| low | `PoesiaGREGORIAFRANCISCA` | LOPEZDECARDENA | 212 | 166/212 (78%) | 0.88 | LOPEZDECARDENA (166), CUEVAYSILVA (17), LICENCIADOROJAS (10), AVELLANEDA (7), BANCESCANDAMO (2) |
| low | `JuanSanchez_CercodeTunezyganadelaGoletapor` | VERATASSIS | 108 | 33/108 (31%) | 0.87 | VERATASSIS (33), CALLE (29), JIMENEZSEDENO (11), SARAVIAYMENDOZA (9), AVELLANEDADELACUEVA (4) |
| low | `LOA_CirconcisionIesuChristo` | JIMENEZSEDENO | 13 | 12/13 (92%) | 0.87 | JIMENEZSEDENO (12), LANINI (1) |
| low | `MoretoyCavanaAgustin_MariquitaLa` | TAMAYO | 12 | 1/12 (8%) | 0.86 | TAMAYO (1), VARGAS (1), PAREDES (1), GONZALEZDEBARCIA (1), QUINONES (1) |
| low | `Entredosmujeres` | LICENCIADOROJAS | 14 | 1/14 (7%) | 0.86 | LICENCIADOROJAS (1), CASTILLOSOLORZANO (1), ROJASZORRILLA (1), LORENZANA (1), CAXESI (1) |
| low | `GodinezManriqueFelipe_DivinoIsaacEl` | CERVANTES | 65 | 16/65 (25%) | 0.85 | CERVANTES (16), COELLO (9), QUINONES (7), BATRES (3), CARVAJAL (3) |
| low | `AntonioEnriquezGomez_ConversiondelaMagdalenaosantaM` | VIDALYSALVADOR | 50 | 12/50 (24%) | 0.85 | VIDALYSALVADOR (12), CORDERO (10), MORETO (5), VALDIVIELSO (2), CANIZARES (2) |
| low | `JoseLanderasyVelasco_MeriendadeshechaLa` | GARCIADEPRADO | 22 | 6/22 (27%) | 0.84 | GARCIADEPRADO (6), CERVANTES (5), GONZALEZDEBARCIA (3), CANIZARES (2), CONTRERAS (2) |
| low | `JeronimodeCancerAtribuidoCalde_PelicanoyelratonEl` | VIDALYSALVADOR | 14 | 2/14 (14%) | 0.84 | VIDALYSALVADOR (2), LICENCIADOROJAS (1), GONZALEZDEBARCIA (1), SANDOVAL (1), CONTRERAS (1) |
| low | `RECUEIL_poesies` | ENRIQUEZ | 343 | 146/343 (43%) | 0.84 | ENRIQUEZ (146), MEDINA (57), GARCIAMARCOS (25), VARGAS (21), TORRESLORENZODE (15) |
| low | `VIOLANTE_CancionReina` | VARGASMACHUCA | 3 | 2/3 (67%) | 0.84 | VARGASMACHUCA (2), GONGORA (1) |
| low | `EngaoshayquesonjustosysegundoReydeRoma` | BOLEAYALVARADO | 59 | 9/59 (15%) | 0.83 | BOLEAYALVARADO (9), VIDALYSALVADOR (9), ALARCON (8), CASTROYSALAZAR (6), GILENRIQUEZ (3) |
| low | `VegaCarpioLopede_VillanodespojadoEl` | LEIVARAMIREZ | 25 | 8/25 (32%) | 0.83 | LEIVARAMIREZ (8), GALLEGOS (4), CARVAJAL (2), ROMEROROQUE (2), JUANDESOTO (2) |
| low | `DarbienpormalElrespetoalsacerdoteySacrilegiovengado` | BATRES | 61 | 10/61 (16%) | 0.83 | BATRES (10), GARCIAMARCOS (7), CASTILLOSOLORZANO (7), ENRIQUEZ (4), PAREDES (3) |
| low | `SOLORZANO_CLARAMONTE_ROJASZORRILLA_DonGilDeLaMancha` | VALDIVIELSO | 104 | 45/104 (43%) | 0.82 | VALDIVIELSO (45), MONTALBAN (35), BELMONTE (3), QUINONES (2), CONTRERAS (1) |
| low | `SebastianAntoniodeGadeayOviedo_TesorodelaiglesiaEl` | FAJARDOYACEVEDO | 33 | 9/33 (27%) | 0.82 | FAJARDOYACEVEDO (9), ALARCON (3), GONZALEZDEBARCIA (2), CASTILLOSOLORZANO (2), JUANDESOTO (2) |
| low | `ARROYOYVELASCO_LoaMasJustoReyDeGrecia` | CONTRERAS | 12 | 10/12 (83%) | 0.81 | CONTRERAS (10), CERVANTES (2) |
| low | `ALEMAN_Expediente_informacionlicencia` | CUEVAYSILVA | 15 | 6/15 (40%) | 0.81 | CUEVAYSILVA (6), ENRIQUEZ (3), REMON (1), LICENCIADOROJAS (1), QUEVEDO (1) |
| low | `QUINONESDEBENAVENTE_CelosdeJoanFrances` | MATOSFRAGOSO | 16 | 4/16 (25%) | 0.80 | MATOSFRAGOSO (4), MESA (4), VELEZ (2), VIDALYSALVADOR (1), REMON (1) |
| low | `MENDESDEHARO_EnganoVictoria` | SANDOVAL | 9 | 2/9 (22%) | 0.79 | SANDOVAL (2), PAREDES (2), MORETO (2), MELO (1), ROMEROROQUE (1) |
| low | `LabatalladelAmor` | LEIVARAMIREZ | 31 | 6/31 (19%) | 0.79 | LEIVARAMIREZ (6), GARCIAMARCOS (6), SARAVIAYMENDOZA (2), CORDERO (2), TIRSO (2) |
| low | `QuirosJuande_FamosatoledanaLaBNE` | VARGASMACHUCA | 125 | 47/125 (38%) | 0.79 | VARGASMACHUCA (47), SANDOVAL (41), AVELLANEDA (10), VALDIVIELSO (8), VERATASSIS (7) |
| low | `MonteserFranciscoAntoniode_BallenaLa` | HURTADODEMENDOZA | 17 | 2/17 (12%) | 0.78 | HURTADODEMENDOZA (2), TORRESLORENZODE (1), QUINONES (1), GODINEZMANRIQUE (1), CLARAMONTE (1) |
| low | `VILLALPANDO_Convitegeneral` | LICENCIADOROJAS | 116 | 78/116 (67%) | 0.78 | LICENCIADOROJAS (78), CERVANTES (37), SANDOVAL (1) |
| low | `FelipeSicardo_Lomasessabervencerse` | ROMEROROQUE | 66 | 17/66 (26%) | 0.77 | ROMEROROQUE (17), FBQUIROS (11), GONGORA (6), HURTADODEMENDOZA (6), CANIZARES (6) |
| low | `QUINONESDEBENAVENTE_LadronesYMoroHueco` | AGUADOELVIEJO | 13 | 9/13 (69%) | 0.77 | AGUADOELVIEJO (9), MULSA (2), MORETO (1), CUENCAYARGUELLO (1) |
| low | `CubillodeAragonAlvaro_BandolerodeFlandesEl` | GONZALEZDEBARCIA | 58 | 11/58 (19%) | 0.77 | GONZALEZDEBARCIA (11), GARCIADEPRADO (9), HOZYMOTA (7), CASTILLOSOLORZANO (5), BATRES (4) |
| low | `FLOREZ_VenenoEnLaHermosura` | TORRESLORENZODE | 58 | 14/58 (24%) | 0.76 | TORRESLORENZODE (14), HOZYMOTA (11), CASTROYSALAZAR (10), LLOBREGATYESTEVE (8), LORENZANA (4) |
| low | `QUINONESDEBENAVENTE_LadronesYReloj` | CASTILLOSOLORZANO | 17 | 13/17 (76%) | 0.76 | CASTILLOSOLORZANO (13), GONZALEZDEBARCIA (1), JIMENEZSEDENO (1) |
| low | `AGUADO_Ermitano` | LEONORCUEVA | 16 | 5/16 (31%) | 0.76 | LEONORCUEVA (5), VIDALYSALVADOR (5), CASTILLOSOLORZANO (4) |
| low | `QUINONESDEBENAVENTE_SacristanesCosquillasYTalegote` | HURTADODEMENDOZA | 10 | 7/10 (70%) | 0.75 | HURTADODEMENDOZA (7), GRACIAN (2), AMESCUA (1) |
| low | `MATOS_JenizanoHungria_LaLaguna` | MELO | 12 | 3/12 (25%) | 0.75 | MELO (3), ROMEROROQUE (2), ONAVIEDMAYTORRES (1), LOPEZDECASTRO (1), GONGORA (1) |
| low | `PARIS_JacaraEnEsdrujulos_Institut` | CASTILLOSOLORZANO | 13 | 9/13 (69%) | 0.73 | CASTILLOSOLORZANO (9), VIDALYSALVADOR (3), AMESCUA (1) |
| low | `TURIA_BeligeraEspanyola` | ENRIQUEZ | 46 | 13/46 (28%) | 0.73 | ENRIQUEZ (13), REMON (7), CERVANTES (6), CARVAJAL (5), LORENZANA (4) |
| low | `POLOP_HidalgoteDeJaca_Autografo` | VARGASMACHUCA | 169 | 34/169 (20%) | 0.71 | VARGASMACHUCA (34), GONGORA (27), CASTILLOSOLORZANO (26), BATRES (11), CALLE (10) |
| low | `DiegoJuandeVeraTassisyVillarro_Baileteflorentin` | VERATASSIS | 25 | 2/25 (8%) | 0.71 | VERATASSIS (2), CASTILLOSOLORZANO (1), AMESCUA (1), MARCHANTE (1) |
| low | `RUIZ_Orfeo` | AVELLANEDA | 15 | 7/15 (47%) | 0.71 | AVELLANEDA (7), VALDIVIELSO (2), VIDALYSALVADOR (1), MELO (1), GONGORA (1) |
| low | `QuirosFranciscoBernardode_MantaLa` | GONZALEZDEBARCIA | 14 | 3/14 (21%) | 0.71 | GONZALEZDEBARCIA (3), BATRES (2) |
| low | `HIDALGO_LoaAlNacimientoDeDios` | CONTRERAS | 4 | 1/4 (25%) | 0.71 | CONTRERAS (1), MELO (1), CASTROYSALAZAR (1), BELMONTE (1) |
| low | `FranciscoAntoniodeBancesCandam_DuelocontrasudamaEl` | LOPEZDECARDENA | 101 | 23/101 (23%) | 0.69 | LOPEZDECARDENA (23), ENRIQUEZ (17), VERATASSIS (17), VALDIVIELSO (10), MARCHANTE (9) |
| low | `JuanEstebanAtribuido_DesposoriosdelaVirgenynacimien` | MELO | 59 | 10/59 (17%) | 0.69 | MELO (10), SANDOVAL (9), VARGASMACHUCA (7), FAJARDOYACEVEDO (6), SARAVIAYMENDOZA (6) |
| low | `ABEC_PapeldeGracejo` | VIDALYSALVADOR | 3 | 2/3 (67%) | 0.69 | VIDALYSALVADOR (2), VARGASMACHUCA (1) |
| low | `RAMOSDELCASTILLO_Autosacramental_sintitulo` | GARCIADEPRADO | 23 | 11/23 (48%) | 0.69 | GARCIADEPRADO (11), VIDALYSALVADOR (5), CALLE (2), LEONORCUEVA (1), QUINONES (1) |
| low | `Lomejoreslomejor` | MONTALBAN | 95 | 29/95 (30%) | 0.68 | MONTALBAN (29), VIDALYSALVADOR (20), CANIZARES (20), MORETO (14), ROJASZORRILLA (2) |
| low | `LOA_FestividadNuestraSenoraRozario` | JIMENEZSEDENO | 9 | 7/9 (78%) | 0.68 | JIMENEZSEDENO (7), MOLINAYMENDOZA (2) |
| low | `TitulosComedias1714` | VIDALYSALVADOR | 4 | 1/4 (25%) | 0.65 | VIDALYSALVADOR (1), VERATASSIS (1), MARCHANTE (1), SARAVIAYMENDOZA (1) |
| low | `MatosFragosoJuandeAtribuido_Jacaraentredosmujeres` | VALDIVIELSO | 23 | 2/23 (9%) | 0.64 | VALDIVIELSO (2), LICENCIADOROJAS (1), CASTILLOSOLORZANO (1), VIDALYSALVADOR (1) |
| low | `GARCILASO_cartasecretarioCobos` | REMON | 4 | 2/4 (50%) | 0.64 | REMON (2), QUEVEDO (1) |
| low | `JosedeValdivielso_FeriasdelalmaLas` | ROMEROROQUE | 28 | 8/28 (29%) | 0.64 | ROMEROROQUE (8), CARVAJAL (6), RUIZALCEO (4), MULSA (2), JUANDESOTO (2) |
| low | `ENRIQUEZGOMEZ_VisitaDeLosPresos` | VALDIVIELSO | 20 | 8/20 (40%) | 0.64 | VALDIVIELSO (8), HURTADODEMENDOZA (7), CONTRERAS (2), SANTATERESA (1) |
| low | `LeonMerchanteoMarchanteJuanMan_Jacaraentremesada` | LORENZANA | 13 | 1/13 (8%) | 0.64 | LORENZANA (1), CARVAJAL (1), CAXESI (1), MIRACLESSOTOMAYOR (1) |
| low | `VIOLANTE_SilvaCristo` | GONGORA | 2 | 1/2 (50%) | 0.63 | GONGORA (1), GARCIADEPRADO (1) |
| low | `LANCELOTO_Musicostontos` | VIDALYSALVADOR | 11 | 4/11 (36%) | 0.61 | VIDALYSALVADOR (4), VARGASMACHUCA (3), ENRIQUEZ (1), QUEVEDO (1), PAREDES (1) |
| low | `MONROYYSILVA_MudanzasFortunayFirmezasAmor` | HURTADODEMENDOZA | 52 | 24/52 (46%) | 0.60 | HURTADODEMENDOZA (24), BELMONTE (8), QUEVEDO (6), GARCIADEPRADO (4), QUINONES (2) |
| low | `LorenzodelasLlamosas_Tambiensevenganlosdioses` | AVELLANEDA | 233 | 142/233 (61%) | 0.58 | AVELLANEDA (142), CERVANTES (52), LICENCIADOROJAS (19), VERATASSIS (3), GONZALEZDEBARCIA (2) |
| low | `VALLADARES_GaleoteCautivo` | SANDOVAL | 144 | 64/144 (44%) | 0.57 | SANDOVAL (64), VERATASSIS (36), CERVANTES (11), AVELLANEDA (8), LEONORCUEVA (3) |
| low | `SALVO_Posturas` | AGUADOELVIEJO | 11 | 6/11 (55%) | 0.56 | AGUADOELVIEJO (6), CONTRERAS (3), LOPEZDECASTRO (1), MULSA (1) |
| low | `CASTRO_MocedadesHazanasCid` | VERATASSIS | 152 | 88/152 (58%) | 0.56 | VERATASSIS (88), SANDOVAL (39), MELO (14), GONGORA (6), GILENRIQUEZ (3) |
| low | `AntonioHurtadodeMendoza_Medicodeespiritusegundapartede` | AVELLANEDADELACUEVA | 20 | 3/20 (15%) | 0.55 | AVELLANEDADELACUEVA (3), ROMEROROQUE (2), LICENCIADOROJAS (1), HURTADODEMENDOZA (1), CERVANTES (1) |
| low | `BienNacidoEncubierto_Lope` | CARVAJAL | 127 | 40/127 (32%) | 0.53 | CARVAJAL (40), CASTILLOSOLORZANO (18), GONGORA (17), GARCIADEPRADO (16), CERVANTES (8) |
| low | `YANEZdeOrteaga_Gedeodivinohumano` | CERVANTES | 91 | 53/91 (58%) | 0.50 | CERVANTES (53), LICENCIADOROJAS (36), LOPEZDECARDENA (1), ROJASVILLANDRANDO (1) |
| low | `MOTASILVA_VerdugosdesusangreLos` | SANDOVAL | 144 | 42/144 (29%) | 0.49 | SANDOVAL (42), JUANDESOTO (15), VARGAS (14), MEDINA (12), LOPE (11) |
| low | `AntoniodeZamoraAtribuido_JuegodelasortijaFindefiestaEl` | BELMONTE | 12 | 4/12 (33%) | 0.47 | BELMONTE (4), LEONORCUEVA (1), GONZALEZDEBARCIA (1), HURTADODEMENDOZA (1), GONGORA (1) |
| low | `CALDERONatribuido_UniversalRedencion` | LICENCIADOROJAS | 60 | 37/60 (62%) | 0.47 | LICENCIADOROJAS (37), CERVANTES (23) |
| low | `AYALA_ZarzuelaDeQuintoElementoEsAmor` | CASTILLOSOLORZANO | 14 | 7/14 (50%) | 0.46 | CASTILLOSOLORZANO (7), JIMENEZSEDENO (3), CONTRERAS (2), VIDALYSALVADOR (1) |
| low | `ENRIQUEZGOMEZ_EnganarParaReinar` | HURTADODEMENDOZA | 28 | 11/28 (39%) | 0.45 | HURTADODEMENDOZA (11), QUEVEDO (6), BELMONTE (3), VELEZ (2), GONGORA (2) |
| low | `MOTASILVA_DesposoriosentremuertosLos` | MONTALBAN | 157 | 38/157 (24%) | 0.43 | MONTALBAN (38), VARGAS (16), JUANDESOTO (13), LOPE (12), VERATASSIS (11) |
| low | `NIETO_LoaPisa` | CERVANTES | 21 | 6/21 (29%) | 0.42 | CERVANTES (6), BENAVIDES (3), VARGASMACHUCA (2), QUEVEDO (2), SANTATERESA (1) |
| low | `AntonioEnriquezGomez_ZapateroydonTerencioCatalanaEl` | VIDALYSALVADOR | 20 | 4/20 (20%) | 0.42 | VIDALYSALVADOR (4), GONGORA (3), MELO (3), VERATASSIS (2), VARGASMACHUCA (2) |
| low | `LOA_CaballeroDama` | JIMENEZSEDENO | 10 | 4/10 (40%) | 0.40 | JIMENEZSEDENO (4), LANINI (2), GARCIAMARCOS (1), PAREDES (1), AVELLANEDADELACUEVA (1) |
| low | `VIOLANTE_Carta_autografo` | VARGASMACHUCA | 2 | 2/2 (100%) | 0.38 | VARGASMACHUCA (2) |
| low | `Elricoavarientoautosacramental` | RUIZALCEO | 29 | 7/29 (24%) | 0.37 | RUIZALCEO (7), CUEVAYSILVA (5), GARCIAMARCOS (5), MIRACLESSOTOMAYOR (1), CERVANTES (1) |
| low | `NIETO_LoaLivorno` | QUEVEDO | 14 | 6/14 (43%) | 0.36 | QUEVEDO (6), SANDOVAL (3), VARGASMACHUCA (3), JIMENEZSEDENO (1) |
| low | `GilLopezdeArmestoyCastro_BorrachosLos` | SANDOVAL | 14 | 2/14 (14%) | 0.35 | SANDOVAL (2), LEIVARAMIREZ (1), CALLE (1) |
| low | `Saineteparaintroducirunsaraofrances` | MOLINAYMENDOZA | 13 | 1/13 (8%) | 0.33 | MOLINAYMENDOZA (1), ROMEROROQUE (1), GONZALEZDEBARCIA (1), GONGORA (1) |
| low | `FERNANDEZ_Comedia_Hisp` | GONGORA | 28 | 17/28 (61%) | 0.32 | GONGORA (17), SARAVIAYMENDOZA (4), CERVANTES (4), CASTILLOSOLORZANO (3) |
| low | `SOLIS_PicoYCanente` | TAMAYO | 19 | 11/19 (58%) | 0.32 | TAMAYO (11), VALDIVIELSO (4), HURTADODEMENDOZA (2), AVELLANEDA (1), SANTATERESA (1) |
| low | `BERMUDEZCALDERON_Europa_British` | VARGASMACHUCA | 182 | 99/182 (54%) | 0.32 | VARGASMACHUCA (99), SANTATERESA (16), CECILIANACIMIENTO (16), GONGORA (13), CERVANTES (11) |
| low | `BERMUDEZCALDERON_MayorEsquilador_British` | VARGASMACHUCA | 162 | 79/162 (49%) | 0.30 | VARGASMACHUCA (79), GONGORA (17), VERATASSIS (17), SANDOVAL (13), ONAVIEDMAYTORRES (6) |
| low | `ROJO_LoaCompaniaVallejo` | GRACIAN | 13 | 6/13 (46%) | 0.28 | GRACIAN (6), MULSA (2), AMESCUA (2), HURTADODEMENDOZA (2), CONTRERAS (1) |
| low | `FERNANDEZ_Dialogoparacantar` | GONGORA | 7 | 4/7 (57%) | 0.26 | GONGORA (4), SARAVIAYMENDOZA (2), CERVANTES (1) |
| low | `VILLAMEDIANA_PoesiasVarias` | SANDOVAL | 419 | 161/419 (38%) | 0.24 | SANDOVAL (161), VERATASSIS (63), ENRIQUEZ (43), GONGORA (22), LEONORCUEVA (14) |
| low | `CIFUENTES_LoMasPrivaLoMenos` | GARCIADEPRADO | 33 | 7/33 (21%) | 0.23 | GARCIADEPRADO (7), HURTADODEMENDOZA (5), QUEVEDO (5), GALLEGOS (4), BELMONTE (4) |
| low | `FranciscoAntoniodeBancesCandam_MojigangaparaelautoElprimerdue` | GONZALEZDEBARCIA | 16 | 2/16 (12%) | 0.22 | GONZALEZDEBARCIA (2), BANCESCANDAMO (1), VIDALYSALVADOR (1), COELLO (1), GARCIADEPRADO (1) |
| low | `FranciscodeLeivaRamirezdeArell_EnsayoEl` | ANDOSILLA | 9 | 3/9 (33%) | 0.19 | ANDOSILLA (3), CASTILLOSOLORZANO (1), QUINONES (1), CANIZARES (1) |

