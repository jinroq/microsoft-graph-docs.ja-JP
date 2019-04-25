---
title: enterpriseCodeSigningCertificate リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 213915889ad575af61fcdda7ee7306c0b38370c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552269"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>enterpriseCodeSigningCertificate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)コレクション|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[enterpriseCodeSigningCertificate を取得する](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[enterpriseCodeSigningCertificate を作成する](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|新しい[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを作成します。|
|[enterpriseCodeSigningCertificate の削除](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|なし|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)を削除します。|
|[enterpriseCodeSigningCertificate の更新](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|content|Binary|未加工のデータ形式の Windows エンタープライズコード署名証明書。|
|status|[certificatestatus](../resources/intune-apps-certificatestatus.md)|証明書の状態がプロビジョニングされているか、プロビジョニングされていません。 可能な値は、`notProvisioned`、`provisioned` です。|
|subjectName|文字列型 (String)|証明書のサブジェクト名。|
|subject|String|証明書のサブジェクトの値。|
|issuerName|String|証明書の発行者名。|
|会社|String|証明書の発行者の値。|
|expirationDateTime|DateTimeOffset|証明書の有効期限。|
|uploaddatetime|DateTimeOffset|CodeSigning Cert がアップロードされたときの日付時刻。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enterpriseCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```





