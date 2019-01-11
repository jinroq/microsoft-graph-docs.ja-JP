---
title: SharePoint サイト使用状況レポート
description: ユーザーが SharePoint サイト、ファイルの数を使用しているアクティブに、これらすべてのサイト間で使用されるストレージに保存されているファイルの合計数の点で SharePoint から取得する値の高レベルのビューを取得できます。 傾向を理解するのには、SharePoint サイトの利用状況レポートに、サイト レベルの詳細のすべてのサイトごとにドリルダウンできます。
localization_priority: Normal
ms.openlocfilehash: 287abafdf279b2a249481ebc4445bfcd980ebc76
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856142"
---
# <a name="sharepoint-site-usage-reports"></a>SharePoint サイト使用状況レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
