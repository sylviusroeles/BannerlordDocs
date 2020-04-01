# The Item Structure of Bannerlord
This file will explain the stucture of the items with possible key value pairs.

## Example Entry
Source: Modules/SandBoxCore/ModuleData/spitems.xml
```xml
  <Item id="headscarf_d"
        name="{=wW3iouiU}Hijab"
        mesh="headscarf_d"
        culture="Culture.aserai"
        weight="0.5"
        appearance="0.5"
        Type="HeadArmor">
    <ItemComponent>
      <Armor head_armor="3"
             has_gender_variations="false"
             hair_cover_type="all"
             modifier_group="cloth_unarmoured"
             material_type="Cloth"
             beard_cover_type="type3" />
    </ItemComponent>
    <Flags Civilian="true"
           UseTeamColor="true" />
  </Item>
```

## &lt;Item&gt; attributes
### name
**type:**  `string`  
**example:**  `{=wW3iouiU}Hijab`
*Note: The prefix in the `{=}` format is the translation id found in strings.txt*
*TODO: Find out if this is auto generated.*  
  
### mesh
**type:**  `string`  
**example:** `headscarf_d`  
*The string is a reference to the mesh id  
TODO: Figure out where this is stored*  
  
### culture
**type:**  `string`  
**possible values:** `'Culture.aserai', 'Culture.sturgia', 'Culture.battania', 'Culture.looters', 'Culture.khuzait', 'Culture.vlandia', 'Culture.empire', 'Culture.neutral_culture'`  
**example:** `Culture.aserai`  
  
### weight
**type:**  `double`  
**example:** `0.5`  
  
### appearance
**type:**  `double`  
**example:** `0.5` 
*TODO: Figure out what this is for*  
### Type
**type:**  `ArmourType`  
**possible values:** `'HeadArmor', 'headArmor', 'Cape', 'BodyArmor', 'HandArmor', 'LegArmor', 'OneHandedWeapon', 'Bow', 'Polearm', 'Crossbow', 'Thrown', 'Arrows', 'Bolts', 'Shield', 'Horse', 'HorseHarness', 'Goods', 'Banner', 'Animal'`
**example:** `HeadArmor`  
  
### multiplayer_item
**type:**  `boolean`  
**possible values:** `'true', 'false'`  
**example:** `false`  
  
### subtype
**type:**  `string`  
**possible values:** `'head_armor', 'body_armor', 'bow', 'two_handed_wpn', 'arrows', 'horse'`  
**example:** `head_armor` 
*TODO: Figure out what this is for*  
  
### difficulty
**type:**  `int`  
**possible values:** `0-100`  
**example:** `80`  
  
### difficulty
**type:**  `int`  
**possible values:** `0-100`  
**example:** `80`  
  
### lod_atlas_index
**type:**  `int`  
**example:** `2`  
*TODO: Figure out what this is for*  
  
### is_merchandise
**type:**  `boolean`  
**example:** `false`  
  
### body_name
**type:**  `id`  
**example:** `bo_mace_a`  
*Possibly the collision mesh of an weapon? TODO: figure out*
  
### recalculate_body
**type:**  `boolean`  
**possible values:** `'true', 'false'`  
**example:** `false` 
*TODO: Figure out what this is for*  
  
### prefab
**type:**  `id`  
**example:** `torch_a_wm_only_flame` 
*TODO: Figure out what this is for. Possibly particle effects?* 
  
### value
**type:**  `int`  
**example:** `150` 
*The average market value* 
  
