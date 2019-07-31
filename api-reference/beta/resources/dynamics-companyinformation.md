---
title: 会社情報リソースの種類
description: Dynamics 365 Business Central の会社情報。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 2e23660775ba96b3f898840b0bad2b53eff9584a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012668"
---
# <a name="companyinformation-resource-type"></a>会社情報リソースの種類
Dynamics 365 Business Central の現在の会社に対して指定されている情報 (名前、住所、電子メールアドレス、web サイトのアドレスなど) を表します。

## <a name="methods"></a>メソッド

| メソッド         | 戻り値の型  |説明|
|:---------------|:-------------|:----------|
|[会社情報の取得](../api/dynamics-companyinformation-get.md)|会社情報|会社の情報を取得します。|
|[パッチ会社の情報](../api/dynamics-companyinformation-update.md)|会社情報|会社情報を更新します。|


## <a name="properties"></a>プロパティ
| プロパティ     | 型      |説明                           |
|:-------------|:--------|:-------------------------------------|
|id            |GUID|会社の一意の ID。 編集できません。|
|displayName   |string   |会社の表示名。           |
|address       |[ナビゲーション."Postaladdress](../resources/dynamics-complextypes.md)|会社の住所。 詳細については、「複合型」を参照してください。|
|phoneNumber   |string   |会社の電話番号。       |
|faxNumber     |string   |会社の fax 番号。             |
|email         |string   |会社の電子メールアドレス。          |
|Web サイト       |string   |会社の web サイトアドレス。        |
|taxRegistrationNumber|string|会社の税務登録番号。|
|currencyCode  |string   |会社が事業を行う通貨。 読み取り専用です。|
|currentFiscalYearStartDate|date|会社の現在の会計年度の開始日。 読み取り専用です。|
|おける      |string   |会社が属している業界。  |
|表       |stream   |会社のロゴ。 読み取り専用です。          |
|businessProfileId|string|財務会社にリンクされているビジネスプロファイル ID。 読み取り専用です。|
|lastModifiedDateTime|datetime|会社が変更された最後の日付です。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

会社情報の JSON 表記を次に示します。
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```

