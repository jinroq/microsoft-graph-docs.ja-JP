---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f9bb19ec9c09b06dd007eb2031f3dbb176eb12d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978229"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>educationSynchronizationConnectionSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

プロバイダー接続の設定を表します。 これにより、Api のプロバイダーに接続する方法を把握するシステムです。 

> **注:** この複合型は抽象です。 特定の種類の接続設定のリストを参照してください。

## <a name="derived-types"></a>派生型
| Type | 説明 | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | OAuth1 接続の設定を提供するのにには、この型を使用します。 |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | OAuth2 クライアントの資格情報の付与の接続の設定を提供するのにには、この型を使用します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **clientId** | String |  クライアント ID をプロバイダーに接続するために使用します。 |
| **clientSecret** | String |  プロバイダーへの接続を認証するためにクライアント シークレット。 |
