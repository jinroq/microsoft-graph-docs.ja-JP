---
title: 仕入先の削除
description: Dynamics 365 Business Central のベンダーオブジェクトを削除します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e9ef641d8c1d6995e93eaaf87a7131e246c9a0f9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365893"
---
# <a name="delete-vendors"></a>仕入先の削除
Dynamics 365 Business Central からベンダーオブジェクトを削除します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類 |アクセス許可 (特権の小さいものから大きいものへ)|
|:---------------|:------------------------------------------|
|委任 (職場または学校のアカウント)|Financials.ReadWrite.All |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求
```
DELETE /financials/companies('{id}')/vendors('{id}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|------|-----|
|Authorization  |ベアラー {トークン}。必須。 |
|If-Match       |必須です。 この要求ヘッダーが含まれており、指定された eTag が**ベンダー**の現在のタグと一致しない場合、**ベンダー**は更新されません。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは ```204 No Content``` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例

**要求**

以下は、要求の例です。

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/vendors('{id}')
```

**応答** 

以下は、応答の例です。 

```json
HTTP/1.1 204 No Content
```