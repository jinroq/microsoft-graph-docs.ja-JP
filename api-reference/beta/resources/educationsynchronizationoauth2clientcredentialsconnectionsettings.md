---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアント資格情報の付与を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ffc3af93a90ba0d6991007a64d24b9fb776e8bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972370"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[OAuth2 クライアント資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。

[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **tokenUrl** | String | データプロバイダーのアクセストークンを取得する URL。 |
| **scope** | String | [アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)。 |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
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
