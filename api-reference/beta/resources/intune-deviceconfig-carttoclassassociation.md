---
title: cartToClassAssociation リソースの種類
description: デバイスカートと教室を関連付けるための CartToClassAssociation。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cdde67e8ffb0d30c631b4bbc39a70ed9b8387da
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990163"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスカートと教室を関連付けるための CartToClassAssociation。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)コレクション|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[CartToClassAssociation を取得する](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[CartToClassAssociation を作成する](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。|
|[CartToClassAssociation の削除](../api/intune-deviceconfig-carttoclassassociation-delete.md)|None|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を削除します。|
|[CartToClassAssociation の更新](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。|
|version|Int32|CartToClassAssociation のバージョン。|
|displayName|String|管理者が指定した、デバイス構成の名前。|
|description|String|CartToClassAssociation の管理者提供の説明。|
|deviceCartIds|文字列コレクション|クラスに関連付けられるデバイスカートの識別子。|
|classroomIds|文字列コレクション|デバイスカートに関連付ける教室の識別子。|

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