### item_holsters
**type:**  `string`  
**possible values:** `'abdomen_left', 'bow_back_2:bow_hip:bow_hip_2:bow_back', 'bow_back:bow_back_2:bow_hip:bow_hip_2', 'sword_left_hip', 'polearm_back:polearm_back_2', 'bow_hip:bow_hip_2:bow_back:bow_back_2', 'crossbow_back:bow_hip:mace_right_hip:bow_hip_2', 'throwing_stone:throwing_stone_2', '', 'quiver_back_top:quiver_back_top_2', 'quiver_back_middle:quiver_bolts_2:quiver_bolts', 'quiver_back_lower:quiver_back_lower_2', 'quiver_back_middle:quiver_bolts:quiver_bolts_2', 'quiver_bolts:quiver_bolts_2:quiver_back_middle:quiver_back_top', 'quiver_back_middle:quiver_back_top:quiver_bolts:quiver_bolts_2', 'shield_round:shield_4', 'shield_oval:shield_4:shield_3:shield_2', 'shield:shield_2:shield_3:shield_4', 'shield_kite:shield_2:shield_3:shield_4'`  
**example:** `abdomen_left` 
*The carry position of a weapon*  
  
### AmmoOffset
**type:**  `vector3d`  
**example:** `0.0, 0.02131, 0.24675` 
*The position the projectile is shot from?* 
  
### holster_position_shift
**type:**  `vector3d`   
**example:** `0.0,0.0,-0.0` 
*TODO: Figure out what this is for*  
  
### holster_body_name
**type:**  `string`   
**example:** `bo_axe_short` 
*TODO: Figure out what this is for*  
  
### holster_mesh
**type:**  `string`   
**example:** `stone_holster` 
*The mesh id of the quivers etc*   
  
### holster_mesh_with_weapon
**type:**  `string`   
**example:** `stone_holster` 
*The mesh id of the quivers etc with the weapon*  
  
### flying_mesh
**type:**  `string`   
**example:** `  ` 
*The mesh id of the projectile* 
  
### shield_body_name
**type:**  `string`   
**example:** `bo_sturgia_shield_a` 
*The hitbox id of a shield*  
  
### using_tableau
**type:**  `boolean`   
**example:** `true` 
*Whether the item has a tableau*  
  
### has_lower_holster_priority
**type:**  `boolean`   
**example:** `true` 
*TODO: Figure out what this exactly does.*  
  
### item_category
**type:**  `id`   
**possible values:** `'horse', 'sumpter_horse', 'war_horse', 'wool', 'silver', 'jewelry', 'salt', 'cotton', 'flax', 'clay', 'pottery', 'linen', 'leather', 'velvet', 'cheese', 'butter', 'fish', 'grape', 'date_fruit', 'olives', 'beer', 'wine', 'oil', 'fur', 'animal', 'sheep', 'cow', 'hog'`  
**example:** `true` 
*Marketable item category*  

### IsFood
**type:**  `boolean`   
**example:** `true` 
*If the item is consumable*  

## &lt;ItemComponent&gt;
The ItemComponent Entry takes no attributes, instead it has a xml child
### Armor
**Attributes**  
```
'head_armor', 'has_gender_variations', 'hair_cover_type', 'modifier_group', 'material_type', 'beard_cover_type',   
'body_armor', 'leg_armor', 'arm_armor', 'covers_body', 'body_mesh_type', 'covers_legs', 'covers_hands', 'mane_cover_type',
'family_type', 'maneuver_bonus', 'speed_bonus', 'charge_bonus', 'reins_mesh', 'covers_head'
```
#### head_armor
**type:**  `int`   
**example:** `64`  
*Amount of head armour*  
  
#### has_gender_variations
**type:**  `boolean`   
**example:** `true`  
*If there is a gender variation of the model*  
  
#### hair_cover_type
**type:**  `string` 
**accepted values:** `'all', 'type1', 'type2', 'type3'`  
**example:** `all`  
*TODO: figure out what type1, type2, type3 stands for*  
  
#### modifier_group
**type:**  `string`   
**accepted values:** `'cloth_unarmoured', 'leather', 'plate', 'chain', 'cloth'`  
**example:** `leather`  
*Modifier for damage soak?*  
  
#### material_type
**type:**  `string`   
**accepted values:** `'Cloth', 'Leather', 'Plate', 'Chainmail'`  
**example:** `Cloth`  
*The material of the armour*  
  
