---
title: SharePoint アクティビティ レポート
description: ファイルとの相互作用を参照して、SharePoint を使用するライセンスを保有するすべてのユーザーの利用状況を取得できます。 共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。
ms.openlocfilehash: fd516b5ca56f8625c98fce943cafc90b32346416
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073319"
---
# <a name="sharepoint-activity-reports"></a>SharePoint アクティビティ レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ファイルとの相互作用を参照して、SharePoint を使用するライセンスを保有するすべてのユーザーの利用状況を取得できます。 共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getsharepointactivityuserdetail.md) | Stream          | [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) | ユーザー別の SharePoint アクティビティに関する詳細を取得します。 |
| [ファイルの数を取得する](../api/reportroot-getsharepointactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getsharepointactivityusercounts.md) | Stream          | [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) | アクティブ ユーザーの数の傾向を取得します。 ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。 |
| [ページを取得する](../api/reportroot-getsharepointactivitypages.md) | Stream          | [sharePointActivityPages](../resources/sharepointactivitypages.md) | ユーザーがアクセスしたそれぞれ別個のページ数を取得します。 |
