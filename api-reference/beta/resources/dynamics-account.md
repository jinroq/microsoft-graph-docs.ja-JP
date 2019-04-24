---
title: accounts リソースの種類
description: Dynamics 365 Business Central の account オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507575"
---
# <a name="accounts-resource-type"></a>accounts リソースの種類
Dynamics 365 Business Central の account オブジェクトを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[アカウントを取得する](../api/dynamics-account-get.md)|アカウント|accounts オブジェクトを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|GUID|アカウントの一意の ID。|
|number|文字列、最大サイズ20|G/L アカウントの番号を指定します。|
|displayName|文字列、最大サイズ50|G/L アカウントの名前を指定します。|
|category|文字列、最大サイズ20|G/L アカウントのカテゴリを指定します。|
|カテゴリー|文字列、最大サイズ80|G/L アカウントのアカウントカテゴリのサブカテゴリを指定します。|
|ブロック|ブール値|G/L アカウントにエントリを投稿できないことを指定します。 **True**は、アカウントがブロックされ、投稿が許可されていないことを示します。|
|lastModifiedDateTime|datetime|アカウントが最後に変更された日付です。|


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
