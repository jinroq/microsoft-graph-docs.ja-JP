---
title: cartToClassAssociation リソースの種類
description: 教室カートのデバイスに関連付けるための CartToClassAssociation です。
author: tfitzmac
ms.openlocfilehash: f712759d82b5edf7d364658211f1f2142fb6eb87
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328281"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

教室カートのデバイスに関連付けるための CartToClassAssociation です。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を一覧表示します。|
|[CartToClassAssociation を取得します。](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を参照してください。|
|[CartToClassAssociation を作成します。](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。|
|[CartToClassAssociation を削除します。](../api/intune-deviceconfig-carttoclassassociation-delete.md)|なし|の[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を削除します。|
|[CartToClassAssociation を更新します。](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。|
|version|Int32|CartToClassAssociation のバージョンです。|
|displayName|String|デバイス構成について管理者が指定した名前。|
|説明|String|管理者には、CartToClassAssociation の説明が用意されています。|
|deviceCartIds|String コレクション|クラスに関連するデバイスのカートの識別子です。|
|classroomIds|String コレクション|デバイスのカートに関連する教室の識別子です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```





