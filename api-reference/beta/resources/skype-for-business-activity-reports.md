---
title: Skype for Business アクティビティ レポート
description: 組織全体でのアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fae59f7b4053a6a57df4869da165aca023c53071
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342868"
---
# <a name="skype-for-business-activity-reports"></a>Skype for Business アクティビティ レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織全体でのアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeforbusinessactivityuserdetail](../resources/skypeforbusinessactivityuserdetail.md) | ユーザー別の Skype for Business アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [skypeforbusinessactivitycounts](../resources/skypeforbusinessactivitycounts.md) | Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。 |
| [ユーザーの数を取得する](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [skypeforbusinessactivityusercounts](../resources/skypeforbusinessactivityusercounts.md) | Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。 |
