---
title: Skype for Business 開催者アクティビティ レポート
description: 組織全体にわたって体系化された会議の活動の詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.openlocfilehash: 7145245d7524c068df19bf6bcdcb49bff138f182
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810074"
---
# <a name="skype-for-business-organizer-activity-reports"></a>Skype for Business 開催者アクティビティ レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

組織全体にわたって体系化された会議の活動の詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の開催者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [アクティビティの数を取得する](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | Stream          | [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) | 組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用状況の傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。 |
| [ユーザーの数を取得する](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | Stream          | [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) | 一意のユーザー数と組織内のユーザーが開催、企画した電話会議セッションの数と種類に関する使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サード パーティへのダイヤルイン/ダイヤルアウト、Microsoft へのダイヤルイン/ダイヤルアウトなどがあります。 |
| [時間 (分) を取得する](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | Stream          | [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) | 組織内のユーザーが開催、企画した電話会議セッションの長さ (分数) と種類に関する使用状況の傾向を取得します。 電話会議セッションの種類には、オーディオ/ビデオ、および Microsoft へのダイヤルインとダイヤルアウトがあります。 |
