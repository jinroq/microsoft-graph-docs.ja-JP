---
title: androidPermissionAction リソースの種類
description: Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62355c3427083df09963e316f3b6b3c104a8662f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425632"
---
# <a name="androidpermissionaction-resource-type"></a>androidPermissionAction リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
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




