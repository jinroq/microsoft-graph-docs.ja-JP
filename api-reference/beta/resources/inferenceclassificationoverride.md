---
title: inferenceClassificationOverride リソースの種類
description: 特定の送信者からの受信メッセージを常に分類する方法についてのユーザーのオーバーライドを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d01cbeb7b031c3e3b9ed66757a155eca6e33e479
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005766"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="481ee-103">inferenceClassificationOverride リソースの種類</span><span class="sxs-lookup"><span data-stu-id="481ee-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="481ee-104">特定の送信者からの受信メッセージを常に[優先受信トレイ](manage-focused-inbox.md)として分類する方法に対するユーザーのオーバーライドを表します。</span><span class="sxs-lookup"><span data-stu-id="481ee-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="481ee-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="481ee-105">Methods</span></span>

| <span data-ttu-id="481ee-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="481ee-106">Method</span></span>           | <span data-ttu-id="481ee-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="481ee-107">Return Type</span></span>    |<span data-ttu-id="481ee-108">説明</span><span class="sxs-lookup"><span data-stu-id="481ee-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="481ee-109">Update</span><span class="sxs-lookup"><span data-stu-id="481ee-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="481ee-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="481ee-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="481ee-111">指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。</span><span class="sxs-lookup"><span data-stu-id="481ee-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="481ee-112">Delete</span><span class="sxs-lookup"><span data-stu-id="481ee-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="481ee-113">None</span><span class="sxs-lookup"><span data-stu-id="481ee-113">None</span></span> |<span data-ttu-id="481ee-114">その ID で指定されたオーバーライドを削除します。</span><span class="sxs-lookup"><span data-stu-id="481ee-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="481ee-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="481ee-115">Properties</span></span>
| <span data-ttu-id="481ee-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="481ee-116">Property</span></span>     | <span data-ttu-id="481ee-117">型</span><span class="sxs-lookup"><span data-stu-id="481ee-117">Type</span></span>   |<span data-ttu-id="481ee-118">説明</span><span class="sxs-lookup"><span data-stu-id="481ee-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="481ee-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="481ee-119">classifyAs</span></span>|<span data-ttu-id="481ee-120">string</span><span class="sxs-lookup"><span data-stu-id="481ee-120">string</span></span>| <span data-ttu-id="481ee-p101">特定の差出人からの着信メッセージを常時分類する方法を指定します。可能な値は、`focused`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="481ee-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="481ee-123">id</span><span class="sxs-lookup"><span data-stu-id="481ee-123">id</span></span>|<span data-ttu-id="481ee-124">string</span><span class="sxs-lookup"><span data-stu-id="481ee-124">string</span></span>| <span data-ttu-id="481ee-p102">オーバーライドの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="481ee-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="481ee-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="481ee-127">senderEmailAddress</span></span>|[<span data-ttu-id="481ee-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="481ee-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="481ee-129">オーバーライドを作成する対象の差出人のメール アドレス情報。</span><span class="sxs-lookup"><span data-stu-id="481ee-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="481ee-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="481ee-130">Relationships</span></span>
<span data-ttu-id="481ee-131">なし</span><span class="sxs-lookup"><span data-stu-id="481ee-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="481ee-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="481ee-132">JSON representation</span></span>

<span data-ttu-id="481ee-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="481ee-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
