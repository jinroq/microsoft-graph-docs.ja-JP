---
title: iosVpnSecurityAssociationParameters リソースの種類
description: VPN セキュリティアソシエーションのパラメーター
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ecf2597222a578d342f69c16c665c493b8c3329
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002729"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a>iosVpnSecurityAssociationParameters リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN セキュリティアソシエーションのパラメーター

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|securityEncryptionAlgorithm|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|暗号化アルゴリズム。 使用可能な値: `aes256`、`des`、`tripleDes`、`aes128`、`aes128Gcm`、`aes256Gcm`。|
|securityIntegrityAlgorithm|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|整合性アルゴリズム。 可能な値は、`sha2_256`、`sha1_96`、`sha1_160`、`sha2_384`、`sha2_512` です。|
|securityDiffieHellmanGroup|Int32|Diffie-hellman グループ|
|lifetimeInMinutes|Int32|有効期間 (分)|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```





