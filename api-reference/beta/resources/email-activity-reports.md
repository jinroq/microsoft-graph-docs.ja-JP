---
title: 電子メール アクティビティ レポート
description: 組織内の電子メールトラフィックの高レベルのビューは、[レポート] ページから入手できます。 また、電子メールアクティビティウィジェットにドリルインして、組織内の電子メールアクティビティのユーザーごとの傾向と詳細を把握することもできます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 748199a2e846cc71a3f04c3ea1bda97dcf2c7301
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542913"
---
# <a name="email-activity-reports"></a>電子メール アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織内の電子メールトラフィックの高レベルのビューは、[レポート] ページから入手できます。 また、電子メールアクティビティウィジェットにドリルインして、組織内の電子メールアクティビティのユーザーごとの傾向と詳細を把握することもできます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [emailactivityuserdetail](../resources/emailactivityuserdetail.md) | ユーザーが実行した電子メール アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getemailactivitycounts.md) | Stream          | [emailactivitysummary](../resources/emailactivitysummary.md) | 組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。 |
| [ユーザーの数を取得する](../api/reportroot-getemailactivityusercounts.md) | Stream          | [emailactivitysummary](../resources/emailactivitysummary.md) | 送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
