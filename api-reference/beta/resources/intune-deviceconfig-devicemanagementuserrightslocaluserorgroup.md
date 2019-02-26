---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68c514635540bcf12db27e8a9ca816573293d3ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174861"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>deviceManagementUserRightsLocalUserOrGroup リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザー権限の設定に使用されるローカルユーザーまたはグループの情報を表します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|name|String|このローカルユーザーまたはグループの名前。|
|説明|String|このローカルユーザーまたはグループの管理者の説明。|
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




