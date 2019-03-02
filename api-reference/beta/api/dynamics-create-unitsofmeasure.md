---
title: unitsOfMeasure を作成する
description: Dynamics 365 Business Central に測定単位オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a0020ab72ee7bcbbe2b229f209d52bc68691dcb2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365347"
---
# <a name="create-unitsofmeasure"></a>unitsOfMeasure を作成する
Dynamics 365 Business Central の測定単位オブジェクトを作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 |アクセス許可 (特権の小さいものから大きいものへ)|
|:---------------|:------------------------------------------|
|委任 (職場または学校のアカウント)|Financials.ReadWrite.All |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求
```
POST /financials/companies('{id}')/unitsOfMeasure
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|------|-----|
|Authorization  |ベアラー {トークン}。必須。 |
|Content-Type  |application/json   |

## <a name="request-body"></a>要求本文
要求本文で、 **unitsOfMeasure**オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答
成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**unitsOfMeasure**オブジェクトを返します。

## <a name="example"></a>例

**要求**

要求の例を次に示します。

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/unitsOfMeasure
Content-type: application/json

{
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA"
}
```

**応答**

以下は、応答の例です。 

> **注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}

```

