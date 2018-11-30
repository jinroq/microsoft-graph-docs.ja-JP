---
title: Yammer グループ アクティビティ レポート
description: 組織で Yammer グループの活動の洞察を獲得でき、Yammer グループの数が表示されるを参照してください作成され、使用されます。
ms.openlocfilehash: faaf270d53108892870a32b7c7296b51f0022fea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069981"
---
# <a name="yammer-groups-activity-reports"></a>Yammer グループ アクティビティ レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。 21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。

組織で Yammer グループの活動の洞察を獲得でき、Yammer グループの数が表示されるを参照してください作成され、使用されます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [グループの詳細を取得する](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | グループ別の Yammer グループ アクティビティに関する詳細を取得します。 |
| [グループの数を取得する](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | 存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。 |
