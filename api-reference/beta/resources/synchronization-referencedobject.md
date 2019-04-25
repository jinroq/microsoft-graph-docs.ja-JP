---
title: referencedobject リソースの種類
description: 同じディレクトリ定義で定義されている別のオブジェクトへの参照を記述します。
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523246"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="bdb00-103">referencedobject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bdb00-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdb00-104">同じ[ディレクトリ定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照を記述します。</span><span class="sxs-lookup"><span data-stu-id="bdb00-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bdb00-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdb00-105">Properties</span></span>

| <span data-ttu-id="bdb00-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdb00-106">Property</span></span>                   | <span data-ttu-id="bdb00-107">型</span><span class="sxs-lookup"><span data-stu-id="bdb00-107">Type</span></span>                      | <span data-ttu-id="bdb00-108">説明</span><span class="sxs-lookup"><span data-stu-id="bdb00-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="bdb00-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="bdb00-109">referencedObjectName</span></span>        |<span data-ttu-id="bdb00-110">String</span><span class="sxs-lookup"><span data-stu-id="bdb00-110">String</span></span>                     |<span data-ttu-id="bdb00-111">参照されるオブジェクトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="bdb00-111">Name of the referenced object.</span></span> <span data-ttu-id="bdb00-112">[ディレクトリ定義](synchronization-directorydefinition.md)内のいずれかのオブジェクトと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="bdb00-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="bdb00-113">referencedproperty</span><span class="sxs-lookup"><span data-stu-id="bdb00-113">referencedProperty</span></span>          |<span data-ttu-id="bdb00-114">String</span><span class="sxs-lookup"><span data-stu-id="bdb00-114">String</span></span>                     |<span data-ttu-id="bdb00-115">**現時点ではサポートされていません**。</span><span class="sxs-lookup"><span data-stu-id="bdb00-115">**Currently not supported**.</span></span> <span data-ttu-id="bdb00-116">参照されるオブジェクト内のプロパティの名前。その値は、参照として使用されます。</span><span class="sxs-lookup"><span data-stu-id="bdb00-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdb00-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bdb00-117">JSON representation</span></span>

<span data-ttu-id="bdb00-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bdb00-118">The following is a JSON representation of the resource.</span></span>

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
            
