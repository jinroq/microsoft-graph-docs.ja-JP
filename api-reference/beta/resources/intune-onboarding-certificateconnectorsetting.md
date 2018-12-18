---
title: certificateConnectorSetting リソースの種類
description: コネクタの設定を証明書です。
author: tfitzmac
ms.openlocfilehash: 8c993634eb4f41e16643ae3f40be74ecc3eb392f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326307"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

コネクタの設定を証明書です。
## <a name="properties"></a>Properties
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





