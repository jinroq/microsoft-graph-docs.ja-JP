---
title: Office 365 アクティブ ユーザー レポート
description: 製品ライセンスの数は、個人、組織内で使用されているを確認するのには Office 365 のユーザーのアクティブなレポートを使用し、ユーザーについては、どのような製品を使用している情報にドリルダウンできます。 このレポートは、管理者が使用率の低い製品またはその他のトレーニングや情報が必要なユーザーの識別に役立ちます。
localization_priority: Normal
ms.openlocfilehash: d52588630dcb18a146f34ad66c154e3a64752266
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837157"
---
# <a name="office-365-active-users-reports"></a>Office 365 アクティブ ユーザー レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

製品ライセンスの数は、個人、組織内で使用されているを確認するのには Office 365 のユーザーのアクティブなレポートを使用し、ユーザーについては、どのような製品を使用している情報にドリルダウンできます。 このレポートは、管理者が使用率の低い製品またはその他のトレーニングや情報が必要なユーザーの識別に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: アクティブ ユーザー](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Office 365 アクティブ ユーザーに関する詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | レポート期間中の日ごとのアクティブ ユーザー数を製品別に取得します。 |
| [サービスのユーザーの数を取得する](../api/reportroot-getoffice365servicesusercounts.md) | Stream          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | アクティビティの種類とサービス別のユーザー数を取得します。 |
