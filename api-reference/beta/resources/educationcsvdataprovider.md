---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507176"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="49c4e-103">educationCsvDataProvider リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49c4e-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49c4e-104">CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="49c4e-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="49c4e-105">[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="49c4e-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="49c4e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49c4e-106">Properties</span></span>

| <span data-ttu-id="49c4e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49c4e-107">Property</span></span> | <span data-ttu-id="49c4e-108">型</span><span class="sxs-lookup"><span data-stu-id="49c4e-108">Type</span></span> | <span data-ttu-id="49c4e-109">説明</span><span class="sxs-lookup"><span data-stu-id="49c4e-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="49c4e-110">**ユーザー**</span><span class="sxs-lookup"><span data-stu-id="49c4e-110">**customizations**</span></span> | [<span data-ttu-id="49c4e-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="49c4e-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="49c4e-112">同期プロファイルに適用されるオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="49c4e-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49c4e-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49c4e-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcsvdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
