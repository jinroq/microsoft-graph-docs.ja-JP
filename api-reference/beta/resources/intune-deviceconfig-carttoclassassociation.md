---
title: cartToClassAssociation リソースの種類
description: 教室カートのデバイスに関連付けるための CartToClassAssociation です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b832e4597b15f062289a086d068ea3da71d9f66a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395693"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

教室カートのデバイスに関連付けるための CartToClassAssociation です。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を一覧表示します。|
|[CartToClassAssociation を取得します。](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティと関係を参照してください。|
|[CartToClassAssociation を作成します。](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。|
|[CartToClassAssociation を削除します。](../api/intune-deviceconfig-carttoclassassociation-delete.md)|なし|の[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を削除します。|
|[CartToClassAssociation を更新します。](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
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




