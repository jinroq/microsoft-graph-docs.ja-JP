---
title: locationmanagementcondition リソースの種類
description: 監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2560309e937bb1b2e6ffd436cec5988fd38dbf2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568836"
---
# <a name="locationmanagementcondition-resource-type"></a>locationmanagementcondition リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

監視対象の場所管理条件 (対象となる領域) を定義するための情報が含まれています。


[managementcondition](../resources/intune-fencing-managementcondition.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[locationmanagementconditions を一覧表示する](../api/intune-fencing-locationmanagementcondition-list.md)|[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション|[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[locationmanagementcondition の取得](../api/intune-fencing-locationmanagementcondition-get.md)|[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)|[locationmanagementcondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|管理条件の一意識別子。 作成時に割り当てられたシステム生成値。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|uniqueName|String|管理条件の一意の名前。 管理条件式で使用されます。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|displayName|String|管理条件の管理者定義の名前。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|説明|String|管理条件の管理者定義の説明。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側を生成しました。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|modifiedDateTime|DateTimeOffset|管理条件が最後に変更された時刻。 サービス側を更新しました。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|eTag|String|管理条件の ETag。 サービス側を更新しました。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件の適用可能なプラットフォーム。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementconditionstatements|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理条件ステートメント。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
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





