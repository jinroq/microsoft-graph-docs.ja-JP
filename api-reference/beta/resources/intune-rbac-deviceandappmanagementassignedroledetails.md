---
title: deviceAndAppManagementAssignedRoleDetails リソースの種類
description: ユーザーに割り当てられた役割定義と役割の割り当てのセット。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93f99cdc91d046b9ebf292bbd34f1bba39b494ac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771405"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>deviceAndAppManagementAssignedRoleDetails リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーに割り当てられた役割定義と役割の割り当てのセット。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|roledefinitionids|String コレクション|ユーザーに割り当てられている表面化ロール定義のロール定義 id。|
|roleAssignmentIds|String コレクション|ユーザーに割り当てられている表面化の役割の割り当ての役割割り当て id。|

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





