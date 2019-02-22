---
title: cartToClassAssociation リソースの種類
description: デバイスカートと教室を関連付けるための CartToClassAssociation。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228a3bfc873fdaf1fbd77e51a79ca184c2416d7c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156596"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスカートと教室を関連付けるための CartToClassAssociation。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[cartToClassAssociation を取得する](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[cartToClassAssociation を作成する](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。|
|[cartToClassAssociation の削除](../api/intune-deviceconfig-carttoclassassociation-delete.md)|なし|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を削除します。|
|[cartToClassAssociation の更新](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。|
|version|Int32|CartToClassAssociation のバージョン。|
|displayName|String|デバイス構成について管理者が指定した名前。|
|説明|String|CartToClassAssociation の管理者提供の説明。|
|devicecartids|String collection|クラスに関連付けられるデバイスカートの識別子。|
|classroomIds|String collection|デバイスカートに関連付ける教室の識別子。|

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




