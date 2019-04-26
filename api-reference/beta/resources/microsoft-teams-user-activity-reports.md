---
title: Microsoft Teams ユーザー アクティビティ レポート
description: microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f88d1c9d568ce3fbbf9bfe19abaf637065d37b8c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342206"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams ユーザー アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

microsoft teams ユーザーアクティビティレポートを使用して、組織内の microsoft teams ユーザーアクティビティの洞察を得ることができます。

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型                              | 説明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsuseractivityuserdetail](../resources/teamsuseractivityuserdetail.md) | ユーザーごとに、Microsoft Teams ユーザー アクティビティの詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getteamsuseractivitycounts.md) | [teamsuseractivitycounts](../resources/teamsuseractivitycounts.md) | アクティビティの種類ごとに、Microsoft Teams アクティビティの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsuseractivityusercounts](../resources/teamsuseractivityusercounts.md) | アクティビティの種類ごとに、ユーザーの数を取得します。 アクティビティの種類は、チーム チャット メッセージ、非公開チャット メッセージ、通話、または会議の数です。 |
