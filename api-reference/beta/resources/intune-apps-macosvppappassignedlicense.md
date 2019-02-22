---
title: macOsVppAppAssignedLicense リソースの種類
description: MacOS ボリューム購入プログラムのライセンス割り当てです。 このクラスは、作成、削除、更新をサポートしていません。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8c7d8eea98c92ae1a041b8220c171d62fceb385
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158892"
---
# <a name="macosvppappassignedlicense-resource-type"></a>macOsVppAppAssignedLicense リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS ボリューム購入プログラムのライセンス割り当てです。 このクラスは、作成、削除、更新をサポートしていません。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)コレクション|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[macOsVppAppAssignedLicense を取得する](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[macOsVppAppAssignedLicense を作成する](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|新しい[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトを作成します。|
|[macOsVppAppAssignedLicense の削除](../api/intune-apps-macosvppappassignedlicense-delete.md)|なし|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)を削除します。|
|[macOsVppAppAssignedLicense の更新](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userEmailAddress|String|ユーザーの電子メールアドレス。|
|userId|String|ユーザー ID。|
|userName|String|ユーザー名。|
|userPrincipalName|String|ユーザー プリンシパル名。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOsVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```




