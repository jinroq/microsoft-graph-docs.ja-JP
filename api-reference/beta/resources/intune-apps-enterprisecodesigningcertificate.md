---
title: enterpriseCodeSigningCertificate リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: f16dbbf59af238e631e282d7e4d92dad46a7083b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328701"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>enterpriseCodeSigningCertificate リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)コレクション|[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[EnterpriseCodeSigningCertificate を取得します。](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティと関係を参照してください。|
|[EnterpriseCodeSigningCertificate を作成します。](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|新しい[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトを作成します。|
|[EnterpriseCodeSigningCertificate を削除します。](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|なし|の[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)を削除します。|
|[EnterpriseCodeSigningCertificate を更新します。](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|[EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|content|Binary|生データの形式で Windows エンタープライズ コード署名証明書。|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|証明書の状態は、準備または準備されていません。 使用可能な値は、`notProvisioned`、`provisioned` です。|
|subjectName|文字列型 (String)|証明書のサブジェクト名。|
|subject|String|証明書のサブジェクト値。|
|issuerName|String|証明書の発行者の名前です。|
|発行者|String|証明書の発行者の値です。|
|expirationDateTime|DateTimeOffset|証明書の有効期限日です。|
|uploadDateTime|DateTimeOffset|コード署名証明書のアップロード時の日時です。|

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





