---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 '
author: mmast-msft
ms.openlocfilehash: 4e8b62a46fa6d14508a9d57ffedc46411910433d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350625"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 

> **注:** この複合型は抽象です。 特定の種類の接続設定のリストを参照してください。

## <a name="derived-types"></a>派生型
| 種類 | 説明 | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | OAuth1 接続の設定を提供するのにには、この型を使用します。 |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | OAuth2 クライアントの資格情報の付与の接続の設定を提供するのにには、この型を使用します。 |

## <a name="properties"></a>Properties

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **clientId** | String |  クライアント ID をプロバイダーに接続するために使用します。 |
| **clientSecret** | String |  プロバイダーへの接続を認証するためにクライアント シークレット。 |