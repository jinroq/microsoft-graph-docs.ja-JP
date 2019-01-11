---
title: Office 365 アクティブ ユーザー レポート
description: Office 365 アクティブ ユーザー レポートを使用すると、組織内の個人に使用されている製品ライセンスの数を確認し、どのユーザーがどんな製品を使用しているかについて、情報を掘り下げることができます。 これらのレポートによって、管理者は使用率の低い製品や、追加トレーニングや追加情報を必要とする可能性のあるユーザーを特定することができます。
localization_priority: Normal
ms.openlocfilehash: 31707a5cd3f39f443e3da5c6b169261a75b3986e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881474"
---
# <a name="office-365-active-users-reports"></a>Office 365 アクティブ ユーザー レポート

Office 365 アクティブ ユーザー レポートを使用すると、組織内の個人に使用されている製品ライセンスの数を確認し、どのユーザーがどんな製品を使用しているかについて、情報を掘り下げることができます。 これらのレポートによって、管理者は使用率の低い製品や、追加トレーニングや追加情報を必要とする可能性のあるユーザーを特定することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activeuserdetail.md) | Stream      | Office 365 アクティブ ユーザーに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activeusercounts.md) | Stream      | レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。 |
| [サービスのユーザーの数を取得する](../api/reportroot-getoffice365servicesusercounts.md) | Stream      | アクティビティの種類とサービス別のユーザー数を取得します。 |
