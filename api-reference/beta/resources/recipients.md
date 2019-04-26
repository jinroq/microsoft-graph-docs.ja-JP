---
title: recipients リソースの種類
description: 以下は、リソースの JSON 表記です
localization_priority: Normal
ms.openlocfilehash: 367b796f46dce0f68e8077f7eba93ef0216279f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343956"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="921bf-103">recipients リソースの種類</span><span class="sxs-lookup"><span data-stu-id="921bf-103">recipients resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="921bf-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="921bf-104">JSON representation</span></span>

<span data-ttu-id="921bf-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="921bf-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="921bf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="921bf-106">Properties</span></span>
| <span data-ttu-id="921bf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="921bf-107">Property</span></span>     | <span data-ttu-id="921bf-108">型</span><span class="sxs-lookup"><span data-stu-id="921bf-108">Type</span></span>   |<span data-ttu-id="921bf-109">説明</span><span class="sxs-lookup"><span data-stu-id="921bf-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="921bf-110">alias</span><span class="sxs-lookup"><span data-stu-id="921bf-110">alias</span></span>|<span data-ttu-id="921bf-111">String</span><span class="sxs-lookup"><span data-stu-id="921bf-111">String</span></span>||
|<span data-ttu-id="921bf-112">email</span><span class="sxs-lookup"><span data-stu-id="921bf-112">email</span></span>|<span data-ttu-id="921bf-113">String</span><span class="sxs-lookup"><span data-stu-id="921bf-113">String</span></span>||
|<span data-ttu-id="921bf-114">objectId</span><span class="sxs-lookup"><span data-stu-id="921bf-114">objectId</span></span>|<span data-ttu-id="921bf-115">String</span><span class="sxs-lookup"><span data-stu-id="921bf-115">String</span></span>||
|<span data-ttu-id="921bf-116">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="921bf-116">permissionIdentityType</span></span>|<span data-ttu-id="921bf-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="921bf-117">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
