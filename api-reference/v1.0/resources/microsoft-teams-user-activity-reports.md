---
title: Microsoft Teams ユーザー アクティビティ レポート
description: Microsoft Teams アクティビティ レポートを使用して、組織内の Microsoft Teams ユーザー アクティビティに関する洞察を得ます。
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: 8ecf68174edb85b2bbf91a6052a6d96ad425dbe6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966336"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams ユーザー アクティビティ レポート

Microsoft Teams アクティビティ レポートを使用して、組織内の Microsoft Teams ユーザー アクティビティに関する洞察を得ます。

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsuseractivityuserdetail.md) | ストリーム      | ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getteamsuseractivitycounts.md) | ストリーム      | アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsuseractivityusercounts.md) | ストリーム      | アクティビティの種類ごとに、ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。 |
