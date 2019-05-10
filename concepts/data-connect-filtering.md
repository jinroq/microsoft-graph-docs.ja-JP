---
title: ユーザーの選択範囲と Microsoft Graph データ接続サポートのフィルター処理
description: Microsoft Graph データ接続を使用してデータを抽出し、返されたデータをフィルター処理するユーザーの選択方法について説明します。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 1d558c441a626a312d0097d143d194255aaed769
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629839"
---
# <a name="user-selection-and-filtering-microsoft-graph-data-connect-supports"></a>ユーザーの選択範囲と Microsoft Graph データ接続サポートのフィルター処理

Microsoft Graph データ接続を使用して、データを抽出するユーザーを選択し、返されるデータを制限するフィルターを追加できます。 この記事では、データ接続が提供するユーザーの選択範囲オプションと、データ接続がサポートするフィルター処理について説明します。 

## <a name="user-selection"></a>ユーザーの選択範囲 

複数のユーザーにパイプラインを実行できます。 ユーザーの選択範囲オプションは次のとおりです。
- 組織内のすべてのユーザー
- 実行する組織内の最大 10 グループのユーザー 
- Azure Active Directory のユーザー プロパティで構成される述語に基づいたユーザー

Azure Data Factory のコピー アクティビティの SourceDataSet で、ユーザーの選択範囲を指定します。 グループのリストで実行するには、**typeProperties** に新規フィールド **allowedGroups** を追加し、これをコンマで区切った最大 10 グループの**オブジェクト ID** のリストに設定します。 既定でグループが指定されていない場合は、組織全体にデータが抽出されます。 

テナント全体で実行する述語を指定するには、**typeProperties** に新規フィールド **userScopeFilterUri** を追加し、これを述語に設定します。 述語の形式は、Microsoft Graph API のクエリ形式に一致する必要があります。 たとえば、財務部門で働いているユーザーに対して選択範囲を制限する場合は、`https://graph.microsoft.com/v1.0/users?$filter=Department eq 'Finance'`を使用できます。

クエリは、クエリを実行している Office 365 の組織内のユーザーのみを返します。 ゲスト ユーザーとユーザー以外のメールボックスは返されません。

## <a name="filtering"></a>フィルター処理 

DateTime プロパティを使用して、クエリの抽出結果を制限できます。 要求されたデータの種類によっては、DateTime フィルターが必要になる可能性があります。 Azure Data Factory のコピー アクティビティにおける SourceDataSet のプロパティを使用すると、DateTime フィルターが提供されます。 DateTime フィルターを指定するには、**typeProperties** に新規フィールド **dateFilterColumn** を追加して、これを次の表のフィルター処理をサポートするプロパティのいずれかに設定します。 次に、**startTime** と **endTime** を追加します。これは、プロパティがフィルター処理される DateTime の値を表します。 

次のデータセットには、対応する DateTime プロパティのいずれかに指定するフィルターが必要です。

| データセット名                                                   | フィルター処理をサポートしているプロパティ                                           | 
|----------------------------------------------------------------|-----------------------------------------------------------------------------| 
| BasicDataSet_v0.Event_v0<br>BasicDataSet_v0.Event_v1           | CreatedDateTime<br>LastModifiedDateTime                                     | 
| BasicDataSet_v0.Message_v0<br>BasicDataSet_v0.Message_v1       | CreatedDateTime<br>LastModifiedDateTime<br>ReceivedDateTime<br>SentDateTime | 
| BasicDataSet_v0.SentItem_v0<br>BasicDataSet_v0.SentItem_v1     | CreatedDateTime<br>LastModifiedDateTime<br>ReceivedDateTime<br>SentDateTime |

>**注** BasicDataSet_v0.CalendarView_v0 を要求しているパイプラインにも DateTime フィルターが必要ですが、SourceDataSet に **dateFilterColumn** が指定されていません。 ただし、**startTime** と **endTime** が必要で、**startTime** の後に開始し、**endTime** が指定される前に終了するイベントのみです。

## <a name="next-steps"></a>次の手順 

データ接続パイプラインで extractoin とフィルター処理に選択したユーザーの変更方法ついては、「[Azure Data Factory Office 365 コネクタ ドキュメント](https://docs.microsoft.com/ja-JP/azure/data-factory/connector-office-365)」を参照してください。  

  
