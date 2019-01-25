---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526866"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 

> **注:** この複合型は抽象です。 特定の種類の接続設定のリストを参照してください。

## <a name="derived-types"></a>派生型
| 型 | 説明 | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | OAuth1 接続の設定を提供するのにには、この型を使用します。 |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | OAuth2 クライアントの資格情報の付与の接続の設定を提供するのにには、この型を使用します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **clientId** | String |  クライアント ID をプロバイダーに接続するために使用します。 |
| client_secret | String |  プロバイダーへの接続を認証するためにクライアント シークレット。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
