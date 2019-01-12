---
title: Microsoft Teams ユーザー アクティビティ レポート
description: 組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2dd3ed3cde8f1a00ae7a48336bfaef857721f046
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991434"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams ユーザー アクティビティ レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。 21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。

組織でマイクロソフトのチームのユーザーの利用状況の洞察を取得するのにには、マイクロソフト チームのユーザー アクティビティ レポートを使用します。

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型                              | 説明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | アクティビティの種類ごとに、ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。 |
