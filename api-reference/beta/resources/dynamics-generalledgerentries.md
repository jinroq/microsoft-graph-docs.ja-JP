---
title: 一般に、リソースの種類
description: Dynamics 365 Business Central の総勘定元帳エントリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365760"
---
# <a name="generalledgerentries-resource-type"></a>一般に、リソースの種類
Dynamics 365 Business Central の一般に備えた入力オブジェクトを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:-------------|:-------------|:----------|
|[一般に備えた gerentries エントリを取得する](../api/dynamics-generalledgerentries-get.md)|一般に備えた gerentries|G/L entry オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|ID                  |numeric                |G/L エントリの一意の ID。              |
|postingdate         |日付                   |G/L エントリの転記日を指定します。 |
|documentnumber      |文字列、最大サイズ20|G/L エントリのドキュメント番号を指定します。|
|documentType        |string                 |G/L エントリのドキュメントの種類を指定します。|
|accountId           |GUID                   |G/L エントリの accountId を指定します。    |
|accountnumber       |文字列、最大サイズ20|G/L エントリの accountnumber を指定します。|
|説明         |文字列、最大サイズ50|G/L エントリの説明を指定します。  |
|debitamount         |numeric                |G/L エントリの金額を指定します。  |
|creditAmount        |numeric                |G/L エントリの creditAmount を指定します。 |
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

