---
title: 顧客の支払いを更新する
description: Dynamics 365 Business Central の顧客支払オブジェクトを更新します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: eada35069ab748b93f115ee9639ecb755c19345a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365557"
---
# <a name="update-customerpayments"></a>顧客の支払いを更新する
Dynamics 365 Business Central の customer 支払いオブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 |アクセス許可 (特権の小さいものから大きいものへ)|
|:---------------|:------------------------------------------|
|委任 (職場または学校のアカウント)|Financials.ReadWrite.All |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求

```
PATCH /financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー        |値                    |
|--------------|-------------------------|
|Authorization |ベアラー {トークン}。必須。|
|Content-Type  |application/json         |
|If-Match      |必須です。 この要求ヘッダーが含まれていて、指定された eTag が、**顧客の支払い**の現在のタグと一致しない場合、その**顧客の支払い**は更新されません。    |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された**顧客支払い**オブジェクトを返します。

## <a name="example"></a>例

**要求**

以下は、要求の例です。
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
Content-type: application/json

{
  "amount": 2000
}
```

**応答**

以下は、応答の例です。 

> **注**: ここに示す応答オブジェクトは読みやすいように短縮される場合があります。 実際の呼び出しではすべてのプロパティが返されます。

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "",
  "contactId": "contactId-value",
  "postingDate": "2015-12-31",
  "documentNumber": "D00001",
  "externalDocumentNumber": "",
  "amount": -2000,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

