---
title: educationSynchronizationDataProvider リソースの種類
description: 'ソース SIS のスキーマを表します。 これにより、受信データを Azure Active Directory (AD の Azure) スキーマにマップする方法を把握するシステムです。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f1e51bd0039b28aa08fa71956efc5143df77651c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420970"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

ソース SIS のスキーマを表します。 これにより、受信データを Azure Active Directory (AD の Azure) スキーマにマップする方法を把握するシステムです。 

> **注:** この複合型は抽象です。 特定の種類の一覧のデータ プロバイダーを参照してください。

## <a name="derived-types"></a>派生型
| Type | 説明 | 
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | 入力ソースとして CSV ファイルを使用します。 |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | 入力ソースとして PowerSchool を使用します。 |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | 入力ソースとして、OneRoster API を使用します。 |

## <a name="properties"></a>プロパティ

この型でのプロパティはありません。



<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationDataProvider "
}-->

```json
{
}
```
