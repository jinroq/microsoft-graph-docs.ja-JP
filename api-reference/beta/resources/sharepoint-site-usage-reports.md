---
title: SharePoint サイト使用状況レポート
description: ユーザーが SharePoint サイト、ファイルの数を使用しているアクティブに、これらすべてのサイト間で使用されるストレージに保存されているファイルの合計数の点で SharePoint から取得する値の高レベルのビューを取得できます。 傾向を理解するのには、SharePoint サイトの利用状況レポートに、サイト レベルの詳細のすべてのサイトごとにドリルダウンできます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f9186c4caca6afe3f96eca8db2c6fc34131f0b98
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508140"
---
# <a name="sharepoint-site-usage-reports"></a>SharePoint サイト使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーが SharePoint サイト、ファイルの数を使用しているアクティブに、これらすべてのサイト間で使用されるストレージに保存されているファイルの合計数の点で SharePoint から取得する値の高レベルのビューを取得できます。 傾向を理解するのには、SharePoint サイトの利用状況レポートに、サイト レベルの詳細のすべてのサイトごとにドリルダウンできます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint サイトの使用状況](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [サイトの詳細を取得する](../api/reportroot-getsharepointsiteusagedetail.md) | Stream          | [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) | SharePoint サイトの使用状況に関する詳細を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) | すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。 ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。 |
| [サイトの数を取得する](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream          | [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) | すべてのサイトのファイルの合計数と、アクティブ ファイルの数を取得します。 ファイル (ユーザーまたはシステム) は、一定期間中に保存、同期、変更、共有されるとアクティブとみなされます。 |
| [ストレージを取得する](../api/reportroot-getsharepointsiteusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | レポート期間中に割り当てられ、消費したストレージの傾向を取得します。 |
| [ページを取得する](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) | すべてのサイトで表示されたページ数を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-site-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
