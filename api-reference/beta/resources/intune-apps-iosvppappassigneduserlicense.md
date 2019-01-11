---
title: iosVppAppAssignedUserLicense リソースの種類
description: iOS ボリューム購入プログラムのユーザー ライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
localization_priority: Normal
ms.openlocfilehash: 3217fc338b2f0bb072de19cf0807a718a4998efa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806896"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>iosVppAppAssignedUserLicense リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS ボリューム購入プログラムのユーザー ライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。

[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)コレクション|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IosVppAppAssignedUserLicense を取得します。](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティと関係を参照してください。|
|[IosVppAppAssignedUserLicense を作成します。](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|新しい[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを作成します。|
|[IosVppAppAssignedUserLicense を削除します。](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|なし|の[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)を削除します。|
|[IosVppAppAssignedUserLicense を更新します。](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|[IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userEmailAddress|String|ユーザーの電子メール アドレスです。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userId|String|ユーザー id。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userName|String|ユーザー名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|
|userPrincipalName|String|ユーザー プリンシパル名。 [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承されました。|

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





