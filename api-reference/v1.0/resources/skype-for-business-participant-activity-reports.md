---
title: Skype for Business 参加者アクティビティ レポート
description: Skype for Business 参加者アクティビティ レポートを使用して、組織全体の参加者アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.openlocfilehash: 05e0ffb222696f66e9c1a4fce49c01076805d893
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847832"
---
# <a name="skype-for-business-participant-activity-reports"></a>Skype for Business 参加者アクティビティ レポート

Skype for Business 参加者アクティビティ レポートを使用して、組織全体の参加者アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business 電話会議の参加者のアクティビティ](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [アクティビティの数を取得する](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream      | 組織からユーザーが参加した会議セッションの数と種類ついて、使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。 |
| [ユーザーの数を取得する](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream      | 組織からユーザーが参加したそれぞれ別個のユーザーの数と会議セッションの種類について、使用傾向を取得します。 会議セッションの種類には、IM、オーディオ/ビデオ、アプリケーション共有、Web、サードパーティへのダイヤルイン/ダイヤルアウトなどがあります。 |
| [時間 (分) を取得する](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Stream      | 組織からユーザーが参加した会議セッションの長さ (分) と種類について、使用傾向を取得します。 会議セッションの種類には、オーディオ/ビデオがあります。 |
