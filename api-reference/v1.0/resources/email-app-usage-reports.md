---
title: メール アプリ使用状況レポート
description: メール アプリの使用状況レポートを使用して、Exchange Online に接続するために使用されたメール アプリの数を確認します。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
ms.openlocfilehash: 3288d987719dd7ba005b0c6bb23231e367b2ad37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869987"
---
# <a name="email-app-usage-reports"></a>メール アプリ使用状況レポート

メール アプリの使用状況レポートを使用して、Exchange Online に接続するために使用されたメール アプリの数を確認します。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getemailappusageuserdetail.md) | Stream      | メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。 |
| [アプリのユーザーの数を取得する](../api/reportroot-getemailappusageappsusercounts.md) | Stream      | メール アプリごとの、それぞれ別個のユーザーの数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getemailappusageusercounts.md) | Stream      | 任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。 |
| [バージョンのユーザーの数を取得する](../api/reportroot-getemailappusageversionsusercounts.md) | Stream      | Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。 |
