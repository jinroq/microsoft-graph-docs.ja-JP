---
title: certificateConnectorSetting リソースの種類
description: 証明書コネクタの設定。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe154ed3150ae434f8068bc04a56dd6e5b48744
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573061"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

証明書コネクタの設定。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|status|Int32|証明書コネクタの状態|
|certExpiryTime|DateTimeOffset|証明書の有効期限|
|enrollmentError|String|証明書コネクタの登録エラー|
|lastコネクタ接続時間|DateTimeOffset|証明書コネクタが前回接続された日時|
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





