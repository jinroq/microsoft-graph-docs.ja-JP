---
title: メール アプリ使用状況レポート
description: Exchange Online への接続に使用されている電子メールアプリの数を確認できます。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: df40e61108a3933801f5e7c21057f71600b496ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340195"
---
# <a name="email-app-usage-reports"></a>メール アプリ使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exchange Online への接続に使用されている電子メールアプリの数を確認できます。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getemailappusageuserdetail.md) | ストリーム          | [emailapp使い方 userdetail](../resources/emailappusageuserdetail.md) | メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。 |
| [アプリのユーザーの数を取得する](../api/reportroot-getemailappusageappsusercounts.md) | Stream          | [emailapp使い方 appsuser計数](../resources/emailappusageappsusercounts.md) | メール アプリごとの、それぞれ別個のユーザーの数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getemailappusageusercounts.md) | Stream          | [emailapp使い方 user計数](../resources/emailappusageusercounts.md) | 任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。 |
| [バージョンのユーザーの数を取得する](../api/reportroot-getemailappusageversionsusercounts.md) | Stream          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。 |