#### beard_cover_type
**type:**  `string`   
**accepted values:** `'type3', 'type2', 'none', 'all', 'type1'`  
**example:** `none`  
*Variable to set the covering of beard*  
  
#### body_armor
**type:**  `int`   
**example:** `23`  
*Amount of body armour*  
  
#### leg_armor
**type:**  `int`   
**example:** `23`  
*Amount of leg armour*  
  
#### arm_armor
**type:**  `int`   
**example:** `23`  
*Amount of hand (gauntlet) armour*  
  
#### covers_body
**type:**  `boolean`  
**accepted values:** `'true', 'false'`  
**example:** `true`  
*If the armour covers the body*  
  
#### body_mesh_type
**type:**  `string`  
**accepted values:** `'shoulders'`  
**example:** `shoulders`  
*TODO: figure out what this does*  
  
#### covers_legs
**type:**  `boolean`  
**accepted values:** `'true', 'false'`  
**example:** `true`  
*If the armour covers the legs*  
  
#### covers_hands
**type:**  `boolean`  
**accepted values:** `'true', 'false'`  
**example:** `true`   
*If the armour covers the hands*   
  
#### mane_cover_type
**type:**  `string`  
**accepted values:** `'none', 'all'`  
**example:** `none`  
*TODO: What exactly does this cover?*  
  
#### family_type
**type:**  `int`  
**accepted values:** `'1', '2'`  
**example:** `1`  
*TODO: What does this value do?*  
  
#### maneuver_bonus
**type:**  `int`   
**example:** `12`  
*Gives a bonus to the maneuverablity TODO: for the player or horse?*  
  
#### speed_bonus
**type:**  `int`   
**example:** `11`  
*Gives a bonus to the speed TODO: for the player or horse?*  
  
#### charge_bonus
**type:**  `int`   
**example:** `11`   
*Gives a charging bonus TODO: for the player or horse?*  
  
#### reins_mesh
**type:**  `string`   
**example:** `horse_harness_vlandia_b_rein`  
*Mesh ID of the reins*  
  
#### covers_head
**type:**  `boolean`  
**accepted values:** `'true', 'false'`  
**example:** `true`  
*If the armour covers the head*  
  
### Weapon
**Attributes**
```
'weapon_class', 'weapon_balance', 'thrust_speed', 'speed_rating', 'missile_speed', 'weapon_length', 'swing_damage', 'swing_damage_type',
'item_usage', 'physics_material', 'ammo_class', 'ammo_limit', 'accuracy', 'thrust_damage', 'thrust_damage_type', 'center_of_mass',
'stack_amount', 'rotation', 'passby_sound_code', 'rotation_speed', 'flying_sound_code', 'sticking_rotation', 'sticking_position',
'trail_particle_name', 'position', 'body_armor', 'hit_points'
```
  
#### weapon_class
**type:**  `string`  
**accepted values:** `'OneHandedAxe', 'Bow', 'OneHandedSword', 'TwoHandedPolearm', 'Crossbow', 'Stone', 'Arrow', 'Boulder', 'Bolt', 'LargeShield', 'Banner'`  
**example:** `OneHandedAxe`  
*Type of weapon*  
  
#### weapon_balance
**type:**  `int`  
**example:** `100`  
*Balance of the weapon*  
  
#### thrust_speed
**type:**  `int`  
**example:** `12`  
*Thrust speed of the weapon*  
  
#### speed_rating
**type:**  `int`  
**example:** `60`  
*Speed rating of the weapon*  
  
#### missile_speed
**type:**  `int`  
**example:** `60`  
*Speed of the projectile being fired from the weapon*  
  
#### weapon_length
**type:**  `int`  
**example:** `60`  
*Length of the weapon*  
  
#### swing_damage
**type:**  `int`  
**example:** `60`  
*Swing damage of the weapon*  
  
