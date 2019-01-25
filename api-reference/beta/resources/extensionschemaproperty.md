---
title: extensionSchemaProperty リソースの種類
description: '**extensionSchemaProperty** リソースを使用して、schemaExtension 定義の一部としてプロパティの名前とその種類を定義します。'
localization_priority: Normal
ms.openlocfilehash: bb044aa2f85ea5accdba4ed43a1a5b1c856a209d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511507"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="9a772-103">extensionSchemaProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a772-103">extensionSchemaProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a772-104">**extensionSchemaProperty** リソースを使用して、[schemaExtension](schemaextension.md) 定義の一部としてプロパティの名前とその種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="9a772-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="9a772-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a772-105">Properties</span></span>
| <span data-ttu-id="9a772-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a772-106">Property</span></span>     | <span data-ttu-id="9a772-107">型</span><span class="sxs-lookup"><span data-stu-id="9a772-107">Type</span></span>   |<span data-ttu-id="9a772-108">説明</span><span class="sxs-lookup"><span data-stu-id="9a772-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a772-109">name</span><span class="sxs-lookup"><span data-stu-id="9a772-109">name</span></span>|<span data-ttu-id="9a772-110">String</span><span class="sxs-lookup"><span data-stu-id="9a772-110">String</span></span>| <span data-ttu-id="9a772-111">スキーマの拡張機能の一部として定義されている厳密に型指定されたプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="9a772-111">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="9a772-112">type</span><span class="sxs-lookup"><span data-stu-id="9a772-112">type</span></span>|<span data-ttu-id="9a772-113">String</span><span class="sxs-lookup"><span data-stu-id="9a772-113">String</span></span>| <span data-ttu-id="9a772-p101">スキーマの拡張機能の一部として定義されているプロパティの種類。使用可能な値は、*Binary、Boolean、DateTime、Integer\*\*String* です。詳細については、次の表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a772-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="9a772-117">サポート対象のプロパティ データ型</span><span class="sxs-lookup"><span data-stu-id="9a772-117">Supported property data types</span></span> 
<span data-ttu-id="9a772-118">スキーマ拡張機能でプロパティを定義する場合、次のデータ型がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9a772-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="9a772-119">プロパティの種類</span><span class="sxs-lookup"><span data-stu-id="9a772-119">Property Type</span></span> | <span data-ttu-id="9a772-120">注釈</span><span class="sxs-lookup"><span data-stu-id="9a772-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="9a772-121">Binary</span><span class="sxs-lookup"><span data-stu-id="9a772-121">Binary</span></span> | <span data-ttu-id="9a772-122">最大 256 バイトです。</span><span class="sxs-lookup"><span data-stu-id="9a772-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="9a772-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a772-123">Boolean</span></span> | <span data-ttu-id="9a772-124">メッセージ、イベント、投稿ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a772-124">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="9a772-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="9a772-125">DateTime</span></span> | <span data-ttu-id="9a772-p102">ISO 8601 形式で指定する必要があります。UTC で格納されます。</span><span class="sxs-lookup"><span data-stu-id="9a772-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="9a772-128">整数</span><span class="sxs-lookup"><span data-stu-id="9a772-128">Integer</span></span> | <span data-ttu-id="9a772-p103">32 ビット値です。メッセージ、イベント、投稿ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a772-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="9a772-131">String</span><span class="sxs-lookup"><span data-stu-id="9a772-131">String</span></span> | <span data-ttu-id="9a772-132">最大 256 文字です。</span><span class="sxs-lookup"><span data-stu-id="9a772-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a772-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a772-133">JSON representation</span></span>
<span data-ttu-id="9a772-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9a772-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/extensionschemaproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
