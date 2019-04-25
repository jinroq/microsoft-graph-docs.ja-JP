---
title: Skype for Business アクティビティ レポート
description: Skype for Business アクティビティ レポートを使用して、組織全体のアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a98e74c1c94f1b94046aea0a5b2964d47f55595b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552782"
---
# <a name="skype-for-business-activity-reports"></a>Skype for Business アクティビティ レポート

Skype for Business アクティビティ レポートを使用して、組織全体のアクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business アクティビティ](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream      | ユーザー別の Skype for Business アクティビティに関する詳細を取得します。 |
| [アクティビティの数を取得する](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream      | Skype for Business を介して組織内で行われた会議セッションの開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。 |
| [ユーザーの数を取得する](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream      | Skype for Business を介して組織内で行われた会議セッションにおける、それぞれ別個の開催ユーザー数と参加ユーザー数の傾向を取得します。 レポートには、ピア ツー ピア セッションの数も含まれます。 |
