---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1cd7cb3f197e381da0b334ed849d881d071979e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990002"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>deviceManagementUserRightsLocalUserOrGroup リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|このローカルユーザーまたはグループの名前。|
|description|String|このローカルユーザーまたはグループの管理者の説明。|
|securityIdentifier|String|このローカルユーザーまたはグループのセキュリティ識別子 (たとえば * S-1-5-32-544)。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





