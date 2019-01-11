---
title: educationSynchronizationCustomization リソースの種類
description: 'リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。 同期されているすべてのエンティティには、カスタマイズを適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9294af5796daeefb394ed1625a9a36128ae7b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860901"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。 同期されているすべてのエンティティには、カスタマイズを適用できます。 

>**注:****SynchronizationStartDate**プロパティは、 **StudentEnrollment**のエンティティにのみ適用されます。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **optionalPropertiesToSync** | 文字列のコレクション |  同期するプロパティ名のコレクションです。かどうかのセットを null に、すべてのプロパティが同期します。       |
| **synchronizationStartDate** | DateTime |  同期を開始する日付。 この値は、将来の日付に設定する必要があります。 場合は null の場合、リソースに設定は、プロファイルの設定が完了したときに同期されます。 **注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。      |
|**isSyncDeferred** |ブール型 | 親エンティティの同期がそれ以降の日付に延期されたかどうかを示します。 |
| **allowDisplayNameUpdate** | ブール型 |  同期によって、リソースの表示名を上書きするかどうかを示します。         |


## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
