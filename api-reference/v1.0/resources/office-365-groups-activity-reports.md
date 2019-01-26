---
title: Office 365 グループ アクティビティ レポート
description: グループ アクティビティ レポートを使用して、組織内の Office 365 グループのアクティビティに関する洞察を得て、作成され、使用されている Office 365 グループの数を確認できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5d8c414034a110db64b770a72fe2e3540806acdd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573467"
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
