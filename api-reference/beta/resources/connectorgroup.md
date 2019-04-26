---
title: コネクタグループリソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 5de46f480ff101e6d149bbfbe246ef47baff2604
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341202"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="1f0e0-103">コネクタグループリソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f0e0-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="1f0e0-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f0e0-104">Methods</span></span>

| <span data-ttu-id="1f0e0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f0e0-105">Method</span></span>           | <span data-ttu-id="1f0e0-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1f0e0-106">Return Type</span></span>    |<span data-ttu-id="1f0e0-107">説明</span><span class="sxs-lookup"><span data-stu-id="1f0e0-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f0e0-108">コネクタグループの取得</span><span class="sxs-lookup"><span data-stu-id="1f0e0-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="1f0e0-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1f0e0-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="1f0e0-110">コネクタのグループオブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="1f0e0-111">アプリケーションを作成する</span><span class="sxs-lookup"><span data-stu-id="1f0e0-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="1f0e0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f0e0-112">application</span></span>](application.md)| <span data-ttu-id="1f0e0-113">アプリケーションコレクションへの投稿によって、アプリケーションをコネクタグループに関連付けます。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="1f0e0-114">アプリケーションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1f0e0-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="1f0e0-115">[アプリケーション](application.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f0e0-115">[application](application.md) collection</span></span>| <span data-ttu-id="1f0e0-116">関連付けられているアプリケーションオブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="1f0e0-117">コネクタを作成する</span><span class="sxs-lookup"><span data-stu-id="1f0e0-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="1f0e0-118">コネクター</span><span class="sxs-lookup"><span data-stu-id="1f0e0-118">connector</span></span>](connector.md)| <span data-ttu-id="1f0e0-119">members コレクションへの投稿によってコネクタをコネクタグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="1f0e0-120">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1f0e0-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="1f0e0-121">[connector](connector.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f0e0-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="1f0e0-122">コネクタオブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="1f0e0-123">更新する</span><span class="sxs-lookup"><span data-stu-id="1f0e0-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="1f0e0-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1f0e0-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="1f0e0-125">コネクタグループオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="1f0e0-126">削除</span><span class="sxs-lookup"><span data-stu-id="1f0e0-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="1f0e0-127">なし</span><span class="sxs-lookup"><span data-stu-id="1f0e0-127">None</span></span> |<span data-ttu-id="1f0e0-128">コネクタグループオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-128">Delete connectorGroup object.</span></span> <span data-ttu-id="1f0e0-129">conector グループを削除する前に、すべてのコネクタを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f0e0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f0e0-130">Properties</span></span>
| <span data-ttu-id="1f0e0-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f0e0-131">Property</span></span>     | <span data-ttu-id="1f0e0-132">型</span><span class="sxs-lookup"><span data-stu-id="1f0e0-132">Type</span></span>   |<span data-ttu-id="1f0e0-133">説明</span><span class="sxs-lookup"><span data-stu-id="1f0e0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f0e0-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="1f0e0-134">connectorGroupType</span></span>|<span data-ttu-id="1f0e0-135">string</span><span class="sxs-lookup"><span data-stu-id="1f0e0-135">string</span></span>| <span data-ttu-id="1f0e0-136">グループで使用されるコネクタの種類。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="1f0e0-137">可能な値は`applicationProxy`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="1f0e0-138">id</span><span class="sxs-lookup"><span data-stu-id="1f0e0-138">id</span></span>|<span data-ttu-id="1f0e0-139">String</span><span class="sxs-lookup"><span data-stu-id="1f0e0-139">String</span></span>| <span data-ttu-id="1f0e0-140">コネクタグループのオブジェクト id</span><span class="sxs-lookup"><span data-stu-id="1f0e0-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="1f0e0-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="1f0e0-141">isDefault</span></span>|<span data-ttu-id="1f0e0-142">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1f0e0-142">Boolean</span></span>| <span data-ttu-id="1f0e0-143">コネクタグループが既定のコネクタグループであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="1f0e0-144">既定のコネクタグループにすることができ、システムによって設定されるのは、1つのコネクタグループのみです。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="1f0e0-145">name</span><span class="sxs-lookup"><span data-stu-id="1f0e0-145">name</span></span>|<span data-ttu-id="1f0e0-146">String</span><span class="sxs-lookup"><span data-stu-id="1f0e0-146">String</span></span>| <span data-ttu-id="1f0e0-147">コネクタグループに関連付けられている名前。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f0e0-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f0e0-148">Relationships</span></span>
| <span data-ttu-id="1f0e0-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f0e0-149">Relationship</span></span> | <span data-ttu-id="1f0e0-150">型</span><span class="sxs-lookup"><span data-stu-id="1f0e0-150">Type</span></span>   |<span data-ttu-id="1f0e0-151">説明</span><span class="sxs-lookup"><span data-stu-id="1f0e0-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f0e0-152">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f0e0-152">applications</span></span>|<span data-ttu-id="1f0e0-153">[アプリケーション](application.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f0e0-153">[application](application.md) collection</span></span>| <span data-ttu-id="1f0e0-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-154">Read-only.</span></span> <span data-ttu-id="1f0e0-155">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-155">Nullable.</span></span>|
|<span data-ttu-id="1f0e0-156">members</span><span class="sxs-lookup"><span data-stu-id="1f0e0-156">members</span></span>|<span data-ttu-id="1f0e0-157">[connector](connector.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f0e0-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="1f0e0-p105">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f0e0-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f0e0-160">JSON representation</span></span>

<span data-ttu-id="1f0e0-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f0e0-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
