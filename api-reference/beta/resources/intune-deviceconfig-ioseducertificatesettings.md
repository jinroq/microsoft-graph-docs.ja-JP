---
title: iosEduCertificateSettings リソースの種類
description: 信頼されたルートと PFX 証明書 EDU の入出力数のです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c48883caa9479638b1a727272abdd0bc5762db9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948676"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

信頼されたルートと PFX 証明書 EDU の入出力数のです。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|trustedRootCertificate|Binary|信頼されたルート証明書です。|
|します|String|UI に表示するファイル名です。|
|certificationAuthority|String|PKCS 証明機関。|
|certificationAuthorityName|String|PKCS 証明機関の名前です。|
|certificateTemplateName|String|PKCS の証明書テンプレートの名前です。|
|renewalThresholdPercentage|Int32|証明書の書き換えのしきい値の割合です。 1 から 99 までの有効な値|
|certificateValidityPeriodValue|Int32|証明書の有効期間の値です。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|証明書の有効期間のスケールです。 可能な値は、`days`、`months`、`years` です。|

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





