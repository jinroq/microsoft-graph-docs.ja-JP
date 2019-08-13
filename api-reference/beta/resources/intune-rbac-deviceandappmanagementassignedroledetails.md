---
title: deviceAndAppManagementAssignedRoleDetails リソースの種類
description: ユーザーに割り当てられた役割定義と役割の割り当てのセット。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 89f864da336045622af0e59a94fb14d0132872db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308191"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>deviceAndAppManagementAssignedRoleDetails リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーに割り当てられた役割定義と役割の割り当てのセット。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|roleDefinitionIds|文字列コレクション|ユーザーに割り当てられている表面化ロール定義のロール定義 Id。|
|roleAssignmentIds|文字列コレクション|ユーザーに割り当てられている表面化の役割の割り当ての役割割り当て Id。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```



