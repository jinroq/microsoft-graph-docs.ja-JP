---
title: Microsoft Graph データ接続がサポートするデータセット、地域、シンク
description: Microsoft Graph データ接続で使用できるサポート対象のデータセットと保存先のストレージの種類について説明します。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: fee7daae0af6ee4a1dc3d887e09acd725a37ceb8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629846"
---
# <a name="datasets-regions-and-sinks-that-microsoft-graph-data-connect-supports"></a>Microsoft Graph データ接続がサポートするデータセット、地域、シンク

Microsoft Graph データ接続は、Microsoft Azure でさまざまなデータセット、データ領域、ストレージの場所をサポートしています。 このトピックは、サポートされているデータセット スキーマ、Office 365、Microsoft Azure リージョンへのアクセス方法、Azure Data Factory からデータ接続が利用するストレージの場所について説明します。

その他のデータセット、地域、またはシンクのサポートを要求する場合は、[UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581)でお知らせください。

## <a name="datasets"></a>データセット

データ接続はすぐに次のデータセットをサポートします。 各データセットのスキーマを表示するには、Azure Data Factory の新しいデータセットを作成し、[スキーマ] タブを使って表示します。 

|データセット名|説明|
|-------------|-----------|
|BasicDataSet_v0.Contact_v0|各ユーザーのアドレス帳の連絡先情報が含まれています。 このエンティティのスキーマは「[Microsoft Graph 個人用連絡先スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/contact)」に類似しています。| 
|BasicDataSet_v0.Event_v0|各ユーザーのカレンダーにイベントがあります。 このエンティティのスキーマは「[Microsoft Graph カレンダー イベント](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/event)」に類似しています。| 
|BasicDataSet_v0.Message_v0|各ユーザーのメールボックスにメッセージがあります。 このエンティティのスキーマは「[Microsoft Graph メッセージ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message)」に類似しています。| 
|BasicDataSet_v0.SentItem_v0|各ユーザーのメールボックスから送信されたメッセージがあります。 このエンティティのスキーマは「[Microsoft Graph メッセージ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message)」に類似しています。| 
|BasicDataSet_v0.User_v0|ユーザー情報 (DisplayName、UserPrincipalName など) が含まれています。| 
|BasicDataSet_v0.MailboxSettings_v0|各ユーザーのメールボックスの設定が含まれています。 このエンティティのスキーマは「[Microsoft Graph メールボックス設定スキーマ](https://docs.microsoft.com/en-us/graph/api/resources/mailboxsettings?view=graph-rest-1.0)」に対応しています。| 
|BasicDataSet_v0.MailFolder_v0|各ユーザーのメールボックスのメール フォルダーがあります。 このエンティティのスキーマは「[Microsoft Graph メール フォルダー スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/mailfolder)」に対応しています。|
|BasicDataSet_v0.Manager_v0|各ユーザーのマネージャーのユーザー情報が含まれています。 このエンティティのスキーマは「[Microsoft Graph ユーザー スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user)」に対応しています。|
|BasicDataSet_v0.DirectReport_v0|各ユーザーに直接報告する従業員に関するユーザー情報が含まれています。 このエンティティのスキーマは「[Microsoft Graph ユーザー スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user)」に対応しています。|
|BasicDataSet_v0.CalendarView_v0|イベントがあります。このエンティティのスキーマは「[Microsoft Graph ユーザー スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/events)」に対応しています。|
|BasicDataSet_v0.User_v1|次の表にはユーザーの情報が含まれています。 このエンティティのスキーマは「[Microsoft Graph ユーザー スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/user)」に対応しています。|
|BasicDataSet_v0.Contact_v1|各ユーザーのアドレス帳の連絡先情報が含まれています。 このエンティティのスキーマは「[Microsoft Graph 個人用連絡先スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/contact)」に対応しています。|
|BasicDataSet_v0.Event_v1|各ユーザーのカレンダーにイベントがあります。 このエンティティのスキーマは「[Microsoft Graph カレンダー イベント スキーマ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/event)」に対応しています。|
|BasicDataSet_v0.Message_v1|各ユーザーのメールボックスにメッセージがあります。 このエンティティのスキーマは「[Microsoft Graph メッセージ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message)」に対応しています。|
|BasicDataSet_v0.SentItem_v1|各ユーザーのメールボックスから送信されたメッセージがあります。 このエンティティのスキーマは「[Microsoft Graph メッセージ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/message)」に対応しています。|

## <a name="regions"></a>地域

データ接続は、さまざまな Office 365 地域のデータ抽出をサポートします。 正常に Office 365 データ センターのデータを Microsoft Azure ストレージに移動するには、Azure Data Factory インスタンスと Azure ストレージの場所の両方が、Office 365 データの保管場所のサポートされている領域にマッピングする必要があります。 次の表は、サポートされている Office 365 の領域と、データの移動に必要な対応する Azure リージョンを示しています。 

| Office の地域                    | Azure リージョン                                |
|----------------------------------|---------------------------------------------|
| **北アメリカ**                | 米国東部<br/>米国東部 2<br/>米国中部<br/>米国中央北部<br/>米国中央南部<br/>米国中央西部<br/>米国西部<br/>米国西部 2|
| **ヨーロッパ**                       | 北ヨーロッパ<br/>西ヨーロッパ|
| **アジア太平洋**                 | 東アジア<br/>東南アジア|
| **オーストラリア**                    | オーストラリア東部<br/>オーストラリア南東部|

## <a name="sinks"></a>シンク

シンクは、Azure ストレージにデータを配置するのに使用する出力先の Data Factory です。 データ接続は次のシンク ストレージの種類をサポートしています。

- Azure Data Lake Storage Gen 2
- Azure Storage Blob
- Azure Data Lake Storage Gen 1

次の特徴をシンクに適用します。 

- 出力ファイルは JSON 形式のラインになります。 出力形式が固定されており、出力形式を変更するためのサポートがありません。 ただし、Azure Data Factory を使用して、(Azure SQL DB) などの別のストレージ メカニズムにデータ接続パイプラインの結果をコピーできます。
- サービス プリンシパル認証は、ソースとして Office 365 を使用したコピー アクティビティで、すべてのシンク タイプに対してサポートされている唯一の認証メカニズムです。
- シンクとして Azure Storage Blob を使用している場合、アプリケーションが Azure Storage Blob の場所への Storage Blob Data Contributor のアクセス権があることを確認する必要があります。

## <a name="next-steps"></a>次の手順

Azure Data Factory の一部としてデータ接続パイプラインを作成する方法については、「[Azure Data Factory Office 365 コネクタ ドキュメント](https://docs.microsoft.com/ja-JP/azure/data-factory/connector-office-365)」を参照してください。  
