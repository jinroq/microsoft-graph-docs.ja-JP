---
title: Microsoft Graph API を使用する
description: Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。アプリを登録 して、サービス または ユーザーの認証トークンを取得する と、Microsoft Graph API に対して要求を行うことができます。
author: jackson-woods
localization_priority: Priority
scenarios: getting-started
ms.openlocfilehash: f022795a9777c463ac9394a1781ea3585fe08371
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792563"
---
# <a name="use-the-microsoft-graph-api"></a>Microsoft Graph API を使用する

Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。[アプリを登録](auth-register-app-v2.md) して、[サービス](auth-v2-service.md) または [ユーザーの認証トークンを取得する](auth-v2-user.md) と、Microsoft Graph API に対して要求を行うことができます。

> **重要:** 条件付きアクセス ポリシーの Microsoft Graph への適用方法は変更されています。 条件付きアクセス ポリシーが構成されるシナリオを処理するよう、アプリケーションを更新する必要があります。 詳細およびガイダンスについては、「[Azure Active Directory の条件付きアクセスについての開発者ガイド](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)」を参照してください。

ユーザーや電子メール メッセージなど、リソースの読み取りや書き込みを行うには、次のような要求を構築します。

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

要求のコンポーネントには以下が含まれます。

* [{HTTP メソッド}](#http-methods) - Microsoft Graph への要求で使用する HTTP メソッド。
* [{バージョン}](#version) - アプリケーションが使用している Microsoft Graph API のバージョン。
* [{リソース}](#resource) - ユーザーが参照している Microsoft Graph のリソース。 
* [{クエリ パラメーター}](#query-parameters) - 応答をカスタマイズするために使用する省略可能な OData クエリ オプションまたは REST メソッド パラメーター。

要求を行うと、次を含む応答が返されます。 

* 状態コード - 成功または失敗を示す HTTP 状態コード。HTTP エラー コードの詳細については、「[エラー](errors.md)」を参照してください。
* 応答メッセージ - 要求したデータ、または操作の結果。応答メッセージは、いくつかの操作で空になる場合があります。
* `nextLink` - 要求が大量のデータを返す場合は、`@odata.nextLink` で返される URL を使用して応答をページングする必要があります。詳細については、「[ページング](paging.md)」を参照してください。

## <a name="http-methods"></a>HTTP メソッド

Microsoft Graph は、要求で HTTP メソッドを使用し、要求が何を行っているかを特定します。API は次のメソッドをサポートしています。


|**メソッド** |**説明**                             |
| :----- | :------------------------------------------- |
| GET    | リソースからデータを読み取ります。                   |
| POST   | 新しいリソースを作成、または処理を実行します。 |
| PATCH  | リソースを新しい値で更新します。           |
| PUT    | リソースを新しいものと置換します。           |
| DELETE | リソースを削除します。                           |

* CRUD メソッドの `GET` と `DELETE` では、要求本文は必要ありません。
* `POST`、`PATCH`、および `PUT` メソッドは、通常 JSON 形式で指定されている要求本文を必要とし、それには、リソースのプロパティの値などの追加の情報が含まれます。

## <a name="version"></a>バージョン

Microsoft Graph は、現在 `v1.0` と `beta` の 2 つのバージョンをサポートしています。

* `v1.0` には、一般公開されている API が含まれます。すべての運用アプリで、v1.0 バージョンを使用します。
* `beta` には、現在プレビュー段階の API が含まれます。ベータ版 API に重大な変更を導入する可能性があるため、開発中のアプリのテストにのみ、ベータ版を使用することをお勧めします。運用アプリでは、ベータ版 API を使用しないでください。

ベータ版 API のフィードバックを常に募集しています。フィードバックの提供または機能のご要望は、「[UserVoice](https://officespdev.uservoice.com/)」ページを参照してください。

API のバージョンに関する詳細については、「[バージョン管理とサポート](versioning-and-support.md)」を参照してください。

## <a name="resource"></a>リソース

リソースには、エンティティまたは複合型が使用でき、一般的にプロパティを使用して定義されます。 エンティティは、常に "**id**" プロパティが含まれる点において、複合型とは異なります。

ユーザーの URL には、要求で操作するリソースが含まれます。たとえば、`me`、**user**、**group**、**drive**、**site** などです。 多くの場合、最上位のリソースには _リレーションシップ_も含まれます。`me/messages` または `me/drive` のように、追加のリソースにアクセスするのに使用できます。 _メソッド_を使用して、リソースを操作することもできます。たとえば、電子メールを送信するには `me/sendMail` を使用します。 詳細については、「[Microsoft Graph 内を移動してデータとメソッドにアクセスする](traverse-the-graph.md)」を参照してください。

各リソースにアクセスするために異なるアクセス許可が必要になる可能性があります。リソースの作成または更新には、リソースの読み取りよりも高いレベルのアクセス許可が必要になります。必要なアクセス許可に関する詳細については、メソッドの参照トピックを参照してください。 

アクセス許可に関する詳細については、「[アクセス許可の参照](permissions-reference.md)」を参照してください。

## <a name="query-parameters"></a>クエリ パラメーター

クエリ パラメーターには、OData のシステム クエリ オプション、または応答をカスタマイズするためにメソッドが受け入れる文字列を使用できます。

省略可能の OData のシステム クエリ オプションを使用すると、既定の応答よりも多い、または少ないプロパティを含めたり、カスタム クエリに一致するアイテムについて応答をフィルター処理したり、メソッドの追加のパラメーターを提供したりできます。

たとえば、次の `filter` パラメーターを追加すると、`jon@contoso.com` の `emailAddress` プロパティを持つメッセージのみが返されるように制限できます。

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

OData クエリ オプションの詳細については、「[Use query parameters to customize responses (クエリパラメーターを使用して応答をカスタマイズする)](query-parameters.md)」を参照してください。

OData クエリ オプション以外に、一部のメソッドでは、クエリ URL の一部としてパラメーター値を指定することが要求されます。 たとえば、ある一定期間内にユーザーの予定表で発生したイベントのコレクションを取得するには、クエリ パラメーターとして `startDateTime` と `endDateTime` の値を使用して期間を指定し、**user** の **calendarView** リレーションシップに対してクエリを実行します。

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="next-steps"></a>次のステップ

Microsoft Graph を使用して、起動および実行する準備ができました。詳細について知るには、[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)に移動して、いくつかの要求や[クイック スタート](https://developer.microsoft.com/graph/quick-start)を試したり、「[SDK とコード サンプル](https://developer.microsoft.com/graph/code-samples-and-sdks)」のいずれかを使用して開始したりします。
