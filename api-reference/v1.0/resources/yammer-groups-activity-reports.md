---
title: Yammer グループ アクティビティ レポート
description: Yammer グループ アクティビティ レポートを使用して、組織内の Yammer グループのアクティビティに関する洞察を得て、作成され、使用されている Yammer グループの数を確認できます。
localization_priority: Normal
ms.openlocfilehash: 9f4c9fa3462517f630e6cacfd7d713d78fe22d3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845354"
---
# <a name="yammer-groups-activity-reports"></a>Yammer グループ アクティビティ レポート

Yammer グループ アクティビティ レポートを使用して、組織内の Yammer グループのアクティビティに関する洞察を得て、作成され、使用されている Yammer グループの数を確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [グループの詳細を取得する](../api/reportroot-getyammergroupsactivitydetail.md) | Stream      | グループ別の Yammer グループ アクティビティに関する詳細を取得します。 |
| [グループの数を取得する](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream      | 存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getyammergroupsactivitycounts.md) | Stream      | グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。 |
