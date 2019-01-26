---
title: Skype for Business アクティビティ レポート
description: 組織全体にわたってアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577383"
---
# <a name="skype-for-business-activity-reports"></a>Skype for Business アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織全体にわたってアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | ユーザー別の Skype for Business アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。 |
| [ユーザーの数を取得する](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
