---
title: メール アプリ使用状況レポート
description: Exchange Online への接続に使用されている電子メールアプリの数を確認できます。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 7f332359af9a6147894bb69e6d12532a83394bb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506686"
---
# <a name="email-app-usage-reports"></a>メール アプリ使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exchange Online への接続に使用されている電子メールアプリの数を確認できます。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [emailapp使い方 userdetail](../resources/emailappusageuserdetail.md) | メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。 |
| [アプリのユーザーの数を取得する](../api/reportroot-getemailappusageappsusercounts.md) | Stream          | [emailapp使い方 appsuser計数](../resources/emailappusageappsusercounts.md) | メール アプリごとの、それぞれ別個のユーザーの数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getemailappusageusercounts.md) | ストリーム          | [emailapp使い方 user計数](../resources/emailappusageusercounts.md) | 任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。 |
| [バージョンのユーザーの数を取得する](../api/reportroot-getemailappusageversionsusercounts.md) | Stream          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
