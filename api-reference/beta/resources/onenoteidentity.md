---
title: oneNoteIdentity リソースの種類
description: '**準備中のサポート**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7ce71775842cc6b7084b86e13e9e4715765567ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963214"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="05d65-103">oneNoteIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05d65-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="05d65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05d65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05d65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05d65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05d65-106">**準備中のサポート**</span><span class="sxs-lookup"><span data-stu-id="05d65-106">**Support coming soon**</span></span>

<span data-ttu-id="05d65-107">OneNoteIdentity 型は、_ユーザー_の id を表します。</span><span class="sxs-lookup"><span data-stu-id="05d65-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="05d65-108">[Id](identity.md)を使用してこの型をマージする将来的には、</span><span class="sxs-lookup"><span data-stu-id="05d65-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="05d65-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05d65-109">JSON representation</span></span>

<span data-ttu-id="05d65-110">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05d65-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="05d65-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05d65-111">Properties</span></span>
| <span data-ttu-id="05d65-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05d65-112">Property</span></span>     | <span data-ttu-id="05d65-113">種類</span><span class="sxs-lookup"><span data-stu-id="05d65-113">Type</span></span>   |<span data-ttu-id="05d65-114">説明</span><span class="sxs-lookup"><span data-stu-id="05d65-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05d65-115">displayName</span><span class="sxs-lookup"><span data-stu-id="05d65-115">displayName</span></span>|<span data-ttu-id="05d65-116">string</span><span class="sxs-lookup"><span data-stu-id="05d65-116">string</span></span>|<span data-ttu-id="05d65-117">Id の表示名です。</span><span class="sxs-lookup"><span data-stu-id="05d65-117">The identity's display name.</span></span>|
|<span data-ttu-id="05d65-118">ID</span><span class="sxs-lookup"><span data-stu-id="05d65-118">id</span></span>|<span data-ttu-id="05d65-119">文字列</span><span class="sxs-lookup"><span data-stu-id="05d65-119">string</span></span>|<span data-ttu-id="05d65-120">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="05d65-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
