---
title: office365ActiveUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bbc51e4859b005c01b0f8d2cfb2db3ca902d60e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581458"
---
# <a name="office365activeusercounts-resource-type"></a>office365ActiveUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportrefreshdate | Date   | コンテンツの最新の日付。          |
| office         | Int64  | Office 365 でアクティブになっているユーザーの数。 この番号には、Exchange、OneDrive、SharePoint、Skype for business、Yammer、Microsoft Teams のすべてのアクティブユーザーが含まれます。 各製品のアクティブユーザーの定義については、それぞれのプロパティの説明を参照してください。 |
| 変換          | Int64  | Exchange 内のアクティブなユーザーの数。 電子メールを読んだり、送信したりできるユーザーは、アクティブなユーザーであると見なされます。 |
| スペース          | Int64  | OneDrive でアクティブになっているユーザーの数。 ファイルを表示または編集したユーザー、内部または外部の共有ファイル、または同期したファイルは、アクティブなユーザーと見なされます。 |
| sharePoint        | Int64  | SharePoint のアクティブなユーザーの数。 ファイルを表示または編集したユーザー、内部または外部の共有ファイル、同期したファイル、または SharePoint ページを表示したユーザーは、アクティブなユーザーであると見なされます。 |
| skypeForBusiness  | Int64  | Skype for business のアクティブなユーザーの数。 電話会議に参加している、またはピアツーピアセッションに参加しているユーザーは、アクティブなユーザーと見なされます。 |
| yammer            | Int64  | Yammer のアクティブユーザーの数。 メッセージを投稿、閲覧、またはそのようにすることができるユーザーは、アクティブなユーザーと見なされます。 |
| teams             | Int64  | Microsoft Teams のアクティブなユーザーの数。 チームチャネルでメッセージを投稿したユーザー、プライベートチャットセッションでメッセージを送信したユーザー、または会議または通話に参加したユーザーは、アクティブなユーザーであると見なされます。 |
| reportDate        | Date   | ユーザー数がアクティブであった日付。 |
| reportperiod      | String | レポートの対象となる日数を指定します。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
