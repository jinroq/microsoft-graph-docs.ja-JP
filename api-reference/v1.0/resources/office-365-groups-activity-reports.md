---
title: Office 365 グループ アクティビティ レポート
description: グループ アクティビティ レポートを使用して、組織内の Office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている Office 365 グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a84584363e8cc3f3123225881179d400e50140b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982285"
---
# <a name="office-365-groups-activity-reports"></a>Office 365 グループ アクティビティ レポート

グループ アクティビティ レポートを使用して、組織内の Office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている Office 365 グループの数を確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Office 365 グループ](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [グループの詳細を取得する](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | グループ別の Office 365 グループ アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | グループ ワークロード全体のグループ活動の数を取得します。 |
| [グループの数を取得する](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | グループの日次合計数と、そのうちのアクティブなグループの数を、電子メールでの会話、Yammer の投稿、SharePoint ファイルのアクティビティに基づいて取得します。 |
| [ストレージを取得する](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | すべてのグループ メールボックスとグループ サイトで使用されているストレージの合計を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | Office 365 グループに関連付けられたグループ サイト全体での、ファイルの合計数と、そのうちのアクティブにされたファイルの数を取得します。 |
