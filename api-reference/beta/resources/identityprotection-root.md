---
title: Azure AD identity protection API を使用する (プレビュー)
description: Microsoft Graph を使用すると、Azure AD id 保護によって検出されたリスクイベントの種類ごとに、identityRiskEvent リソースに対してクエリを実行できます。 これらのイベントは、Azure AD Premium P2 を使用しているお客様が利用できます。 Azure AD Premium P1 を使用しているお客様は、イベントのサブセットを利用できます。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 597ff7ed156dede995b10f07ee6ac6945745b83c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506378"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Azure AD identity protection API を使用する (プレビュー)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph を使用すると、 [Azure AD id 保護](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)によって検出されたリスクイベントの種類ごとに、 [identityRiskEvent](identityriskevent.md)リソースに対してクエリを実行できます。 これらのイベントは、Azure AD Premium P2 を使用しているお客様が利用できます。 Azure AD Premium P1 を使用しているお客様は、イベントのサブセットを利用できます。

* [匿名 IP アドレスからのサインイン](anonymousipriskevent.md)
* [マルウェアに感染したデバイスからのサインイン](malwareriskevent.md)
* [例外的でない場所への移動は不可能](impossibletravelriskevent.md)
* [資格情報が漏洩したユーザー](leakedcredentialsriskevent.md)
* [疑わしい IP アドレスからのサインイン](suspiciousipriskevent.md)
* [見慣れない場所からのサインイン](unfamiliarlocationriskevent.md)

これらのイベントと関連情報を取得するには、次の操作を使用します。

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[identityRiskEvent を一覧表示する](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| identityRiskEvent コレクションを取得します。 |
|[identityRiskEvent を取得する](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| identityRiskEvent オブジェクトを取得します。 |
|[anonymousIpRiskEvent を一覧表示する](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| anonymousIpRiskEvent コレクションを取得します。 |
|[anonymousIpRiskEvent を取得する](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| anonymousIpRiskEvent オブジェクトを取得します。 |
|[impossibleTravelRiskEvent を一覧表示する](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| impossibleTravelRiskEvent コレクションを取得します。 |
|[impossibleTravelRiskEvent を取得する](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| impossibleTravelRiskEvent オブジェクトを取得します。 |
|[leakedCredentialsRiskEvent を一覧表示する](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| leakedCredentialsRiskEvent コレクションを取得します。 |
|[leakedCredentialsRiskEvent を取得する](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| leakedCredentialsRiskEvent オブジェクトを取得します。 |
|[malwareRiskEvent を一覧表示する](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| malwareRiskEvent コレクションを取得します。 |
|[malwareRiskEvent を取得する](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| malwareRiskEvent オブジェクトを取得します。 |
|[suspiciousIpRiskEvent を一覧表示する](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| suspiciousIpRiskEvent コレクションを取得します。 |
|[suspiciousIpRiskEvent を取得する](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| suspiciousIpRiskEvent オブジェクトを取得します。 |
|[unfamiliarLocationRiskEvent を一覧表示する](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| unfamiliarLocationRiskEvent コレクションを取得します。 |
|[unfamiliarLocationRiskEvent を取得する](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| unfamiliarLocationRiskEvent オブジェクトを取得します。 |

# <a name="see-also"></a>関連項目

* [Azure Active Directory id 保護について](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Azure Active Directory id 保護と Microsoft Graph の概要](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityprotection-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
