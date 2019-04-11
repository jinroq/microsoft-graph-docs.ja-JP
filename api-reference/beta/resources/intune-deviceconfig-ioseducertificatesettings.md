---
title: iosEduCertificateSettings リソースの種類
description: iOS EDU の信頼されたルートおよび PFX 証明書。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d9060c28744bae52d4690bf75487e298d58d2a1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800932"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS EDU の信頼されたルートおよび PFX 証明書。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|trustedRootCertificate|Binary|信頼されたルート証明書。|
|certfilename|文字列|UI に表示されるファイル名。|
|certificationAuthority|文字列|PKCS 証明機関。|
|certificationAuthorityName|文字列|PKCS 証明機関名。|
|certificatetemplatename|文字列|PKCS 証明書テンプレート名。|
|renewalThresholdPercentage|Int32|証明書の更新しきい値の割合。 有効な値は 1 ~ 99|
|certificateValidityPeriodValue|Int32|証明書の有効期間の値。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|証明書の有効期間のスケール。 可能な値は、`days`、`months`、`years` です。|

## <a name="relationships"></a>関係
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





