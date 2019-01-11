---
title: certificateConnectorSetting リソースの種類
description: コネクタの設定を証明書です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56f12600b6aa78982dc51732d685dcd7c962d0b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888600"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

コネクタの設定を証明書です。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|status|Int32|証明書のコネクタの状態|
|certExpiryTime|DateTimeOffset|証明書の有効期限が切れる時間|
|enrollmentError|String|コネクタの登録の証明書のエラー|
|lastConnectorConnectionTime|DateTimeOffset|コネクタが接続されている証明書の最後に|
|connectorVersion|String|コネクタの証明書のバージョン|
|lastUploadVersion|Int64|最後の証明書をアップロードしたコネクタのバージョン|

## <a name="relationships"></a>リレーションシップ
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





