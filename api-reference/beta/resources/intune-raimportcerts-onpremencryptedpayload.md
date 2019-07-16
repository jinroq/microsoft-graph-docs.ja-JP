---
title: onPremEncryptedPayload リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30f0abc0c25fefd957cd9b40a0a4ae5e0f6ad953
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741466"
---
# <a name="onpremencryptedpayload-resource-type"></a>onPremEncryptedPayload リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト onPremEncryptedPayloads](../api/intune-raimportcerts-onpremencryptedpayload-list.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)コレクション|[OnPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[OnPremEncryptedPayload を取得する](../api/intune-raimportcerts-onpremencryptedpayload-get.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|[OnPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[OnPremEncryptedPayload を作成する](../api/intune-raimportcerts-onpremencryptedpayload-create.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|新しい[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトを作成します。|
|[OnPremEncryptedPayload の削除](../api/intune-raimportcerts-onpremencryptedpayload-delete.md)|None|[OnPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)を削除します。|
|[OnPremEncryptedPayload の更新](../api/intune-raimportcerts-onpremencryptedpayload-update.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|[OnPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|tenantId|Guid|まだ文書化されていません|
|userId|Guid|まだ文書化されていません|
|deviceId|Guid|まだ文書化されていません|
|payloadId|Guid|まだ文書化されていません|
|deviceKeyThumbprint|String|まだ文書化されていません|
|cert1PayloadUUID|String|まだ文書化されていません|
|cert2PayloadUUID|String|まだ文書化されていません|
|cert3PayloadUUID|String|まだ文書化されていません|
|plistTemplate|String|まだ文書化されていません|
|encryptedBlob|Binary|まだ文書化されていません|
|payloadVersion|Int32|まだ文書化されていません|
|status|Int32|まだ文書化されていません|
|createdTime|DateTimeOffset|まだ文書化されていません|
|lastModifiedTime|DateTimeOffset|まだ文書化されていません|
|eTag|String|まだ文書化されていません|
|isDeleted|ブール型 (Boolean)|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremEncryptedPayload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "Guid",
  "userId": "Guid",
  "deviceId": "Guid",
  "payloadId": "Guid",
  "deviceKeyThumbprint": "String",
  "cert1PayloadUUID": "String",
  "cert2PayloadUUID": "String",
  "cert3PayloadUUID": "String",
  "plistTemplate": "String",
  "encryptedBlob": "binary",
  "payloadVersion": 1024,
  "status": 1024,
  "createdTime": "String (timestamp)",
  "lastModifiedTime": "String (timestamp)",
  "eTag": "String",
  "isDeleted": true
}
```





