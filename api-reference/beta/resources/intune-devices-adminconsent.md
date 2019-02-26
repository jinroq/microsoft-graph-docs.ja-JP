---
title: adminconsent リソースの種類
description: 管理者の同意情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f46e379a47bd7b08be1427115c785452543dfbf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157940"
---
# <a name="adminconsent-resource-type"></a>adminconsent リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理者の同意情報。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|/sharepoint データの編集|[adminconの状態](../resources/intune-devices-adminconsentstate.md)|ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。 可能な値は、`notConfigured`、`granted`、`notGranted` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




