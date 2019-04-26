---
title: Office 365 グループ アクティビティ レポート
description: 組織内の office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている office 365 グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a46e1823acd63616f10ce2569a72a0099e390f93
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342022"
---
# <a name="office-365-groups-activity-reports"></a>Office 365 グループ アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織内の office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている office 365 グループの数を確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [グループの詳細を取得する](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | グループ別の Office 365 グループ アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getoffice365groupsactivitycounts.md) | ストリーム          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | グループ ワークロード全体のグループ活動の数を取得します。 |
| [グループの数を取得する](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。 |
| [ストレージを取得する](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Office 365 グループに関連付けられたグループ サイト全体での、ファイルの合計数と、そのうちのアクティブにされたファイルの数を取得します。 |
