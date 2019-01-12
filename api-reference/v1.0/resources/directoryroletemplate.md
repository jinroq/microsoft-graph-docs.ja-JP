---
title: directoryRoleTemplate リソース型
description: 'ディレクトリの役割のテンプレートを表します。 ロール テンプレート ディレクトリは、ディレクトリの役割 (directoryRole) のプロパティ値を指定します。 テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 POST 要求を送信するその他の利用可能なディレクトリの役割を有効にするのには、`/directoryRoles`の要求の**roleTemplateId**パラメーターで指定されたディレクトリの役割の基になるディレクトリ ロール テンプレートの ID を持つエンドポイントです。 この要求の完了時に読み取りとディレクトリのロールにメンバーを割り当てるし、開始できます。 **注**: このロールに、ユーザー ディレクトリのディレクトリの役割のテンプレートが公開されています。 ユーザー ディレクトリの役割は、暗黙の型がクライアントのディレクトリに表示されていません。 テナントのすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。 ロールが既にアクティブになっています。 このテンプレートを使用しません。'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 57dec43699ba75c7e936fa02dbdf09df74dd06ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966994"
---
# <a name="directoryroletemplate-resource-type"></a>directoryRoleTemplate リソース型

ディレクトリ ロール テンプレートを表します。ディレクトリ ロール テンプレートでは、ディレクトリ ロール ([directoryRole](directoryrole.md)) のプロパティ値を指定します。テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、ディレクトリ ロール テンプレートの ID を使用して `/directoryRoles` エンドポイントに POST 要求を送信します。この ID は、要求の **roleTemplateId** パラメーターで指定したディレクトリ ロールに基づきます。この要求が正常に完了すると、ディレクトリ ロールの読み取りや、ディレクトリ ロールへのメンバーの追加ができるようになります。**注**:ディレクトリ ロール テンプレートは、ユーザー (Users) ディレクトリ ロールに公開されます。ユーザー ディレクトリ ロールは、暗黙的であり、ディレクトリ クライアントには表示されません。テナント内のすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。このロールは、あらかじめアクティブ化されています。このテンプレートは、使用しないでください。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Get directoryRoleTemplate](../api/directoryroletemplate-get.md) | [directoryRoleTemplate](directoryroletemplate.md) |directoryRoleTemplate オブジェクトのプロパティとリレーションシップを読み取ります。|
|[directoryRoleTemplate を一覧表示する](../api/directoryroletemplate-list.md) | [directoryRoleTemplate](directoryroletemplate.md) コレクション |directoryRoleTemplate オブジェクトのリストを取得します|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|説明|String|ディレクトリ ロールに設定する説明。読み取り専用。|
|displayName|String|ディレクトリ ロールに設定する表示名。読み取り専用。 |
|id|String|テンプレートの一意識別子。[directoryObject](directoryobject.md) から継承されます。POST 要求の **roleTemplateId** プロパティにディレクトリ ロール テンプレートの **id** を指定して、テナントの [directoryRole](directoryrole.md) をアクティブ化します。キーであり、Null は許容されません。読み取り専用。|

## <a name="relationships"></a>リレーションシップ
なし



## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
