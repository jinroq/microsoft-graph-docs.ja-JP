---
title: Yammer アクティビティ レポート
description: 組織内での活動のレベル、および Yammer でのメッセージの投稿、送受信を行う一意のユーザーの数によって、組織の契約レベルを知ることができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: efdb4ba603be33f18cd66529edd724f6e1a3798d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963831"
---
# <a name="yammer-activity-reports"></a>Yammer アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織内での活動のレベル、および Yammer でのメッセージの投稿、送受信を行う一意のユーザーの数によって、組織の契約レベルを知ることができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer アクティビティ](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | ユーザー別の Yammer アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | 投稿、読み取り、および " いいね!" を付けられたメッセージの数によって、組織内での Yammer アクティビティの量の傾向を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Yammer メッセージを投稿、読み取り、および「いいね!」を付けた、それぞれ別個のユーザー数の傾向を取得します。 |
