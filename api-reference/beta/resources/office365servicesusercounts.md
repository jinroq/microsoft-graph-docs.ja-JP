---
title: office365ServicesUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 5958ab3cb05767465b0866078d378208f1b466e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009469"
---
# <a name="office365servicesusercounts-resource-type"></a>office365ServicesUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                 | 型   | 説明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日付   | コンテンツの最新の日付。          |
| exchangeActive           | Int64  | Exchange 上のアクティブなユーザーの数。 電子メールを読んだり、送信したりできるユーザーは、アクティブなユーザーであると見なされます。 |
| exchangeInactive         | Int64  | Exchange 上の非アクティブなユーザーの数。 |
| Onedrive Active           | Int64  | OneDrive 上のアクティブなユーザーの数。 ファイルを表示または編集したユーザー、内部または外部の共有ファイル、または同期したファイルは、アクティブなユーザーと見なされます。 |
| Onedrive 非アクティブ         | Int64  | OneDrive 上の非アクティブなユーザーの数。 |
| sharePointActive         | Int64  | SharePoint 上のアクティブなユーザーの数。 ファイルを表示または編集したユーザー、内部または外部の共有ファイル、同期したファイル、または SharePoint ページを表示したユーザーは、アクティブなユーザーであると見なされます。 |
| sharePointInactive       | Int64  | SharePoint 上の非アクティブなユーザーの数。 |
| skypeForBusinessActive   | Int64  | Skype For Business 上のアクティブなユーザーの数。 電話会議に参加している、またはピアツーピアセッションに参加しているユーザーは、アクティブなユーザーと見なされます。 |
| skypeForBusinessInactive | Int64  | Skype For Business で使用されていないユーザーの数。 |
| yammerActive             | Int64  | Yammer のアクティブなユーザーの数。 メッセージを投稿、閲覧、またはそのようにすることができるユーザーは、アクティブなユーザーと見なされます。 |
| yammerInactive           | Int64  | Yammer の非アクティブユーザーの数。  |
| teamsActive              | Int64  | Microsoft Teams のアクティブなユーザーの数。 チームチャネルでメッセージを投稿したユーザー、プライベートチャットセッションでメッセージを送信したユーザー、または会議または通話に参加したユーザーは、アクティブなユーザーであると見なされます。 |
| teamsInactive            | Int64  | Microsoft Teams の非アクティブなユーザーの数。     |
| office365Active          | Int64  | Office 365 上のアクティブユーザーの数。   |
| office365Inactive        | Int64  | Office 365 の非アクティブなユーザーの数。     |
| reportPeriod             | String | レポートの対象となる日数を指定します。    |

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
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
