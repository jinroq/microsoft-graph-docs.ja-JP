---
title: Office 365 アクティブ ユーザー レポート
description: 製品ライセンスの数は、個人、組織内で使用されているを確認するのには Office 365 のユーザーのアクティブなレポートを使用し、ユーザーについては、どのような製品を使用している情報にドリルダウンできます。 このレポートは、管理者が使用率の低い製品またはその他のトレーニングや情報が必要なユーザーの識別に役立ちます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e85924b7066dde92f0db5fd0b3f1f83dd32fd0c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516211"
---
# <a name="office-365-active-users-reports"></a>Office 365 アクティブ ユーザー レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

製品ライセンスの数は、個人、組織内で使用されているを確認するのには Office 365 のユーザーのアクティブなレポートを使用し、ユーザーについては、どのような製品を使用している情報にドリルダウンできます。 このレポートは、管理者が使用率の低い製品またはその他のトレーニングや情報が必要なユーザーの識別に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Office 365 アクティブ ユーザーに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activeusercounts.md) | ストリーム          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。 |
| [サービスのユーザーの数を取得する](../api/reportroot-getoffice365servicesusercounts.md) | Stream          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | アクティビティの種類とサービス別のユーザー数を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
