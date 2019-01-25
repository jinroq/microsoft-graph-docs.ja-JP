---
title: educationSynchronizationDataProvider リソースの種類
description: 'ソース SIS のスキーマを表します。 これにより、受信データを Azure Active Directory (AD の Azure) スキーマにマップする方法を把握するシステムです。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515497"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ソース SIS のスキーマを表します。 これにより、受信データを Azure Active Directory (AD の Azure) スキーマにマップする方法を把握するシステムです。

> **注:** この複合型は抽象です。 特定の種類の一覧のデータ プロバイダーを参照してください。

## <a name="derived-types"></a>派生型
| 型 | 説明 |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | 入力ソースとして CSV ファイルを使用します。 |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | 入力ソースとして PowerSchool を使用します。 |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | 入力ソースとして、OneRoster API を使用します。 |

## <a name="properties"></a>プロパティ

この型でのプロパティはありません。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
