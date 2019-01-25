---
title: OneDrive 使用状況レポート
description: OneDrive ファイルと OneDrive のすべてのアカウントが組織内で使用されているストレージの合計数から取得する値の高度なビューを取得できます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 できます、単位の OneDrive のアカウントの詳細。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c5a73b33f4422440df8817c3f6a69299eedeae50
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519837"
---
# <a name="onedrive-usage-reports"></a>OneDrive 使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneDrive ファイルと OneDrive のすべてのアカウントが組織内で使用されているストレージの合計数から取得する値の高度なビューを取得できます。 さらにドリルダウンすると、アクティブな OneDrive アカウントの傾向、ユーザーが操作したファイルの数、使用したストレージの量などを把握することができます。 できます、単位の OneDrive のアカウントの詳細。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: OneDrive for Business の使用状況](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [アカウントの詳細を取得する](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) | アカウント別の OneDrive の使用状況に関する詳細を取得します。 |
| [アカウントの数を取得する](../api/reportroot-getonedriveusageaccountcounts.md) | Stream          | [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) | アクティブな OneDrive for Business サイトの数の傾向を取得します。 ユーザーがファイルを表示、変更、アップロード、ダウンロード、共有、同期したサイトはすべて、アクティブなサイトとみなされます。 |
| [ファイルの数を取得する](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | すべてのサイトのファイル合計数と、アクティブ ファイルの数を取得します。 ファイルは一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。 |
| [ストレージを取得する](../api/reportroot-getonedriveusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | OneDrive for Business で使用しているストレージの量の傾向を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
