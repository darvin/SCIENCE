# Text pattern classification in large corpus of text

I have a large dataset that is a PDF files of the books of few different Tabletop roleplaying games. I have a few long text files that contain 

, a text file that conain a copy paste of the glossaries from those books, like that:


```
Ability Scores - Numerical ratings ranging from 3-18 for a character’s strength, intelligence, wisdom, constitution,dexterity, and charisma. ADBD - ADVANCED DUNGEONS8 d r a g o n s TM
Alignment - A general description of a character’s behaviorial and ethical tendencies nomed by a combination of Law, Neutrality, or Chaos with Good, Neutrality, or Evil.
Armor Class - A number representing the relative protection from harm the character will enjoy. This includes type of armor, dexterity bonuses or penalties, magical protections,etc.
Artifact-A magical item of tremendouspower, fabricated in the distantpast.
Astral - Pertaining to or within the Astral Plane (see PHB, p. 120).Not the same as ethereal (q.v.) . Bok- 1.Missilefromacrossbow.2.Barlockingadoor.3.Streakoflightning.4.Toflee.
Breath Weapon - Special attack of certain creatures like dragons, chimerae, etc. causing any of several different effects. For saving throw purposes the ”Breath We-apon” category excludes petrification and polymorph results, which have their own category.
```



, and a text file that contains a copy paste of player's characters from those books, like that:


```
Character Name: Kastala the Scarred Player Name________________________________________
Character Type: Human Archetype: Psyker
Character History: Kastala grew up in one of the the warring tribes of the feral world of Iocanthos in the Calixis Sector. An orphan, she barely survived as an unwanted outcast. However, early in life she learned she could sense a blow’s impact just before it hit. Kastala stopped avoiding
the beatings from the tribe’s warriors. Though this earned her many scars, it also honed her power until she could dodge any blow. The warriors’ derision turned to awe, then terror when she began summoning vicious bolts of darkness to consume any who dared raise a hand against her. Kastala rose from outcast to avatar of destruction, carving a bloody swath through Iocanthos before being noticed and captured by the Inquisition. Pride: Foresight Failing: Wrath Motivation: Ascendancy
Weapon Skill Ballistic Skill Strength Toughness Agility Intelligence Perception Willpower Fellowship Infamy (WS) (BS) (S) (T) (Ag) (Int) (Per) (WP) (Fel) (Inf)
29 3 2 2 8 3 1 3 3 3 2 4 8 5 0 2 9 3 0
  Awareness (Per)
xooo
Dodge (Ag) Scrutiny (Per)
xooo xxxo
SKILLS
 Playing Kastala the scarred
Kastala is a quiet woman, but prone to violent rage when threatened. Her most notable feature is her singular force of will, which since her earliest memories is bent towards survival. Of course, now she has tasted the gifts the warp has to offer, and knows that true survival can only be found in its embrace. She wants to live long enough to grow in power, until nothing can destroy her.
Kastala has no qualms about working with others. However, if they ever threaten her, she’ll burn them down immediately.
 Forbidden Lore (Warp) (Int)







  CharaCter Name _S_e_r_g_e_an__t _A_d_r_i_n_e_O__sp__ar_n_________________ Player Name _________________________________ regimeNt _C__a_d_ia_n__9_9_t_h_M__e_c_h_a_n_i_se_d__I_n_fa_n_t_r_y________________ SPeCiality _S_e_r_g_e_a_n_t____________________________
DemeaNour __H_e_r_o_i_c_________________________________________ DeSCriPtioN _A_s_h_re_w_d__ta_c_ti_ci_an__a_n_d_d_ef_t_so_l_di_e_r,_A_d_r_in_e_O_s_p_a_rn__w_o_n_ _so_m_e__re_n_ow__n_in__th_e_r_eg_i_m_e_nt_a_f_te_r_le_a_d_in_g_a__sq_u_a_d_to__ro_u_t_se_v_e_ra_l_D_a_r_k_E_l_da_r_p_a_t_ro_l_s_on__K_a_lf_._D_e_sp_it_e_th_i_s_m_i_no_r_f_a_m_e,_O__sp_a_r_n_r_em_a_i_n_s



 CharaCter Name _ANOTHER CHARACTER________________ Player Name _________________________________ regimeNt _C__a_d_ia_n__9_9_t_h_M__e_c_h_a_n_i_se_d__I_n_fa_n_t_r_y________________ SPeCiality _S_e_r_g_e_a_n_t____________________________
DemeaNour __H_e_r_o_i_c_________________________________________ DeSCriPtioN _A_s_h_re_w_d__ta_c_ti_ci_an__a_n_d_d_ef_t_so_l_di_e_r,_A_d_r_in_e_O_s_p_a_rn__w_o_n_ _so_m_e__re_n_ow__n_in__th_e_r_eg_i_m_e_nt_a_f_te_r_le_a_d_in_g_a__sq_u_a_d_to__ro_u_t_se_v_e_ra_l_D_a_r_k_E_l_da_r_p_a_t_ro_l_s_on__K_a_lf_._D_e_sp_it_e_th_i_s_m_i_no_r_f_a_m_e,_O__sp_a_r_n_r_em_a_i_n_s
```



