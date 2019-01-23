---
title: iosVppAppAssignedLicense リソースの種類
description: iOS ボリューム購入プログラムのライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ff1d467dd0bd5ef34836d77f2f7dd034d877f1f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395658"
---
# <a name="iosvppappassignedlicense-resource-type"></a>iosVppAppAssignedLicense リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS ボリューム購入プログラムのライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)コレクション|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IosVppAppAssignedLicense を取得します。](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティと関係を参照してください。|
|[IosVppAppAssignedLicense を作成します。](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|新しい[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトを作成します。|
|[IosVppAppAssignedLicense を削除します。](../api/intune-apps-iosvppappassignedlicense-delete.md)|なし|の[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)を削除します。|
|[IosVppAppAssignedLicense を更新します。](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userEmailAddress|String|ユーザーの電子メール アドレスです。|
|userId|String|ユーザー id。|
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




