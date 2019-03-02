---
title: 顧客の支払いリソースの種類
description: Dynamics 365 Business Central の顧客の支払いオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365613"
---
# <a name="customerpayments-resource-type"></a>顧客の支払いリソースの種類
Dynamics 365 Business Central の顧客の支払いを表します。 顧客支払は、顧客の支払仕訳帳に明細行として入力されます。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型  |説明|
|:---------------|:-------------|:----------|
|[顧客の支払いを取得する](../api/dynamics-customerpayment-get.md)|顧客の支払い|顧客支払を取得します。|
|[顧客の支払いを投稿する](../api/dynamics-create-customerpayment.md)|顧客の支払い|顧客の支払いを作成します。|
|[更新プログラムの顧客の支払い](../api/dynamics-customerpayment-update.md)|顧客の支払い|顧客の支払いを更新します。|
|[顧客の支払いを削除する](../api/dynamics-customerpayment-delete.md)|none|顧客の支払を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型    |説明|
|:-------------|:--------|:----------|
|ID|GUID|顧客の支払の一意の ID。 編集不可。|
|journalDisplayName|string|支払いレコードが行である顧客支払仕訳帳。|
|lineNumber|integer|顧客の支払回数。|
|customerId|GUID|支払いが関連付けられている顧客の一意の ID。|
|顧客番号|文字列、最大サイズ20|支払いが関連付けられている顧客の番号。|
|contactId|文字列、最大サイズ250|指定された顧客の exchange 連絡先 id。 顧客 id が指定されていない場合は、連絡先 id を使用して検索します。|
|postingdate|日付|顧客の支払が転記される日付。|
|documentnumber|文字列、最大サイズ20|顧客支払のドキュメント番号を指定します。|
|externaldocumentnumber|文字列、最大サイズ20|顧客支払の外部ドキュメント番号を指定します。|
|値|decimal|顧客の支払を構成する合計金額 (VAT を含む) を指定します。|
|appliesToInvoiceId|GUID|支払が関連付けられている請求書の一意の ID。|
|appliesToInvoiceNumber|文字列、最大サイズ20|支払が関連付けられている請求書の番号。|
|説明|文字列、最大サイズ50|ユーザーまたは autocreated によって提供される顧客の支払いの説明。|
|コメント|文字列、最大サイズ250|顧客支払に対してユーザーが指定したコメント。|
|lastModifiedDateTime|datetime|顧客の支払が最後に変更された日時。 読み取り専用です。|


## <a name="relationships"></a>リレーションシップ
顧客支払は、顧客の支払仕訳帳のサブページです。 直接アクセスすることはできません。

顧客支払は、寸法線の "親エンティティ" にすることができます。

Customers テーブルに Customer (customerId) が存在している必要があります。

請求書 (appliesToInvoiceId) は、[売上請求書] テーブルに存在する必要があります。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

