---
title: Yammer グループ アクティビティ レポート
description: 組織内の Yammer グループのアクティビティについての洞察を得て、作成され、使用されている Yammer グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 07a78a4b2047e03beee611443240f56739f76b4f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963842"
---
# <a name="yammer-groups-activity-reports"></a>Yammer グループ アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織内の Yammer グループのアクティビティについての洞察を得て、作成され、使用されている Yammer グループの数を確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer グループ アクティビティ](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [グループの詳細を取得する](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | グループ別の Yammer グループ アクティビティに関する詳細を取得します。 |
| [グループの数を取得する](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | 存在したグループ、およびグループ会話アクティビティを含んだグループの合計数を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | グループ内で投稿、読み取り、および「いいね!」を付けた Yammer メッセージの数を取得します。 |
