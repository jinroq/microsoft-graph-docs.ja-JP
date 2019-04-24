---
title: Microsoft Teams ユーザー アクティビティ レポート
description: microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457082"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams ユーザー アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型                              | 説明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsuseractivityuserdetail](../resources/teamsuseractivityuserdetail.md) | ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getteamsuseractivitycounts.md) | [teamsuseractivitycounts](../resources/teamsuseractivitycounts.md) | アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。 アクティビティの種類は、チームのチャット メッセージ数、プライベート チャット メッセージ数、コール数、または会議数です。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsuseractivityusercounts](../resources/teamsuseractivityusercounts.md) | アクティビティの種類ごとに、ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
