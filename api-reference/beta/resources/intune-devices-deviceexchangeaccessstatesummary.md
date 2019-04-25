---
title: deviceExchangeAccessStateSummary リソースの種類
description: デバイスの Exchange アクセス状態の要約
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39f944b7559abf72d144f5c1608ec4efec014530
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549119"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>deviceExchangeAccessStateSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの Exchange アクセス状態の要約

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedDeviceCount|Int32|Exchange アクセス状態が Allowed のデバイスの総数です。|
|blockedDeviceCount|Int32|Exchange アクセス状態が Blocked のデバイスの総数です。|
|quarantinedDeviceCount|Int32|Exchange アクセス状態が Quarantined のデバイスの総数です。|
|unknownDeviceCount|Int32|Exchange アクセス状態が Unknown のデバイスの総数です。|
|unavailableDeviceCount|Int32|Exchange アクセス状態を検出できなかったデバイスの総数です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```





