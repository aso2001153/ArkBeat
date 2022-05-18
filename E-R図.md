```uml
@startuml
!define Color_T Blue
!define Color_R Red
!define Color_C DeepSkyBlue

skinparam class {
  BackgroundColor CadetBlue
  BorderColor white
  ArrowColor black
  IconFontColor black
}

package "クイズメーカー" as target_system{

  entity "ユーザーテーブル" as user <<T,Color_T>> {
    + user_id [PK]
    --
    user_name
    user_mail
    user_psw
    user_tel
    user_post
    user_address
    user_sale
    user_penalty
    user_created	
    user_updated	
    user_deleted
  }

