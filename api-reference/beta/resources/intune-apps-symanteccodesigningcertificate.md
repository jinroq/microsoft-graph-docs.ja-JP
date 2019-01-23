---
title: symantecCodeSigningCertificate リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f22f86f6facfbe1b21bb0f857b8401393ed1a77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425996"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>symantecCodeSigningCertificate リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[SymantecCodeSigningCertificate を取得します。](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティと関係を参照してください。|
|[SymantecCodeSigningCertificate を更新します。](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|content|Binary|生データの形式で Windows のシマンテック社のコード署名証明書。|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|証明書の状態は、準備または準備されていません。 使用可能な値は、`notProvisioned`、`provisioned` です。|
|password|String|.Pfx ファイルに必要なパスワードです。|
|subjectName|文字列型 (String)|証明書のサブジェクト名。|
|subject|String|証明書のサブジェクト値。|
|issuerName|String|証明書の発行者の名前です。|
|発行者|String|証明書の発行者の値です。|
|expirationDateTime|DateTimeOffset|証明書の有効期限日です。|
|uploadDateTime|DateTimeOffset|シマンテック社の証明書とコード署名証明書の種類です。|

## <a name="relationships"></a>リレーションシップ
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




