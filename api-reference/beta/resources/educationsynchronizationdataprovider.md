---
title: educationSynchronizationDataProvider リソースの種類
description: 'ソース SIS スキーマを表します。 これにより、システムは、受信データを azure Active Directory (azure AD) スキーマにマップする方法を知ることができます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507040"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>educationSynchronizationDataProvider リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ソース SIS スキーマを表します。 これにより、システムは、受信データを azure Active Directory (azure AD) スキーマにマップする方法を知ることができます。

> **注:** この複合型は抽象型です。 記載されている特定の種類のデータプロバイダーを参照してください。

## <a name="derived-types"></a>派生型
| 型 | 説明 |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | 入力ソースとして CSV ファイルで使用されます。 |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | 入力ソースとして powerschool を使用します。 |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | 入力ソースとして OneRoster API で使用されます。 |

## <a name="properties"></a>プロパティ

この種類のプロパティは公開されません。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
