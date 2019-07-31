---
title: referencedObject リソースの種類
description: 同じディレクトリ定義で定義されている別のオブジェクトへの参照を記述します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1c7e1554764031efbfa3a5d1c1280f4b72bc160
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007859"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="3c735-103">referencedObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c735-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c735-104">同じ[ディレクトリ定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照を記述します。</span><span class="sxs-lookup"><span data-stu-id="3c735-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3c735-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c735-105">Properties</span></span>

| <span data-ttu-id="3c735-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c735-106">Property</span></span>                   | <span data-ttu-id="3c735-107">型</span><span class="sxs-lookup"><span data-stu-id="3c735-107">Type</span></span>                      | <span data-ttu-id="3c735-108">説明</span><span class="sxs-lookup"><span data-stu-id="3c735-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="3c735-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="3c735-109">referencedObjectName</span></span>        |<span data-ttu-id="3c735-110">String</span><span class="sxs-lookup"><span data-stu-id="3c735-110">String</span></span>                     |<span data-ttu-id="3c735-111">参照されるオブジェクトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c735-111">Name of the referenced object.</span></span> <span data-ttu-id="3c735-112">[ディレクトリ定義](synchronization-directorydefinition.md)内のいずれかのオブジェクトと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c735-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="3c735-113">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="3c735-113">referencedProperty</span></span>          |<span data-ttu-id="3c735-114">String</span><span class="sxs-lookup"><span data-stu-id="3c735-114">String</span></span>                     |<span data-ttu-id="3c735-115">**現時点ではサポートされていません**。</span><span class="sxs-lookup"><span data-stu-id="3c735-115">**Currently not supported**.</span></span> <span data-ttu-id="3c735-116">参照されるオブジェクト内のプロパティの名前。その値は、参照として使用されます。</span><span class="sxs-lookup"><span data-stu-id="3c735-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c735-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c735-117">JSON representation</span></span>

<span data-ttu-id="3c735-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3c735-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
            
