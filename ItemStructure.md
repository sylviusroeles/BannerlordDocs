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
  
## &lt;CraftedItem&gt; attributes
### crafting_template
**type:**  `string`  
**possible values:** `'TwoHandedPolearm', 'OneHandedAxe', 'Mace', 'TwoHandedAxe', 'OneHandedSword', 'TwoHandedSword', 'Pike', 'Dagger', 'Javelin', 'ThrowingAxe', 'ThrowingKnife'`  
**example:** `TwoHandedPolearm`   
