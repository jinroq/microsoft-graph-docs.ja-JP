---
title: pfxUserCertificate リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9f709281d4ca0711fab6d2cf9a5c8fd453ba32b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741476"
---
# <a name="pfxusercertificate-resource-type"></a>pfxUserCertificate リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト pfxUserCertificates](../api/intune-raimportcerts-pfxusercertificate-list.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)コレクション|[PfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[PfxUserCertificate を取得する](../api/intune-raimportcerts-pfxusercertificate-get.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|[PfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[PfxUserCertificate を作成する](../api/intune-raimportcerts-pfxusercertificate-create.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|新しい[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトを作成します。|
|[PfxUserCertificate の削除](../api/intune-raimportcerts-pfxusercertificate-delete.md)|None|[PfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)を削除します。|
|[PfxUserCertificate の更新](../api/intune-raimportcerts-pfxusercertificate-update.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|[PfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|tenantId|Guid|まだ文書化されていません|
|userId|Guid|まだ文書化されていません|
|拇印|String|まだ文書化されていません|
|userUpn|String|まだ文書化されていません|
|encryptedPfxBlob|String|まだ文書化されていません|
|encryptedPfxPassword|String|まだ文書化されていません|
|certStartDate|DateTimeOffset|まだ文書化されていません|
|certExpirationDate|DateTimeOffset|まだ文書化されていません|
|プロバイダー|String|まだ文書化されていません|
|encryptionKeyName|String|まだ文書化されていません|
|paddingScheme|Int32|まだ文書化されていません|
|status|Int32|まだ文書化されていません|
|intendedPurpose|Int32|まだ文書化されていません|
|createdTime|DateTimeOffset|まだ文書化されていません|
|isDeleted|ブール型 (Boolean)|まだ文書化されていません|
|lastModifiedTime|DateTimeOffset|まだ文書化されていません|
|eTag|String|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxUserCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "Guid",
  "userId": "Guid",
  "thumbprint": "String",
  "userUpn": "String",
  "encryptedPfxBlob": "String",
  "encryptedPfxPassword": "String",
  "certStartDate": "String (timestamp)",
  "certExpirationDate": "String (timestamp)",
  "providerName": "String",
  "encryptionKeyName": "String",
  "paddingScheme": 1024,
  "status": 1024,
  "intendedPurpose": 1024,
  "createdTime": "String (timestamp)",
  "isDeleted": true,
  "lastModifiedTime": "String (timestamp)",
  "eTag": "String"
}
```





