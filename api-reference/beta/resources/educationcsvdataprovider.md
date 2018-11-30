---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。  '
ms.openlocfilehash: a3079b4f18c74c95fb0f8646116f2c7901d17b3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066864"
---
# <a name="educationcsvdataprovider-resource-type"></a>educationCsvDataProvider リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

CSV ファイルは、入力ソースとは、学校のデータの同期プロファイルを設定するために使用します。  

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **カスタマイズ** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルを適用するオプションのカスタマイズです。|

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
