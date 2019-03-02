---
title: journalLines リソースの種類
description: Dynamics 365 Business Central のジャーナル明細行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7a6841bcc2f893f8ca794e7d8e6aeafbcd4e48ca
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365956"
---
# <a name="journallines-resource-type"></a>journalLines リソースの種類
Dynamics 365 Business Central のジャーナルの行を表します。

## <a name="methods"></a>メソッド

| メソッド                                                    | 戻り値の型|説明         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[journalLines を取得する](../api/dynamics-journalline-get.md)      |journalLines|仕訳帳明細行を取得します。   |
|[Post journalLines](../api/dynamics-create-journalline.md)  |journalLines|仕訳帳明細行を作成します。|
|[Patch journalLines](../api/dynamics-journalline-update.md) |journalLines|仕訳帳明細行を更新します。|
|[journalLines の削除](../api/dynamics-journalline-delete.md)|none        |仕訳帳明細行を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ             | 型                   |説明                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|ID                    |GUID                    |仕訳帳明細行の一意の ID。 編集不可。                   |
|journalDisplayName    |文字列、最大サイズ10 |この行が属するジャーナルの表示名。 読み取り専用です。|
|lineNumber            |integer                 |仕訳帳明細行の番号。                                    |
|accountId             |GUID                    |仕訳帳明細行が関連付けられているアカウントの一意の ID。  |
|accountnumber         |文字列、最大サイズ20 |仕訳帳明細行が関連付けられているアカウントの番号。     |
|postingdate           |日付                    |仕訳帳明細行が転記される日付。                          |
|documentnumber        |文字列、最大サイズ20 |仕訳帳明細行の文書番号を指定します。                  |
|externaldocumentnumber|文字列、最大サイズ20 |仕訳帳明細行の外部ドキュメント番号を指定します。        |
|値                |decimal                 |仕訳帳明細行を構成する合計金額 (VAT を含む) を指定します。|
|説明           |文字列、最大サイズ50 |ユーザーまたは autocreated によって提供される、仕訳帳明細行の説明。|
|コメント               |文字列、最大サイズ250|ユーザーが仕訳帳明細行に対して指定したコメント。                      |
|lastModifiedDateTime  |datetime                |履歴明細行が変更された最後の datetime。 読み取り専用です。        |

## <a name="relationships"></a>リレーションシップ
ジャーナル明細行は、ジャーナルのサブページです。 直接アクセスすることはできません。

仕訳線は、寸法線の "親エンティティ" にすることができます。

アカウント (accountId) は、Accounts テーブルに存在する必要があります。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```
