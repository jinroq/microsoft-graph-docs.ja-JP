---
title: iosVppAppAssignedUserLicense リソースの種類
description: iOS ボリューム購入プログラムのユーザーライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e259c1b31d1b61fe3c9a3508d52160ddbe0c4fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005479"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>iosVppAppAssignedUserLicense リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS ボリューム購入プログラムのユーザーライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。


[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)コレクション|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[IosVppAppAssignedUserLicense を取得する](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[IosVppAppAssignedUserLicense を作成する](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|新しい[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを作成します。|
|[IosVppAppAssignedUserLicense の削除](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|None|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)を削除します。|
|[IosVppAppAssignedUserLicense の更新](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userEmailAddress|String|ユーザーの電子メールアドレス。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userId|String|ユーザー ID。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userName|String|ユーザー名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userPrincipalName|String|ユーザー プリンシパル名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedUserLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





