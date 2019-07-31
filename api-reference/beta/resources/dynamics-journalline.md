---
title: journalLines リソースの種類
description: Dynamics 365 Business Central のジャーナル明細行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: cb9b20d7d88159dbddd2a18caa6db7fe52e5a601
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972916"
---
# <a name="journallines-resource-type"></a>journalLines リソースの種類
Dynamics 365 Business Central のジャーナルの行を表します。

## <a name="methods"></a>メソッド

| メソッド                                                    | 戻り値の型|説明         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[JournalLines を取得する](../api/dynamics-journalline-get.md)      |journalLines|仕訳帳明細行を取得します。   |
|[Post journalLines](../api/dynamics-create-journalline.md)  |journalLines|仕訳帳明細行を作成します。|
|[Patch journalLines](../api/dynamics-journalline-update.md) |journalLines|仕訳帳明細行を更新します。|
|[JournalLines の削除](../api/dynamics-journalline-delete.md)|none        |仕訳帳明細行を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ             | 型                   |説明                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|id                    |GUID                    |仕訳帳明細行の一意の ID。 編集できません。                   |
|journalDisplayName    |文字列、最大サイズ10 |この行が属するジャーナルの表示名。 読み取り専用です。|
|lineNumber            |整数                 |仕訳帳明細行の番号。                                    |
|accountId             |GUID                    |仕訳帳明細行が関連付けられているアカウントの一意の ID。  |
|accountNumber         |文字列、最大サイズ20 |仕訳帳明細行が関連付けられているアカウントの番号。     |
|postingDate           |date                    |仕訳帳明細行が転記される日付。                          |
|documentNumber        |文字列、最大サイズ20 |仕訳帳明細行の文書番号を指定します。                  |
|externalDocumentNumber|文字列、最大サイズ20 |仕訳帳明細行の外部ドキュメント番号を指定します。        |
|値                |decimal                 |仕訳帳明細行を構成する合計金額 (VAT を含む) を指定します。|
|description           |文字列、最大サイズ50 |ユーザーまたは autocreated によって提供される、仕訳帳明細行の説明。|
|コメント               |文字列、最大サイズ250|ユーザーが仕訳帳明細行に対して指定したコメント。                      |
|lastModifiedDateTime  |datetime                |履歴明細行が変更された最後の datetime。 読み取り専用。        |

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
