---
title: educationSynchronizationConnectionSettings リソースの種類
description: 'プロバイダー接続の設定を表します。 これにより、システムはプロバイダ api への接続方法を知ることができます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334115"
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