#### swing_damage_type
**type:**  `string`  
**accepted values:** `'Pierce', 'Blunt', 'Cut'`   
**example:** `Pierce`  
*Swing damage type of the weapon*  
  
#### item_usage
**type:**  `string`  
**accepted values:** `'torch', 'bow', 'long_bow', 'onehanded_block_shield_swing', 'polearm_block_thrust', 'crossbow_fast', 'crossbow', 'stone', '', 'heavy_stone', 'arrow_top', 'arrow_right', 'hand_shield', 'shield', 'banner'`   
**example:** `heavy_stone`  
*How the item is used*  
  
#### physics_material
**type:**  `string`  
**accepted values:** `'metal_weapon', 'wood_weapon', 'missile', 'ballista_missile', 'burning_ballista', 'boulder_stone', 'burning_jar', 'wood_shield', 'metal_shield'`   
**example:** `metal_shield`  
*What the weapon consists of*  
  
#### ammo_class
**type:**  `string`  
**accepted values:** `'Arrow', 'Bolt', 'Stone', 'Boulder'`   
**example:** `Arrow`  
*Ammo type*  
  
#### ammo_limit
**type:**  `int`   
**example:** `1`  
*Amount of ammo stored in the weapon. TODO: if set to 2 will it shoot 2 arrows? Or with crossbows will it become a repeating crossbow?*   
#### accuracy
**type:**  `int`   
**example:** `21`  
*Accuracy of a ranged weapon*   
  
#### thrust_damage
**type:**  `int`   
**example:** `21`  
*Thrust damage of a weapon*   
  
#### thrust_damage_type
**type:**  `string`  
**accepted values:** `'Pierce', 'Blunt', 'Cut'`   
**example:** `Pierce`  
*Thrust damage type of the weapon*  
  
#### center_of_mass
**type:**  `vector3d`  
**example:** `0.15,0,0`  
*Center of mass of the weapon. TODO: what is this used for?*  
  
#### stack_amount
**type:**  `int`  
**example:** `23`  
*Amount of projectiles the weapon (arrows, bolts, stones) has*  
  
#### rotation
**type:**  `vector3d`  
**example:** `100,30,20`  
*TODO: figure out what this does*  
  
#### passby_sound_code
**type:**  `string`  
**example:** `event:/mission/combat/missile/passby`  
*What sound a projectile should make if passing by an agent*  
  
#### rotation_speed
**type:**  `double`  
**example:** `0.5`  
*TODO: figure out what this does*  
  
#### flying_sound_code
**type:**  `string`  
**example:** `event:/mission/combat/missile/foley/passby`  
*What sound a projectile should make when flying in midair*  
  
#### sticking_rotation
**type:**  `vector3d`  
**example:** `90,0,0`  
*TODO: figure out what this does*  
  
#### sticking_position
**type:**  `vector3d`  
**example:** `90,0,0`  
*TODO: figure out what this does*  
  
#### trail_particle_name
**type:**  `string`  
**example:** `psys_game_missile_flame`  
*Particles that are emitted on a flying projectile*  
  
#### position
**type:**  `vector3d`  
**example:** `-0.04, -0.05, 0.01`  
*TODO: figure out what this does*  
  
#### body_armor
**type:**  `int`  
**example:** `82`  
*The amount of body armour a weapon gives. TODO: figure out if this is possible with head, leg, and hand armour as well.*  
  
#### hit_points
**type:**  `int`  
**example:** `820`  
*Hit points of a shield*  
  
  
## &lt;CraftedItem&gt; attributes
### crafting_template
**type:**  `string`  
**possible values:** `'TwoHandedPolearm', 'OneHandedAxe', 'Mace', 'TwoHandedAxe', 'OneHandedSword', 'TwoHandedSword', 'Pike', 'Dagger', 'Javelin', 'ThrowingAxe', 'ThrowingKnife'`  
**example:** `TwoHandedPolearm`   
