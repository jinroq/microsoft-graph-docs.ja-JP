---
title: networkManagementCondition リソースの種類
description: ネットワーク管理条件を定義するための情報が含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03a27bc32c4a1a0e5b1f03601f8c511d914d073f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941220"
---
# <a name="networkmanagementcondition-resource-type"></a>networkManagementCondition リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ネットワーク管理条件を定義するための情報が含まれています。


[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[NetworkManagementConditions を一覧表示する](../api/intune-fencing-networkmanagementcondition-list.md)|[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)コレクション|[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[NetworkManagementCondition の取得](../api/intune-fencing-networkmanagementcondition-get.md)|[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)|[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|文字列|管理条件の一意識別子。 作成時に割り当てられたシステム生成値。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|uniqueName|String|管理条件の一意の名前。 管理条件式で使用されます。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|displayName|String|管理条件の管理者定義の名前。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|description|String|管理条件の管理者定義の説明。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側を生成しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|modifiedDateTime|DateTimeOffset|管理条件が最後に変更された時刻。 サービス側を更新しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|eTag|String|管理条件の ETag。 サービス側を更新しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件の適用可能なプラットフォーム。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditionStatements|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理条件ステートメント。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




