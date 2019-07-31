---
title: CustomerPaymentJournals を作成する
description: Dynamics 365 Business Central に顧客の支払仕訳帳オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 3f1bcae115bd1d5e9c117b6bc90981402397ab0e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956696"
---
# <a name="create-customerpaymentjournals"></a>CustomerPaymentJournals を作成する
Dynamics 365 Business Central に顧客支払仕訳帳オブジェクトを作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 |アクセス許可 (特権の小さいものから大きいものへ)|
|:---------------|:------------------------------------------|
|委任 (職場または学校のアカウント)|Financials.ReadWrite.All |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求

```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー        |値                    |
|--------------|-------------------------|
|Authorization |ベアラー {トークン}。必須。|
|Content-Type  |application/json         |

## <a name="request-body"></a>要求本文
要求本文で、 **customerPaymentJournals**オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答
成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**customerPaymentJournals**オブジェクトを返します。

## <a name="example"></a>例

**要求**

要求の例を次に示します。

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

**応答**

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


