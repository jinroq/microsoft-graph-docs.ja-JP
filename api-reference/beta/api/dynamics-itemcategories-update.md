---
title: ItemCategories の更新
description: Dynamics 365 Business Central のアイテムカテゴリを更新します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: a44da57af784d0506392090e06a0851887499f34
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956192"
---
# <a name="update-itemcategories"></a>ItemCategories の更新
Dynamics 365 Business Central のアイテムカテゴリオブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 |アクセス許可 (特権の小さいものから大きいものへ)|
|:---------------|:------------------------------------------|
|委任 (職場または学校のアカウント)|Financials.ReadWrite.All |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求

```
PATCH /financials/companies('{id}')/itemCategories('{id}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー       |値                    |
|-------------|-------------------------|
|Authorization|ベアラー {トークン}。必須。|
|Content-Type |application/json         |
|If-Match     |必須です。 この要求ヘッダーが含まれていて、指定された eTag が**Itemcategories**の現在のタグと一致しない場合、 **itemcategories**は更新されません。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された**itemcategories**オブジェクトを返します。

## <a name="example"></a>例

**要求**

以下は、要求の例です。
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories('{id}')
Content-type: application/json

{
  "displayName": "Office Chair - swivel"
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
  "code": "CHAIR",
  "displayName": "Office Chair - swivel",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}
```
