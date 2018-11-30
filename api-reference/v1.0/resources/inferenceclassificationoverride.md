---
title: inferenceClassificationOverride リソースの種類
description: 特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。
ms.openlocfilehash: 3f3f07e870a4ba549062197a380633ab591c54fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022021"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="03668-103">inferenceClassificationOverride リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03668-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="03668-104">特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。</span><span class="sxs-lookup"><span data-stu-id="03668-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="03668-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="03668-105">Methods</span></span>

| <span data-ttu-id="03668-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="03668-106">Method</span></span>           | <span data-ttu-id="03668-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="03668-107">Return Type</span></span>    |<span data-ttu-id="03668-108">説明</span><span class="sxs-lookup"><span data-stu-id="03668-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03668-109">Update</span><span class="sxs-lookup"><span data-stu-id="03668-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="03668-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="03668-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="03668-111">指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。</span><span class="sxs-lookup"><span data-stu-id="03668-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="03668-112">削除</span><span class="sxs-lookup"><span data-stu-id="03668-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="03668-113">なし</span><span class="sxs-lookup"><span data-stu-id="03668-113">None</span></span> |<span data-ttu-id="03668-114">その ID で指定されたオーバーライドを削除します。</span><span class="sxs-lookup"><span data-stu-id="03668-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="03668-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03668-115">Properties</span></span>
| <span data-ttu-id="03668-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03668-116">Property</span></span>     | <span data-ttu-id="03668-117">型</span><span class="sxs-lookup"><span data-stu-id="03668-117">Type</span></span>   |<span data-ttu-id="03668-118">説明</span><span class="sxs-lookup"><span data-stu-id="03668-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03668-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="03668-119">classifyAs</span></span>|<span data-ttu-id="03668-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="03668-120">inferenceClassificationType</span></span>| <span data-ttu-id="03668-121">特定の差出人からの着信メッセージを常時分類する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="03668-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="03668-122">可能な値: `focused`、 `other`。</span><span class="sxs-lookup"><span data-stu-id="03668-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="03668-123">ID</span><span class="sxs-lookup"><span data-stu-id="03668-123">id</span></span>|<span data-ttu-id="03668-124">文字列</span><span class="sxs-lookup"><span data-stu-id="03668-124">string</span></span>| <span data-ttu-id="03668-p102">オーバーライドの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03668-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="03668-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="03668-127">senderEmailAddress</span></span>|[<span data-ttu-id="03668-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="03668-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="03668-129">オーバーライドを作成する対象の差出人のメール アドレス情報。</span><span class="sxs-lookup"><span data-stu-id="03668-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03668-130">関係</span><span class="sxs-lookup"><span data-stu-id="03668-130">Relationships</span></span>
<span data-ttu-id="03668-131">なし</span><span class="sxs-lookup"><span data-stu-id="03668-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="03668-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03668-132">JSON representation</span></span>

<span data-ttu-id="03668-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03668-133">Here is a JSON representation of the resource.</span></span>

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