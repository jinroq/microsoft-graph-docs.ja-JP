---
title: oneNoteIdentity リソースの種類
description: '**準備中のサポート**'
localization_priority: Normal
ms.openlocfilehash: 80d0719bd2770b715902b5c600fe65012e0064d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883889"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="e14dc-103">oneNoteIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e14dc-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="e14dc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e14dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e14dc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e14dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e14dc-106">**準備中のサポート**</span><span class="sxs-lookup"><span data-stu-id="e14dc-106">**Support coming soon**</span></span>

<span data-ttu-id="e14dc-107">OneNoteIdentity 型は、_ユーザー_の id を表します。</span><span class="sxs-lookup"><span data-stu-id="e14dc-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="e14dc-108">[Id](identity.md)を使用してこの型をマージする将来的には、</span><span class="sxs-lookup"><span data-stu-id="e14dc-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="e14dc-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e14dc-109">JSON representation</span></span>

<span data-ttu-id="e14dc-110">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e14dc-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e14dc-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e14dc-111">Properties</span></span>
| <span data-ttu-id="e14dc-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e14dc-112">Property</span></span>     | <span data-ttu-id="e14dc-113">種類</span><span class="sxs-lookup"><span data-stu-id="e14dc-113">Type</span></span>   |<span data-ttu-id="e14dc-114">説明</span><span class="sxs-lookup"><span data-stu-id="e14dc-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e14dc-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e14dc-115">displayName</span></span>|<span data-ttu-id="e14dc-116">string</span><span class="sxs-lookup"><span data-stu-id="e14dc-116">string</span></span>|<span data-ttu-id="e14dc-117">Id の表示名です。</span><span class="sxs-lookup"><span data-stu-id="e14dc-117">The identity's display name.</span></span>|
|<span data-ttu-id="e14dc-118">ID</span><span class="sxs-lookup"><span data-stu-id="e14dc-118">id</span></span>|<span data-ttu-id="e14dc-119">文字列</span><span class="sxs-lookup"><span data-stu-id="e14dc-119">string</span></span>|<span data-ttu-id="e14dc-120">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e14dc-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
