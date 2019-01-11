---
title: inferenceClassificationOverride リソースの種類
description: 特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。
localization_priority: Normal
ms.openlocfilehash: 8df0f1e5fa34c630c51de7c73234e6092448f867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885065"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="06672-103">inferenceClassificationOverride リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06672-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="06672-104">特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。</span><span class="sxs-lookup"><span data-stu-id="06672-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="06672-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="06672-105">Methods</span></span>

| <span data-ttu-id="06672-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="06672-106">Method</span></span>           | <span data-ttu-id="06672-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06672-107">Return Type</span></span>    |<span data-ttu-id="06672-108">説明</span><span class="sxs-lookup"><span data-stu-id="06672-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06672-109">Update</span><span class="sxs-lookup"><span data-stu-id="06672-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="06672-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="06672-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="06672-111">指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。</span><span class="sxs-lookup"><span data-stu-id="06672-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="06672-112">Delete</span><span class="sxs-lookup"><span data-stu-id="06672-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="06672-113">なし</span><span class="sxs-lookup"><span data-stu-id="06672-113">None</span></span> |<span data-ttu-id="06672-114">その ID で指定されたオーバーライドを削除します。</span><span class="sxs-lookup"><span data-stu-id="06672-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="06672-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06672-115">Properties</span></span>
| <span data-ttu-id="06672-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06672-116">Property</span></span>     | <span data-ttu-id="06672-117">種類</span><span class="sxs-lookup"><span data-stu-id="06672-117">Type</span></span>   |<span data-ttu-id="06672-118">説明</span><span class="sxs-lookup"><span data-stu-id="06672-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06672-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="06672-119">classifyAs</span></span>|<span data-ttu-id="06672-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="06672-120">inferenceClassificationType</span></span>| <span data-ttu-id="06672-121">特定の差出人からの着信メッセージを常時分類する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="06672-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="06672-122">可能な値: `focused`、 `other`。</span><span class="sxs-lookup"><span data-stu-id="06672-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="06672-123">ID</span><span class="sxs-lookup"><span data-stu-id="06672-123">id</span></span>|<span data-ttu-id="06672-124">文字列</span><span class="sxs-lookup"><span data-stu-id="06672-124">string</span></span>| <span data-ttu-id="06672-p102">オーバーライドの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="06672-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="06672-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="06672-127">senderEmailAddress</span></span>|[<span data-ttu-id="06672-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="06672-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="06672-129">オーバーライドを作成する対象の差出人のメール アドレス情報。</span><span class="sxs-lookup"><span data-stu-id="06672-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06672-130">関係</span><span class="sxs-lookup"><span data-stu-id="06672-130">Relationships</span></span>
<span data-ttu-id="06672-131">なし</span><span class="sxs-lookup"><span data-stu-id="06672-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="06672-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06672-132">JSON representation</span></span>

<span data-ttu-id="06672-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06672-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
