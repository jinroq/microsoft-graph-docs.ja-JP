---
title: pfxRecryptionRequest リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 308b487ad77558ef5e847599e7b4a130c2ef6603
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741468"
---
# <a name="pfxrecryptionrequest-resource-type"></a>pfxRecryptionRequest リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト pfxRecryptionRequests](../api/intune-raimportcerts-pfxrecryptionrequest-list.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)コレクション|[PfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[PfxRecryptionRequest を取得する](../api/intune-raimportcerts-pfxrecryptionrequest-get.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|[PfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[PfxRecryptionRequest を作成する](../api/intune-raimportcerts-pfxrecryptionrequest-create.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|新しい[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトを作成します。|
|[PfxRecryptionRequest の削除](../api/intune-raimportcerts-pfxrecryptionrequest-delete.md)|None|[PfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)を削除します。|
|[PfxRecryptionRequest の更新](../api/intune-raimportcerts-pfxrecryptionrequest-update.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|[PfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|tenantId|Guid|まだ文書化されていません|
|userId|Guid|まだ文書化されていません|
|deviceId|Guid|まだ文書化されていません|
|profileId|Guid|まだ文書化されていません|
|拇印|String|まだ文書化されていません|
|deviceKeyThumbprint|String|まだ文書化されていません|
|status|Int32|まだ文書化されていません|
|sourceType|Int32|まだ文書化されていません|
|createdTime|DateTimeOffset|まだ文書化されていません|
|lastModifiedTime|DateTimeOffset|まだ文書化されていません|
|isDeleted|ブール型 (Boolean)|まだ文書化されていません|
|eTag|String|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxRecryptionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "Guid",
  "userId": "Guid",
  "deviceId": "Guid",
  "profileId": "Guid",
  "thumbprint": "String",
  "deviceKeyThumbprint": "String",
  "status": 1024,
  "sourceType": 1024,
  "createdTime": "String (timestamp)",
  "lastModifiedTime": "String (timestamp)",
  "isDeleted": true,
  "eTag": "String"
}
```





