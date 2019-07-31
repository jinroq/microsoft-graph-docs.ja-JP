---
title: employees リソースの種類
description: Dynamics 365 Business Central の employee オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 96d44856ad52c983e61181fc64b93477fbe79e6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972951"
---
# <a name="employees-resource-type"></a>employees リソースの種類
Dynamics 365 Business Central の従業員を表します。

## <a name="methods"></a>メソッド

| メソッド                                              | 戻り値の型|説明               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[従業員の取得](../api/dynamics-employee-get.md)      |向け  |Employee オブジェクトを取得します。   |
|[従業員の投稿](../api/dynamics-create-employee.md)  |向け  |Employee オブジェクトを作成します。|
|[パッチの従業員](../api/dynamics-employee-update.md) |向け  |Employee オブジェクトを更新します。|
|[従業員を削除する](../api/dynamics-employee-delete.md)|none       |Employee オブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型   |説明                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |GUID    |従業員 ID。 編集できません。                         |
|番号              |string  |従業員番号。 読み取り専用です。                        |
|displayName         |string  |従業員の givenName + 姓。 読み取り専用です。           |
|givenName           |string  |従業員の指定された名前。                        |
|middleName          |string  |従業員のミドルネーム。                       |
|surname             |string  |従業員の姓                            |
|jobTitle            |string  |従業員の正式な名前                          |
|address             |[ナビゲーション."Postaladdress](../resources/dynamics-complextypes.md)|従業員の住所を指定します。 このアドレスは、従業員のすべてのリソースドキュメントに表示されます。|
|phoneNumber         |string  |従業員の電話番号を指定します。             |
|mobilePhone         |string  |従業員の携帯電話番号を指定します。      |
|email               |string  |従業員の電子メールアドレスを指定します。                |
|パーソナル電子メール       |string  |従業員の個人の電子メールアドレスを指定します。       |
|employmentDate      |date    |従業員が会社の作業を開始した日付を指定します。|
|終了した日付     |date    |退職または棄却のために従業員が終了した日付を指定します (例:)。|
|status              |string  |従業員の状態を指定します。 有効な値、非アクティブな値、または終了した値を指定します。|
|birthDate           |date    |従業員の生年月日を指定します。                |
|表             |stream  |従業員の画像。 読み取り専用です。                       |
|lastModifiedDateTime|datetime|従業員が最後に変更された日時。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

