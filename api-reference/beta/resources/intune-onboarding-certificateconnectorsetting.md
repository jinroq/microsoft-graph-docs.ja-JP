---
title: certificateConnectorSetting リソースの種類
description: 証明書コネクタの設定。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a980e6bf8dd97141fc3fc5a078beedbd0348a79
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940464"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

証明書コネクタの設定。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|status|Int32|証明書コネクタの状態|
|certExpiryTime|DateTimeOffset|証明書の有効期限|
|enrollmentError|String|証明書コネクタの登録エラー|
|Lastコネクタ接続時間|DateTimeOffset|証明書コネクタが前回接続された日時|
|コネクタのバージョン|String|証明書コネクタのバージョン|
|lastUploadVersion|Int64|最後にアップロードされた証明書コネクタのバージョン|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```




