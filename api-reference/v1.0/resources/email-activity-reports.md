---
title: 電子メール アクティビティ レポート
description: 電子メール アクティビティ レポートを使用して、組織内の電子メール トラフィックの詳細ビューを取得します。 [メール アクティビティ] ウィジェットに進み、組織内のユーザーごとの電子メール アクティビティの傾向と詳細を把握することもできます。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: e28e968a536b4025094ba0376973352f7d9cc949
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981785"
---
# <a name="email-activity-reports"></a>電子メール アクティビティ レポート

電子メール アクティビティ レポートを使用して、組織内の電子メール トラフィックの詳細ビューを取得します。 [メール アクティビティ] ウィジェットに進み、組織内のユーザーごとの電子メール アクティビティの傾向と詳細を把握することもできます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: 電子メール アクティビティ](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getemailactivityuserdetail.md) | Stream      | ユーザーが実行した電子メール アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getemailactivitycounts.md) | Stream      | 組織内の電子メール アクティビティ (送信、読み取り、受信の数) の傾向を把握できます。 |
| [ユーザーの数を取得する](../api/reportroot-getemailactivityusercounts.md) | Stream      | 送信、読み取り、受信などの電子メール アクティビティを実行しているそれぞれ別個のユーザーの数に関する傾向を把握することができます。 |
