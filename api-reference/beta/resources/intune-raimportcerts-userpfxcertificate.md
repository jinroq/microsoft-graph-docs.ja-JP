---
title: userPFXCertificate リソースの種類
description: PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 95ae97b44a82d5ec87e3e2622a519debcfd8d7c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406039"
---
# <a name="userpfxcertificate-resource-type"></a>userPFXCertificate リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

PFX 証明書のユーザーのために必要なすべての情報をカプセル化するエンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)コレクション|[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[UserPFXCertificate を取得します。](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティと関係を参照してください。|
|[UserPFXCertificate を作成します。](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|新しい[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトを作成します。|
|[UserPFXCertificate を削除します。](../api/intune-raimportcerts-userpfxcertificate-delete.md)|なし|の[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)を削除します。|
|[UserPFXCertificate を更新します。](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|PFX 証明書の一意の識別子です。|
|拇印|String|PFX 証明書の拇印を sha-1 です。|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|証明書からのポイントからのビューの展開の目的のものです。 可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。|
|userPrincipalName|String|PFX 証明書のユーザー プリンシパル名です。|
|startDateTime|DateTimeOffset|証明書の有効性は、日付と時刻を開始します。|
|expirationDateTime|DateTimeOffset|証明書の有効期限切れ日時です。|
|プロバイダー|String|暗号サービス プロバイダーがこの blob の暗号化に使用します。|
|キー名|String|(プロバイダー) 内のキーの名前が blob の暗号化に使用します。|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|暗号化/復号化中に、プロバイダーによって使用されるスキームをパディングします。 使用可能な値: `none`、`pkcs1`、`oaepSha1`、`oaepSha256`、`oaepSha384`、`oaepSha512`。|
|encryptedPfxBlob|Binary|PFX の暗号化された blob です。|
|encryptedPfxPassword|String|PFX パスワードを暗号化します。|
|createdDateTime|DateTimeOffset|PFX 証明書がインポートされたときに、日付と時刻。|
|lastModifiedDateTime|DateTimeOffset|PFX 証明書が最後に修正された日時です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




