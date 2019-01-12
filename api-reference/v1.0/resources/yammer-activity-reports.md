---
title: Yammer アクティビティ レポート
description: Yammer アクティビティ レポートを使用すると、組織全体での生成アクティビティの数と、Yammar でメッセージを投稿、「いいね!」を設定、メッセージを読み取ったそれぞれ別個のユーザーの数を確認することにより、Yammer への組織の関与のレベルを把握することができます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2a97b0d8020a5fce8777d93588e1a38a7ccd8355
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937622"
---
# <a name="yammer-activity-reports"></a>Yammer アクティビティ レポート

Yammer アクティビティ レポートを使用すると、組織全体での生成アクティビティの数と、Yammar でメッセージを投稿、「いいね!」を設定、メッセージを読み取ったそれぞれ別個のユーザーの数を確認することにより、Yammer への組織の関与のレベルを把握することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getyammeractivityuserdetail.md) | Stream      | ユーザー別の Yammer アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getyammeractivitycounts.md) | Stream      | 投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getyammeractivityusercounts.md) | Stream      | Yammer メッセージを投稿、読み取り、および「いいね!」を付けた、それぞれ別個のユーザー数の傾向を取得します。 |
