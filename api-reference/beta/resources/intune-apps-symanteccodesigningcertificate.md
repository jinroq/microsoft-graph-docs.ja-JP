---
title: symantecCodeSigningCertificate リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea5578f39f607a66770a040c4b88fbc2d75e8ffc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949732"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>symantecCodeSigningCertificate リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[SymantecCodeSigningCertificate を取得する](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[SymantecCodeSigningCertificate の更新](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|content|Binary|Windows Symantec コード署名証明書が生データ形式で表示されます。|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|証明書の状態がプロビジョニングされているか、プロビジョニングされていません。 可能な値は、`notProvisioned`、`provisioned` です。|
|パスワード|String|.Pfx ファイルに必要なパスワードを指定します。|
|subjectName|String|証明書のサブジェクト名。|
|subject|String|証明書のサブジェクトの値。|
|issuerName|String|証明書の発行者名。|
|会社|String|証明書の発行者の値。|
|expirationDateTime|DateTimeOffset|証明書の有効期限。|
|uploadDateTime|DateTimeOffset|Symantec Cert としての CodeSigning Cert の種類。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```




