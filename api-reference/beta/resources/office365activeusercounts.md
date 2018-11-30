---
title: office365ActiveUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 63d0469f5531d68a7b81c37014103a02e977e870
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069853"
---
# <a name="office365activeusercounts-resource-type"></a>office365ActiveUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 型   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | コンテンツの最新の日付。          |
| office365         | Int64  | Office 365 のアクティブ ユーザーの数です。 この数値には、Exchange、OneDrive、SharePoint、Skype のビジネス、Yammer、およびマイクロソフトのチームで作業中のすべてのユーザーが含まれます。 それぞれのプロパティの説明では、各製品のアクティブなユーザーの定義が表示されます。 |
| 交換          | Int64  | Exchange 内のアクティブ ユーザーの数です。 読み取りし、電子メールを送信できるユーザーは、アクティブなユーザーと見なされます。 |
| oneDrive          | Int64  | OneDrive でアクティブなユーザーの数です。 表示または編集したファイルを内部または外部でファイルを共有またはファイルを同期するユーザーは、アクティブなユーザーと見なされます。 |
| sharePoint        | Int64  | SharePoint でのアクティブ ユーザーの数です。 表示または編集したファイルをファイルを社内で共有または外部で、ファイルを同期または SharePoint ページを表示したすべてのユーザーは、アクティブなユーザーと見なされます。 |
| skypeForBusiness  | Int64  | Skype のビジネスでのアクティブ ユーザーの数です。 整理または会議に参加またはピア ツー ピア セッションに参加しているユーザーは、アクティブなユーザーと見なされます。 |
| yammer            | Int64  | Yammer のアクティブ ユーザーの数です。 投稿、読み取り、またはメッセージのようなユーザーは、アクティブなユーザーと見なされます。 |
| チーム             | Int64  | マイクロソフトのチームで作業中のユーザーの数です。 チームのチャネルでメッセージを投稿、プライベート チャットのセッションにメッセージを送信、または会議や通話に参加したユーザーは、アクティブなユーザーと見なされます。 |
| reportDate        | Date   | 複数のユーザーがアクティブだった日付。 |
| reportPeriod      | String | レポートの対象日数です。    |

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
