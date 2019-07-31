---
title: iosEduCertificateSettings リソースの種類
description: IOS EDU の信頼されたルートおよび PFX 証明書。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd063ec70dd794ffb151036ea7bbbda090829343
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001257"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

IOS EDU の信頼されたルートおよび PFX 証明書。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|trustedRootCertificate|Binary|信頼されたルート証明書。|
|certFileName|String|UI に表示されるファイル名。|
|certificationAuthority|String|PKCS 証明機関。|
|certificationAuthorityName|String|PKCS 証明機関名。|
|certificateTemplateName|String|PKCS 証明書テンプレート名。|
|renewalThresholdPercentage|Int32|証明書の更新しきい値の割合。 有効な値は 1 ~ 99|
|certificateValidityPeriodValue|Int32|証明書の有効期間の値。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|証明書の有効期間のスケール。 可能な値は、`days`、`months`、`years` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```





