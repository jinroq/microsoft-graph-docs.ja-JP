---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアント資格情報の付与を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507041"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[OAuth2 クライアント資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。

[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **tokenurl** | String | データプロバイダーのアクセストークンを取得する URL。 |
| **scope** | String | [アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)。 |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth2clientcredentialsconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
