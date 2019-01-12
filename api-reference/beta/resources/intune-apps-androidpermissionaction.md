---
title: androidPermissionAction リソースの種類
description: Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ad7b438951b947cc515f1472dd1eae8caf472f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977123"
---
# <a name="androidpermissionaction-resource-type"></a>androidPermissionAction リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|アクセス許可|String|Android のアクセス許可の文字列、公式の Android のドキュメントで定義されています。  'Android.permission.READ_CONTACTS' の使用例です。|
|action|[androidPermissionActionType](../resources/intune-apps-androidpermissionactiontype.md)|Android 権限操作の種類です。 可能な値は、`prompt`、`autoGrant`、`autoDeny` です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```





