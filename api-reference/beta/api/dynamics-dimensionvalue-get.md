---
title: dimensionvalues の値を取得する
description: Dynamics 365 Business Central の分析コード値オブジェクトを取得します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ad8d9f26faa4fcc2f03f2da04c073857bcfd152f
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365725"
---
# <a name="get-dimensionvalues"></a>dimensionvalues の値を取得する
Dynamics 365 Business Central の分析コード値オブジェクトのプロパティとリレーションシップを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 |アクセス許可 (特権の小さいものから大きいものへ)|
|:---------------|:------------------------------------------|
|委任 (職場または学校のアカウント)|Financials.ReadWrite.All |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求

```
GET /financials/companies('{id}')/dimensions('{id}')/dimensionValues('{id}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー       |値                     |
|-------------|--------------------------|
|Authorization|ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で**dimensionvalues**オブジェクトを返します。

## <a name="example"></a>例

**要求**

以下は、要求の例です。
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/dimensions('{id}')/dimensionValues('{id}')
```

**応答**

以下は、応答の例です。 

> **注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。

```json
{
  "id": "id-value",
  "code": "30",
  "displayName": "Europe North (EU)",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

