---
title: 一般に、リソースの種類
description: Dynamics 365 Business Central の総勘定元帳エントリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 500c78d0e29d83c68c2b7247a9787b977cc8a7b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973605"
---
# <a name="generalledgerentries-resource-type"></a>一般に、リソースの種類
Dynamics 365 Business Central の一般に備えた入力オブジェクトを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:-------------|:-------------|:----------|
|[一般に備えた Gerentries エントリを取得する](../api/dynamics-generalledgerentries-get.md)|一般に備えた Gerentries|G/L entry オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|id                  |数値                |G/L エントリの一意の ID。              |
|postingDate         |date                   |G/L エントリの転記日を指定します。 |
|documentNumber      |文字列、最大サイズ20|G/L エントリのドキュメント番号を指定します。|
|documentType        |string                 |G/L エントリのドキュメントの種類を指定します。|
|accountId           |GUID                   |G/L エントリの accountId を指定します。    |
|accountNumber       |文字列、最大サイズ20|G/L エントリの accountNumber を指定します。|
|description         |文字列、最大サイズ50|G/L エントリの説明を指定します。  |
|debitAmount         |数値                |G/L エントリの金額を指定します。  |
|creditAmount        |数値                |G/L エントリの creditAmount を指定します。 |
|lastModifiedDateTime|datetime               |G/L エントリが変更された最後の datetime。|


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

