---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb9ededd9d1a2bb93f970f9f0da0c41a248e840
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425800"
---
# <a name="auditactor-resource-type"></a>auditActor リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

監査アクターのプロパティが含まれるクラス。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|type|文字列型 (String)|アクターの種類。|
|userPermissions|String コレクション|監査の実行時におけるユーザーのアクセス許可の一覧。|
|applicationId|文字列型 (String)|AAD アプリケーション ID。|
|applicationDisplayName|文字列型 (String)|アプリケーションの名前。|
|userPrincipalName|文字列型 (String)|ユーザー プリンシパル名 (UPN)。|
|servicePrincipalName|文字列型 (String)|サービス プリンシパル名 (SPN)。|
|ipAddress|文字列型 (String)|IPAddress。|
|userId|文字列型 (String)|ユーザー ID。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```




