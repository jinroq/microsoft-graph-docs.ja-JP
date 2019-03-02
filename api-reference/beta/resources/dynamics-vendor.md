---
title: ベンダーリソースの種類
description: Dynamics 365 Business Central のベンダーオブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365662"
---
# <a name="vendors-resource-type"></a>ベンダーリソースの種類
Dynamics 365 Business Central のベンダーを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ベンダーを取得する](../api/dynamics-vendor-get.md)|主要|ベンダーオブジェクトを取得します。|
|[ベンダーを投稿する](../api/dynamics-create-vendor.md)|主要|ベンダーオブジェクトを作成します。|
|[パッチベンダー](../api/dynamics-vendor-update.md)|主要|ベンダーオブジェクトを更新します。|
|[ベンダーの削除](../api/dynamics-vendor-delete.md)|none|ベンダーオブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ID|GUID|ベンダーの一意の ID。 編集不可。|
|number|string|仕入先番号。|
|displayName|string|仕入先の表示名。|
|address|[ナビゲーション."postaladdress](../resources/dynamics-complextypes.md)|仕入先の住所。|
|phoneNumber|string|仕入先の電話番号。|
|email|string|仕入先の電子メールアドレス。|
|Web サイト|string|ベンダーの web サイトアドレス。|
|taxRegistrationNumber|string|仕入先の税登録番号。|
|currencyId|GUID|仕入先の既定通貨コード ID。|
|currencyCode|string|仕入先の既定の通貨コード。|
|irs1099Code|string|ベンダーの1099コードを指定します。 US のみ|
|paymentTermsId|GUID|仕入先の既定の支払条件 ID。|
|paymentMethodId|GUID|仕入先の既定の支払方法 ID。|
|taxLiable|ブール値|仕入先が税金に対して責任を負わないかどうかを指定します。|
|ブロック|string|転記できない仕入先のトランザクションを指定します。 指定できる値は空白、支払いまたはすべてです|
|対照|decimal|仕入先の残高。 読み取り専用です。|
|lastModifiedDateTime|datetime|ベンダーが最後に変更された datetime。 読み取り専用です。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、ベンダーの JSON 表記です。

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

