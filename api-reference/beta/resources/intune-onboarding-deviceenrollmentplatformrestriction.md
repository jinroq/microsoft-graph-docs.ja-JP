---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1485c429594967fd3c76fc27cb89e85c84cda92
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374359"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a>deviceEnrollmentPlatformRestriction リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

プラットフォーム固有の登録の制限

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|platformBlocked|Boolean|登録で対象プラットフォームをブロックします|
|personalDeviceEnrollmentBlocked|ブール型 (Boolean)|個人所有のデバイスの登録をブロックします|
|osMinimumVersion|String|サポートされる最小 OS バージョン|
|osMaximumVersion|文字列型 (String)|サポートされる最大 OS バージョン|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



