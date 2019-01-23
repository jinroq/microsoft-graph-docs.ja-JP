---
title: macOsVppAppAssignedLicense リソースの種類
description: MacOS ボリューム購入プログラムのライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c3a029d0f0aca7ab295f34d108b8bf61bdc17dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430329"
---
# <a name="macosvppappassignedlicense-resource-type"></a>macOsVppAppAssignedLicense リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS ボリューム購入プログラムのライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)コレクション|[MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MacOsVppAppAssignedLicense を取得します。](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|[MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティと関係を参照してください。|
|[MacOsVppAppAssignedLicense を作成します。](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|新しい[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトを作成します。|
|[MacOsVppAppAssignedLicense を削除します。](../api/intune-apps-macosvppappassignedlicense-delete.md)|なし|の[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)を削除します。|
|[MacOsVppAppAssignedLicense を更新します。](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|[MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)オブジェクトのプロパティを更新します。|

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




