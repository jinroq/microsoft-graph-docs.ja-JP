---
title: referencedObject リソースの種類
description: 同じディレクトリの定義で定義されている別のオブジェクトへの参照について説明します。
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821036"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="8caee-103">referencedObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8caee-103">referencedObject resource type</span></span>

> <span data-ttu-id="8caee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8caee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8caee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8caee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8caee-106">同じ[ディレクトリの定義](synchronization-directorydefinition.md)で定義されている別のオブジェクトへの参照について説明します。</span><span class="sxs-lookup"><span data-stu-id="8caee-106">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8caee-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8caee-107">Properties</span></span>

| <span data-ttu-id="8caee-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8caee-108">Property</span></span>                   | <span data-ttu-id="8caee-109">種類</span><span class="sxs-lookup"><span data-stu-id="8caee-109">Type</span></span>                      | <span data-ttu-id="8caee-110">説明</span><span class="sxs-lookup"><span data-stu-id="8caee-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="8caee-111">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="8caee-111">referencedObjectName</span></span>        |<span data-ttu-id="8caee-112">String</span><span class="sxs-lookup"><span data-stu-id="8caee-112">String</span></span>                     |<span data-ttu-id="8caee-113">参照先オブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="8caee-113">Name of the referenced object.</span></span> <span data-ttu-id="8caee-114">[ディレクトリの定義](synchronization-directorydefinition.md)内のオブジェクトのいずれかに一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8caee-114">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="8caee-115">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="8caee-115">referencedProperty</span></span>          |<span data-ttu-id="8caee-116">String</span><span class="sxs-lookup"><span data-stu-id="8caee-116">String</span></span>                     |<span data-ttu-id="8caee-117">**サポートされていません**。</span><span class="sxs-lookup"><span data-stu-id="8caee-117">**Currently not supported**.</span></span> <span data-ttu-id="8caee-118">対象の値が、参照として使用されるが、参照されるオブジェクトのプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="8caee-118">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8caee-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8caee-119">JSON representation</span></span>

<span data-ttu-id="8caee-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8caee-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