, copy paste of the pages that contain monsters, like that:

```
   Character Name: Babaroth Player Name________________________________________
Character Type: Chaos Space Marine Archetype: Chosen
Character History: Babaroth is a terrifying figure, a towering berserker in the blood-red armour of the dreaded World Eaters legion. Whether or not he is truly one of these ancient warriors is an open question, for none have worked up the courage to ask him. Babaroth has long served with warbands travelling out of the Eye of Terror. He is always content to follow the orders of other leaders, though his only desire is slaughter, and his only allegiance is to the deity he sees as his patron: Khorne, the Blood God. Babaroth was captured by a concerted Inquisitorial effort. They hope severe psychic interrogation could provide valuable information that would offset the loss of a company of Guardsmen in capturing him.
Pride: Devotion Failing: Destruction Motivation: Violence
Weapon Skill Ballistic Skill Strength Toughness Agility Intelligence Perception Willpower Fellowship Infamy (WS) (BS) (S) (T) (Ag) (Int) (Per) (WP) (Fel) (Inf)
10 8
43 3 8 4 7 4 4 3 8 2 9 4 1 5 2 3 1 3 2
   WEAPONS Class: Melee Damage: 1d10+14
SKILLS
Name: Chainaxes Special Rules: Tearing
Pen: 2
Awareness (Per) Intimidate (S)
xooo xxoo
 TALENTS AND SPECIAL RULES


 Tomb Stalker (Master)
WS BS S T Ag Int Per WP Fel Inf
12 14
55 30 60 60 55 30 30 30 05 - -
Wounds: 90 Total TB: 14
                    Movement: 4/8/16/32
Armour: Machine Trait (8 All)
Skills: Intimidate (S)+10, Logic (Int)+20, Stealth (Ag)+20, Tech-Use (Int)+20.
Talents: Ambidextrous, Gunslinger, Independent Targeting, Swift Attack, Two Weapon Weilder, Whirlwind of Death. Traits: Crawler, Dark Sight, Size (6), Regeneration (5), Machine (8), Sturdy, Unnatural Senses (150), Unnatural Strength (+6), Unnatural Toughness (+8).
Weapons: Brutal Blades (2d10+12 R; Pen 12; Razor Sharp), Crushing Legs (1d10+12; Pen 6), Two Gauss Flayers (Basic; 100m; 1d10+8 E; Pen 3; S/2/—; Clip —;
```


How to approach a development of the classifier that learns this patterns of text (notice that each category can have multiple patterns. probably first samples should be devided onto subpatterns and generally cleared for ease of perception)





# Search of the images with similiar drawing style

I have a dataset of the images in `JPG` extracted from various tabletop roleplaying rulebooks. They are different by:
 - size
 - color - some are greyscale, some are rgb
 - flow of text - some are square like, some are have text flow around them
 - artist style - many are drawn by the same artist in the same style, there are serveral styles in corpus

What is the good approach to classify them by artist style? Dataset is huge, what is modern approach in building (distributed, AWS/docker etc hosted) pipeline for learning?




# Convertation of OBJ file into USDz file with autogenerated textures of given color with accent


# Generation of OBJ file using the pixel color information of PNG as normal map

# Generation of USDz model with textures from OBJ file, using given PNG files as textures/normal maps



# Computer vision of the position of arbitrary real world object from predefined set of objects on the table top using a movable camera.

I have a large set of photos of the tabletop under different angles/ligthing/position, containing various objects:
  - coins (10 items)
  - bicycle playing cards (52 items)
  - Magic The Gathering cards (many 1000s)
  - Warhammer 40k miniatures (many 1000s)

 in various groupings in various postions. their postion within the photo is labeled.

 I want to develop an efficient computer vision system that will identify and will track them

   - future optimization: "flow" like algo to track the identity of object that became smaller 
