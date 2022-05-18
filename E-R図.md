```uml
@startuml
!define Color_M Blue
!define Color_R Red
!define Color_C DeepSkyBlue

skinparam class {
  BackgroundColor CadetBlue
  BorderColor white
  ArrowColor black
  IconFontColor black
}

package "クイズメーカー" as target_system{

  entity "メンバーテーブル" as user <<M,Color_M>> {
    + member_id [PK]
    --
    member_id
    member_name
    member_pass
    member_mail
  }

entity "四択問題テーブル" as user <<M,Color_M>> {
    + for-choice_id [PK]
    --
    for-choice_sentence
    choice1
    choice2
    choice3
    choice4
    explanation
  }

