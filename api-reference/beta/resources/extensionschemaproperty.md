---
title: extensionSchemaProperty リソースの種類
description: '**extensionSchemaProperty** リソースを使用して、schemaExtension 定義の一部としてプロパティの名前とその種類を定義します。'
ms.openlocfilehash: f699ccebefc849a7bf9cacc6dbda61cbcbb9896d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068094"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="dd97a-103">extensionSchemaProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dd97a-103">extensionSchemaProperty resource type</span></span>

> <span data-ttu-id="dd97a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dd97a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd97a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd97a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd97a-106">**extensionSchemaProperty** リソースを使用して、[schemaExtension](schemaextension.md) 定義の一部としてプロパティの名前とその種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="dd97a-106">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="dd97a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd97a-107">Properties</span></span>
| <span data-ttu-id="dd97a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd97a-108">Property</span></span>     | <span data-ttu-id="dd97a-109">型</span><span class="sxs-lookup"><span data-stu-id="dd97a-109">Type</span></span>   |<span data-ttu-id="dd97a-110">説明</span><span class="sxs-lookup"><span data-stu-id="dd97a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd97a-111">名前</span><span class="sxs-lookup"><span data-stu-id="dd97a-111">name</span></span>|<span data-ttu-id="dd97a-112">String</span><span class="sxs-lookup"><span data-stu-id="dd97a-112">String</span></span>| <span data-ttu-id="dd97a-113">スキーマの拡張機能の一部として定義されている厳密に型指定されたプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="dd97a-113">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="dd97a-114">type</span><span class="sxs-lookup"><span data-stu-id="dd97a-114">type</span></span>|<span data-ttu-id="dd97a-115">String</span><span class="sxs-lookup"><span data-stu-id="dd97a-115">String</span></span>| <span data-ttu-id="dd97a-p102">スキーマの拡張機能の一部として定義されているプロパティの種類。使用可能な値は、*Binary、Boolean、DateTime、Integer\*\*String* です。詳細については、次の表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd97a-p102">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="dd97a-119">サポート対象のプロパティ データ型</span><span class="sxs-lookup"><span data-stu-id="dd97a-119">Supported property data types</span></span> 
<span data-ttu-id="dd97a-120">スキーマ拡張機能でプロパティを定義する場合、次のデータ型がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="dd97a-120">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="dd97a-121">プロパティの種類</span><span class="sxs-lookup"><span data-stu-id="dd97a-121">Property Type</span></span> | <span data-ttu-id="dd97a-122">注釈</span><span class="sxs-lookup"><span data-stu-id="dd97a-122">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="dd97a-123">Binary</span><span class="sxs-lookup"><span data-stu-id="dd97a-123">Binary</span></span> | <span data-ttu-id="dd97a-124">最大 256 バイトです。</span><span class="sxs-lookup"><span data-stu-id="dd97a-124">256 bytes maximum.</span></span> |
| <span data-ttu-id="dd97a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd97a-125">Boolean</span></span> | <span data-ttu-id="dd97a-126">メッセージ、イベント、投稿ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd97a-126">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="dd97a-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="dd97a-127">DateTime</span></span> | <span data-ttu-id="dd97a-p103">ISO 8601 形式で指定する必要があります。UTC で格納されます。</span><span class="sxs-lookup"><span data-stu-id="dd97a-p103">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="dd97a-130">整数</span><span class="sxs-lookup"><span data-stu-id="dd97a-130">Integer</span></span> | <span data-ttu-id="dd97a-p104">32 ビット値です。メッセージ、イベント、投稿ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd97a-p104">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="dd97a-133">String</span><span class="sxs-lookup"><span data-stu-id="dd97a-133">String</span></span> | <span data-ttu-id="dd97a-134">最大 256 文字です。</span><span class="sxs-lookup"><span data-stu-id="dd97a-134">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd97a-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd97a-135">JSON representation</span></span>
<span data-ttu-id="dd97a-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dd97a-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->