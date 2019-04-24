---
title: journalLines を作成する
description: Dynamics 365 Business Central の仕訳帳明細行を作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c6ed8b1ccbe1f33cad174e1c5e4f9b3832f2a5c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463580"
---
# <a name="create-journallines"></a>journalLines を作成する
Dynamics 365 Business Central に、ジャーナル明細行オブジェクトを作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 |アクセス許可 (特権の小さいものから大きいものへ)|
|:---------------|:------------------------------------------|
|委任 (職場または学校のアカウント)|Financials.ReadWrite.All |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求

```
POST /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー        |値                    |
|--------------|-------------------------|
|Authorization |ベアラー {トークン}。必須。|
|Content-Type  |application/json         |

## <a name="request-body"></a>要求本文
要求本文で、 **journalLines**オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答
成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**journalLines**オブジェクトを返します。

## <a name="example"></a>例

**要求**

要求の例を次に示します。

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines
Content-type: application/json

{
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": ""
}
```
**応答**

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```


