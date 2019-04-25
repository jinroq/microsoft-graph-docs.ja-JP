---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、システムはプロバイダ api への接続方法を知ることができます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542992"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロバイダー接続の設定を表します。 これにより、システムはプロバイダ api への接続方法を知ることができます。 

> **注:** この複合型は抽象型です。 一覧にある特定の種類の接続設定を参照してください。

## <a name="derived-types"></a>派生型
| 型 | 説明 | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | この型を使用して、OAuth1 の接続設定を提供します。 |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | この種類を使用して、OAuth2 クライアント資格情報の付与に接続設定を提供します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **clientId** | String |  プロバイダーへの接続に使用されるクライアント ID。 |
| **clientSecret** | String |  プロバイダーへの接続を認証するクライアントシークレット。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
