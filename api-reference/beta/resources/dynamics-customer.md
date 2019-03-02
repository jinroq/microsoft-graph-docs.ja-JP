---
title: customers リソースの種類
description: Dynamics 365 Business Central の顧客を表します。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e4daa28018001fb6cb6e4866bedf8e256a72abef
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365935"
---
# <a name="customers-resource-type"></a>customers リソースの種類
Dynamics 365 Business Central の顧客を表します。

## <a name="methods"></a>メソッド

| メソッド                                              |戻り値の型| 説明      |
|:----------------------------------------------------|:----------|:-----------------|
|[顧客を取得する](../api/dynamics-customer-get.md)      |ユーザー   |顧客を取得します。   |
|[顧客を作成する](../api/dynamics-create-customer.md)|ユーザー   |顧客を作成します。|
|[顧客を更新する](../api/dynamics-customer-update.md)|ユーザー   |顧客を更新します。|
|[顧客を削除する](../api/dynamics-customer-delete.md)|none        |顧客を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ    | 型     |説明|
|:------------|:---------|:----------|
|ID           |GUID      |アイテムの一意の ID です。 編集不可。|
|number       |string    |顧客番号。|
|displayName  |string    |顧客の名前を指定します。 この名前は、顧客のすべての販売ドキュメントに表示されます。|
|type         |文字列    |顧客の種類として、"Company" または "Person" を指定します。|
|address      |[ナビゲーション."postaladdress](../resources/dynamics-complextypes.md)|顧客の住所を指定します。 この住所は、お客様のすべてのセールスドキュメントに表示されます。|
|phoneNumber  |string    |顧客の電話番号を指定します。|
|email        |string    |顧客の電子メールアドレスを指定します。|
|Web サイト      |string    |顧客のホームページのアドレスを指定します。|
|taxLiable    |ブール値   |顧客または仕入先が売上税に対して責任を負わないかどうかを指定します。 お客様が納税責任を持つ場合は**true**に設定します。|
|taxAreaId    |GUID      |顧客が属する税エリアを指定します。|
|taxAreaDisplayName|string|顧客が属する税エリアの表示名を指定します。|
|taxRegistrationNumber|文字列、最大サイズ20|顧客の税務登録番号を指定します。|
|currencyId   |GUID      |顧客が使用する通貨を指定します。|
|currencyCode |numeric   |顧客の既定の通貨コード。|
|paymentTermsId|GUID     |顧客が使用する支払い条件を指定します。|
|paymentMethodId|GUID    |顧客が使用する支払い方法を指定します。|
|shipmentMethodId|GUID   |顧客がどの送付方法を使用するかを指定します。|
|ブロック      |string    |顧客とのトランザクションを転記できないことを指定します。 顧客がブロックされていない場合は、[**すべて**] に設定します。ブロックしない場合は、[空白] に設定します。|
|対照      |numeric   |顧客が完了した売上に対して支払うべき支払い金額を指定します。 この値は、顧客の残高とも呼ばれます。 読み取り専用です。|
|overdueAmount|numeric   |顧客の延滞金額を指定します。|
|totalSalesExcludingTax|numeric|顧客の税を除いた合計売上金額を指定します。|
|lastModifiedDateTime|datetime|顧客が最後に変更された日付です。 読み取り専用です。|  


## <a name="relationships"></a>リレーションシップ
通貨 (currencyCode) は、[通貨] テーブルに存在している必要があります。

支払い条件 (paymentTerms) は支払い条件テーブルに存在する必要があります。

送付方法 (shipmentMethod) は、送付方法テーブルに存在する必要があります。

支払い方法 ([cash]) は支払い方法テーブルに存在する必要があります。

税エリア (taxArea) は、税エリアテーブルに存在する必要があります。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```

