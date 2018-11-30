---
title: inferenceClassificationOverride リソースの種類
description: 特定の送信者からの受信のメッセージのユーザーのオーバーライドする必要があります常として分類されます。
ms.openlocfilehash: 63c753b7af21907717d7d9706d0606726d5670f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067523"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="e9101-103">inferenceClassificationOverride リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9101-103">inferenceClassificationOverride resource type</span></span>

> <span data-ttu-id="e9101-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e9101-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9101-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9101-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9101-106">どのように特定の送信者からメッセージを受信する必要があります常に分類される、[受信トレイの中心](manage-focused-inbox.md)のように、ユーザーのオーバーライドを表します。</span><span class="sxs-lookup"><span data-stu-id="e9101-106">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="e9101-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e9101-107">Methods</span></span>

| <span data-ttu-id="e9101-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e9101-108">Method</span></span>           | <span data-ttu-id="e9101-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e9101-109">Return Type</span></span>    |<span data-ttu-id="e9101-110">説明</span><span class="sxs-lookup"><span data-stu-id="e9101-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e9101-111">Update</span><span class="sxs-lookup"><span data-stu-id="e9101-111">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="e9101-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e9101-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="e9101-113">指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。</span><span class="sxs-lookup"><span data-stu-id="e9101-113">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="e9101-114">削除</span><span class="sxs-lookup"><span data-stu-id="e9101-114">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="e9101-115">なし</span><span class="sxs-lookup"><span data-stu-id="e9101-115">None</span></span> |<span data-ttu-id="e9101-116">その ID で指定されたオーバーライドを削除します。</span><span class="sxs-lookup"><span data-stu-id="e9101-116">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="e9101-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9101-117">Properties</span></span>
| <span data-ttu-id="e9101-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9101-118">Property</span></span>     | <span data-ttu-id="e9101-119">型</span><span class="sxs-lookup"><span data-stu-id="e9101-119">Type</span></span>   |<span data-ttu-id="e9101-120">説明</span><span class="sxs-lookup"><span data-stu-id="e9101-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9101-121">classifyAs</span><span class="sxs-lookup"><span data-stu-id="e9101-121">classifyAs</span></span>|<span data-ttu-id="e9101-122">文字列</span><span class="sxs-lookup"><span data-stu-id="e9101-122">string</span></span>| <span data-ttu-id="e9101-p102">特定の差出人からの着信メッセージを常時分類する方法を指定します。可能な値は、`focused`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="e9101-p102">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="e9101-125">ID</span><span class="sxs-lookup"><span data-stu-id="e9101-125">id</span></span>|<span data-ttu-id="e9101-126">文字列</span><span class="sxs-lookup"><span data-stu-id="e9101-126">string</span></span>| <span data-ttu-id="e9101-p103">オーバーライドの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e9101-p103">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="e9101-129">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e9101-129">senderEmailAddress</span></span>|[<span data-ttu-id="e9101-130">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e9101-130">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="e9101-131">オーバーライドを作成する対象の差出人のメール アドレス情報。</span><span class="sxs-lookup"><span data-stu-id="e9101-131">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9101-132">関係</span><span class="sxs-lookup"><span data-stu-id="e9101-132">Relationships</span></span>
<span data-ttu-id="e9101-133">なし</span><span class="sxs-lookup"><span data-stu-id="e9101-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e9101-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9101-134">JSON representation</span></span>

<span data-ttu-id="e9101-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e9101-135">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->