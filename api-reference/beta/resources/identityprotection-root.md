---
title: Azure AD identity protection API を使用する (プレビュー)
description: Microsoft Graph を使用すると、Azure AD Id 保護によって検出されたリスクイベントの種類ごとに、identityRiskEvent リソースに対してクエリを実行できます。 これらのイベントは、Azure AD Premium P2 を使用しているお客様が利用できます。 Azure AD Premium P1 を使用しているお客様は、イベントのサブセットを利用できます。
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: d43f3a54e8ec8aebd0c8018cea9986c0c161a073
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005822"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Azure AD identity protection API を使用する (プレビュー)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph を使用すると、 [AZURE AD Id 保護](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)によって検出されたリスクイベントの種類ごとに、 [identityRiskEvent](identityriskevent.md)リソースに対してクエリを実行できます。 これらのイベントは、Azure AD Premium P2 を使用しているお客様が利用できます。 Azure AD Premium P1 を使用しているお客様は、イベントのサブセットを利用できます。

* [匿名 IP アドレスからのサインイン](anonymousipriskevent.md)
* [マルウェアに感染したデバイスからのサインイン](malwareriskevent.md)
* [例外的でない場所への移動は不可能](impossibletravelriskevent.md)
* [資格情報が漏洩したユーザー](leakedcredentialsriskevent.md)
* [疑わしい IP アドレスからのサインイン](suspiciousipriskevent.md)
* [見慣れない場所からのサインイン](unfamiliarlocationriskevent.md)

これらのイベントと関連情報を取得するには、次の操作を使用します。

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[identityRiskEvent を一覧表示する](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| IdentityRiskEvent コレクションを取得します。 |
|[identityRiskEvent を取得する](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| IdentityRiskEvent オブジェクトを取得します。 |
|[anonymousIpRiskEvent を一覧表示する](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| AnonymousIpRiskEvent コレクションを取得します。 |
|[anonymousIpRiskEvent を取得する](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| AnonymousIpRiskEvent オブジェクトを取得します。 |
|[impossibleTravelRiskEvent を一覧表示する](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| ImpossibleTravelRiskEvent コレクションを取得します。 |
|[impossibleTravelRiskEvent を取得する](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| ImpossibleTravelRiskEvent オブジェクトを取得します。 |
|[leakedCredentialsRiskEvent を一覧表示する](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| LeakedCredentialsRiskEvent コレクションを取得します。 |
|[leakedCredentialsRiskEvent を取得する](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| LeakedCredentialsRiskEvent オブジェクトを取得します。 |
|[malwareRiskEvent を一覧表示する](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| MalwareRiskEvent コレクションを取得します。 |
|[malwareRiskEvent を取得する](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| MalwareRiskEvent オブジェクトを取得します。 |
|[suspiciousIpRiskEvent を一覧表示する](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| SuspiciousIpRiskEvent コレクションを取得します。 |
|[suspiciousIpRiskEvent を取得する](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| SuspiciousIpRiskEvent オブジェクトを取得します。 |
|[unfamiliarLocationRiskEvent を一覧表示する](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| UnfamiliarLocationRiskEvent コレクションを取得します。 |
|[unfamiliarLocationRiskEvent を取得する](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| UnfamiliarLocationRiskEvent オブジェクトを取得します。 |

# <a name="see-also"></a>関連項目

* [Azure Active Directory Id 保護について](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Azure Active Directory id 保護と Microsoft Graph の概要](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
