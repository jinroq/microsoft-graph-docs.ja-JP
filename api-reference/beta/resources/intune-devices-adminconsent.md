---
title: adminConsent リソースの種類
description: 管理者の同意情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d78333cd683501a8bf4fea0aa3a2e55944d9b5a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319309"
---
# <a name="adminconsent-resource-type"></a>adminConsent リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理者の同意情報。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|/Sharepoint データの編集|[Adminconの状態](../resources/intune-devices-adminconsentstate.md)|ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。 可能な値は、`notConfigured`、`granted`、`notGranted` です。|
|shareUserExperienceAnalyticsData|[Adminconの状態](../resources/intune-devices-adminconsentstate.md)|ユーザー環境分析データの共有に関する管理者の同意を取得または設定します。 可能な値は、`notConfigured`、`granted`、`notGranted` です。|

## <a name="relationships"></a>リレーションシップ
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
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```



