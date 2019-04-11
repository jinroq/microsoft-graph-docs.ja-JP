---
title: iosVppAppAssignedLicense リソースの種類
description: iOS Volume Purchase Program ライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 162eaeebd8c678bf29b3b40729114f67d1325c86
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790376"
---
# <a name="iosvppappassignedlicense-resource-type"></a>iosVppAppAssignedLicense リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS Volume Purchase Program ライセンスの割り当て。 このクラスは、作成、削除、更新をサポートしていません。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)コレクション|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[iosVppAppAssignedLicense を取得する](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosVppAppAssignedLicense を作成する](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|新しい[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトを作成します。|
|[iosVppAppAssignedLicense の削除](../api/intune-apps-iosvppappassignedlicense-delete.md)|なし|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)を削除します。|
|[iosVppAppAssignedLicense の更新](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|userEmailAddress|文字列|ユーザーの電子メールアドレス。|
|userId|String|ユーザー ID。|
|userName|文字列型 (String)|ユーザー名。|
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





