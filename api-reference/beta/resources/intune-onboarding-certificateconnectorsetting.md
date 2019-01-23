---
title: certificateConnectorSetting リソースの種類
description: コネクタの設定を証明書です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398654"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コネクタの設定を証明書です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
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




