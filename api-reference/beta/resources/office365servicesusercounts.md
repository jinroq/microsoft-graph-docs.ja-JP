---
title: office365ServicesUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 975a70b040ac5886ea36219a5407f580a42aeadc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067407"
---
# <a name="office365servicesusercounts-resource-type"></a>office365ServicesUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                 | 型   | 説明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Date   | コンテンツの最新の日付。          |
| exchangeActive           | Int64  | Exchange 上のアクティブ ユーザーの数です。 読み取りし、電子メールを送信できるユーザーは、アクティブなユーザーと見なされます。 |
| exchangeInactive         | Int64  | Exchange 上のアクティブでないユーザーの数です。 |
| oneDriveActive           | Int64  | OneDrive のアクティブなユーザーの数です。 表示または編集したファイルを内部または外部でファイルを共有またはファイルを同期するユーザーは、アクティブなユーザーと見なされます。 |
| oneDriveInactive         | Int64  | OneDrive 上のアクティブでないユーザーの数です。 |
| sharePointActive         | Int64  | SharePoint のアクティブなユーザーの数です。 表示または編集したファイルをファイルを社内で共有または外部で、ファイルを同期または SharePoint ページを表示したすべてのユーザーは、アクティブなユーザーと見なされます。 |
| sharePointInactive       | Int64  | SharePoint でアクティブでないユーザーの数です。 |
| skypeForBusinessActive   | Int64  | Skype のビジネス上のアクティブ ユーザーの数です。 整理または会議に参加またはピア ツー ピア セッションに参加しているユーザーは、アクティブなユーザーと見なされます。 |
| skypeForBusinessInactive | Int64  | Skype のビジネス上のアクティブでないユーザーの数です。 |
| yammerActive             | Int64  | Yammer のアクティブなユーザーの数です。 投稿、読み取り、またはメッセージのようなユーザーは、アクティブなユーザーと見なされます。 |
| yammerInactive           | Int64  | Yammer にアクティブでないユーザーの数です。  |
| teamsActive              | Int64  | チームのアクティブなユーザーの数です。 チームのチャネルでメッセージを投稿、プライベート チャットのセッションにメッセージを送信、または会議や通話に参加したユーザーは、アクティブなユーザーと見なされます。 |
| teamsInactive            | Int64  | チームのアクティブなユーザーの数です。     |
| reportPeriod             | String | レポートの対象日数です。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "reportPeriod": "String"
}
```