---
title: deviceEnrollmentPlatformRestriction リソースの種類
description: プラットフォーム固有の登録の制限
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0288883ec1deaaecc142aec42f413a4f60a76b5b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993159"
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





