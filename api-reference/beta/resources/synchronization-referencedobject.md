---
title: referencedObject リソースの種類
description: 同じディレクトリの定義で定義されている別のオブジェクトへの参照について説明します。
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529321"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="1d06c-103">referencedObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d06c-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d06c-104">同じ[ディレクトリの定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d06c-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1d06c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d06c-105">Properties</span></span>

| <span data-ttu-id="1d06c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d06c-106">Property</span></span>                   | <span data-ttu-id="1d06c-107">型</span><span class="sxs-lookup"><span data-stu-id="1d06c-107">Type</span></span>                      | <span data-ttu-id="1d06c-108">説明</span><span class="sxs-lookup"><span data-stu-id="1d06c-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="1d06c-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="1d06c-109">referencedObjectName</span></span>        |<span data-ttu-id="1d06c-110">String</span><span class="sxs-lookup"><span data-stu-id="1d06c-110">String</span></span>                     |<span data-ttu-id="1d06c-111">参照先オブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="1d06c-111">Name of the referenced object.</span></span> <span data-ttu-id="1d06c-112">[ディレクトリの定義](synchronization-directorydefinition.md)内のオブジェクトのいずれかに一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d06c-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="1d06c-113">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="1d06c-113">referencedProperty</span></span>          |<span data-ttu-id="1d06c-114">String</span><span class="sxs-lookup"><span data-stu-id="1d06c-114">String</span></span>                     |<span data-ttu-id="1d06c-115">現時点ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d06c-115">**Currently not supported**.</span></span> <span data-ttu-id="1d06c-116">対象の値が、参照として使用されるが、参照されるオブジェクトのプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="1d06c-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d06c-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d06c-117">JSON representation</span></span>

<span data-ttu-id="1d06c-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d06c-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-referencedobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
            
