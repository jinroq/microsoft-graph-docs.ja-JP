---
title: Skype for Business ピア ツー ピア アクティビティ レポート
description: Skype for Business ピア ツー ピア アクティビティ レポートを使用して、組織全体のピア ツー ピア アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 6c94b4fd09fb71af3c264664eaa0182256dfa949
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920731"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Skype for Business ピア ツー ピア アクティビティ レポート

Skype for Business ピア ツー ピア アクティビティ レポートを使用して、組織全体のピア ツー ピア アクティビティの詳細を取得できます。 これらの詳細は、組織のための調査、計画、その他のビジネスの意思決定の際に非常に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Skype for Business ピア ツー ピア アクティビティ](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [アクティビティの数を取得する](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Stream      | 組織内で実施されたセッションの数と種類について、使用傾向を取得します。 セッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。 |
| [ユーザーの数を取得する](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Stream      | 組織内で実施されたピア ツー ピア セッションの一意のユーザー数と種類について、使用傾向を取得します。 ピア ツー ピア セッションでのセッションの種類には IM、オーディオ、ビデオ、アプリケーション共有、ファイル転送があります。 |
| [時間 (分) を取得する](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Stream      | 組織内で実施されたピア ツー ピア セッションの長さ (分数) と種類についての使用傾向を取得します。 セッションの種類には、オーディオとビデオが含まれます。 |

