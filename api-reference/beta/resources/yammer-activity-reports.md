---
title: Yammer アクティビティ レポート
description: Yammer に組織の活動のレベルを理解するには、組織、Yammer にメッセージを読むの投稿などのおよび一意のユーザー数の間でどの程度の活動が生成されます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 69c155df86cfe772e0c065bec0297a83fb7f3a8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912037"
---
# <a name="yammer-activity-reports"></a>Yammer アクティビティ レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。 21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。

Yammer に組織の活動のレベルを理解するには、組織、Yammer にメッセージを読むの投稿などのおよび一意のユーザー数の間でどの程度の活動が生成されます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | ユーザー別の Yammer アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Yammer メッセージを投稿、読み取り、および「いいね!」を付けた、それぞれ別個のユーザー数の傾向を取得します。 |
