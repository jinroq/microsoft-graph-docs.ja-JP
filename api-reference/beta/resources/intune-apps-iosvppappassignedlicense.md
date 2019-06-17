---
title: iosVppAppAssignedLicense リソースの種類
description: iOS Volume Purchase Program ライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6765b7ae313714433c848b57dec0ef1a58d7a38d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987860"
---
# <a name="iosvppappassignedlicense-resource-type"></a>iosVppAppAssignedLicense リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS Volume Purchase Program ライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)コレクション|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[IosVppAppAssignedLicense を取得する](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[IosVppAppAssignedLicense を作成する](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|新しい[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトを作成します。|
|[IosVppAppAssignedLicense の削除](../api/intune-apps-iosvppappassignedlicense-delete.md)|None|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)を削除します。|
|[IosVppAppAssignedLicense の更新](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
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
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





