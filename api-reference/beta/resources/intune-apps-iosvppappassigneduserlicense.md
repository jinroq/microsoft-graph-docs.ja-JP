---
title: iosVppAppAssignedUserLicense リソースの種類
description: iOS ボリューム購入プログラムのユーザーライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed98c188cc094530d6a4e3504fa5efb4d84bd599
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158003"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>iosVppAppAssignedUserLicense リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS ボリューム購入プログラムのユーザーライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。


[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)コレクション|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[iosVppAppAssignedUserLicense を取得する](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosVppAppAssignedUserLicense を作成する](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|新しい[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトを作成します。|
|[iosVppAppAssignedUserLicense の削除](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|なし|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)を削除します。|
|[iosVppAppAssignedUserLicense の更新](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userEmailAddress|String|ユーザーの電子メールアドレス。 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userId|String|ユーザー ID。 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userName|String|ユーザー名。 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|
|userPrincipalName|String|ユーザー プリンシパル名。 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)から継承します。|

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




