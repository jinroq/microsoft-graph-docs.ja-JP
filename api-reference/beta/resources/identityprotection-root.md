---
title: Azure AD id 保護 API (プレビュー) を使用します。
description: Azure AD のアイデンティティ保護によって検出されたリスク イベントの種類ごとに identityRiskEvent リソースを照会するのにには、Microsoft Graph を使用します。 Azure AD プレミアム p2 のお客様にこれらのイベントを利用できます。 イベントのサブセットでは、Azure AD プレミアム P1 で使用可能です。
ms.openlocfilehash: 10b2e7dc59c8a9aeef25aa4ed5e27667b12a8eee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071456"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Azure AD id 保護 API (プレビュー) を使用します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[Azure AD のアイデンティティ保護](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)によって検出されたリスク イベントの種類ごとに[identityRiskEvent](identityriskevent.md)リソースを照会するのにには、Microsoft Graph を使用します。 Azure AD プレミアム p2 のお客様にこれらのイベントを利用できます。 イベントのサブセットでは、Azure AD プレミアム P1 で使用可能です。

* [匿名の IP アドレスからサインイン](anonymousipriskevent.md)
* [マルウェアに感染したデバイスからのサインインの問題](malwareriskevent.md)
* [典型的な場所に旅行を不可能になります。](impossibletravelriskevent.md)
* [リークした資格情報を持つユーザー](leakedcredentialsriskevent.md)
* [不審な IP アドレスからサインイン](suspiciousipriskevent.md)
* [未知の場所からサインイン](unfamiliarlocationriskevent.md)

これらのイベントと関連付けられている情報を取得するのにには、次の操作を使用します。

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リスト identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| IdentityRiskEvent コレクションを取得します。 |
|[IdentityRiskEvent を取得します。](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| IdentityRiskEvent オブジェクトを取得します。 |
|[リスト anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| AnonymousIpRiskEvent コレクションを取得します。 |
|[AnonymousIpRiskEvent を取得します。](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| AnonymousIpRiskEvent オブジェクトを取得します。 |
|[リスト impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| ImpossibleTravelRiskEvent コレクションを取得します。 |
|[ImpossibleTravelRiskEvent を取得します。](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| ImpossibleTravelRiskEvent オブジェクトを取得します。 |
|[リスト leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| LeakedCredentialsRiskEvent コレクションを取得します。 |
|[LeakedCredentialsRiskEvent を取得します。](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| LeakedCredentialsRiskEvent オブジェクトを取得します。 |
|[リスト malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| MalwareRiskEvent コレクションを取得します。 |
|[MalwareRiskEvent を取得します。](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| MalwareRiskEvent オブジェクトを取得します。 |
|[リスト suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| SuspiciousIpRiskEvent コレクションを取得します。 |
|[SuspiciousIpRiskEvent を取得します。](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| SuspiciousIpRiskEvent オブジェクトを取得します。 |
|[リスト unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| UnfamiliarLocationRiskEvent コレクションを取得します。 |
|[UnfamiliarLocationRiskEvent を取得します。](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| UnfamiliarLocationRiskEvent オブジェクトを取得します。 |

# <a name="see-also"></a>関連項目

* [Azure Active Directory Id の保護について](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Azure Active Directory アイデンティティ保護と Microsoft Graph を使用します。](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
