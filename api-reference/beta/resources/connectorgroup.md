---
title: connectorGroup リソースの種類
description: 以下は、リソースの JSON 表記です。
ms.openlocfilehash: a3131b887216f1f400f70ed8d607477f65793cc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071541"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="092bb-103">connectorGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="092bb-103">connectorGroup resource type</span></span>

> <span data-ttu-id="092bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="092bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="092bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="092bb-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="methods"></a><span data-ttu-id="092bb-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="092bb-106">Methods</span></span>

| <span data-ttu-id="092bb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="092bb-107">Method</span></span>           | <span data-ttu-id="092bb-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="092bb-108">Return Type</span></span>    |<span data-ttu-id="092bb-109">説明</span><span class="sxs-lookup"><span data-stu-id="092bb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="092bb-110">ConnectorGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="092bb-110">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="092bb-111">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="092bb-111">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="092bb-112">ConnectorGroup オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="092bb-112">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="092bb-113">アプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="092bb-113">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="092bb-114">application</span><span class="sxs-lookup"><span data-stu-id="092bb-114">application</span></span>](application.md)| <span data-ttu-id="092bb-115">コネクタ グループにアプリケーションを関連付けるアプリケーションのコレクションへの投稿。</span><span class="sxs-lookup"><span data-stu-id="092bb-115">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="092bb-116">アプリケーション一覧</span><span class="sxs-lookup"><span data-stu-id="092bb-116">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="092bb-117">[アプリケーション](application.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="092bb-117">[application](application.md) collection</span></span>| <span data-ttu-id="092bb-118">関連付けられているアプリケーション オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="092bb-118">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="092bb-119">コネクタを作成します。</span><span class="sxs-lookup"><span data-stu-id="092bb-119">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="092bb-120">コネクタ</span><span class="sxs-lookup"><span data-stu-id="092bb-120">connector</span></span>](connector.md)| <span data-ttu-id="092bb-121">図形をグループ化するメンバーのコレクションへの投稿、コネクタを追加します。</span><span class="sxs-lookup"><span data-stu-id="092bb-121">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="092bb-122">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="092bb-122">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="092bb-123">[コネクタ](connector.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="092bb-123">[connector](connector.md) collection</span></span>| <span data-ttu-id="092bb-124">コネクタ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="092bb-124">Get a connector object collection.</span></span>|
|[<span data-ttu-id="092bb-125">Update</span><span class="sxs-lookup"><span data-stu-id="092bb-125">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="092bb-126">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="092bb-126">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="092bb-127">ConnectorGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="092bb-127">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="092bb-128">削除</span><span class="sxs-lookup"><span data-stu-id="092bb-128">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="092bb-129">なし</span><span class="sxs-lookup"><span data-stu-id="092bb-129">None</span></span> |<span data-ttu-id="092bb-130">ConnectorGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="092bb-130">Delete connectorGroup object.</span></span> <span data-ttu-id="092bb-131">すべてのコネクタは、コネクタのグループを削除する前に削除をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="092bb-131">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="092bb-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="092bb-132">Properties</span></span>
| <span data-ttu-id="092bb-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="092bb-133">Property</span></span>     | <span data-ttu-id="092bb-134">型</span><span class="sxs-lookup"><span data-stu-id="092bb-134">Type</span></span>   |<span data-ttu-id="092bb-135">説明</span><span class="sxs-lookup"><span data-stu-id="092bb-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="092bb-136">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="092bb-136">connectorGroupType</span></span>|<span data-ttu-id="092bb-137">文字列</span><span class="sxs-lookup"><span data-stu-id="092bb-137">string</span></span>| <span data-ttu-id="092bb-138">グループで使用するコネクタの種類です。</span><span class="sxs-lookup"><span data-stu-id="092bb-138">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="092bb-139">使用可能な値: `applicationProxy`。</span><span class="sxs-lookup"><span data-stu-id="092bb-139">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="092bb-140">id</span><span class="sxs-lookup"><span data-stu-id="092bb-140">id</span></span>|<span data-ttu-id="092bb-141">String</span><span class="sxs-lookup"><span data-stu-id="092bb-141">String</span></span>| <span data-ttu-id="092bb-142">ConnectorGroup のオブジェクト id</span><span class="sxs-lookup"><span data-stu-id="092bb-142">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="092bb-143">isDefault</span><span class="sxs-lookup"><span data-stu-id="092bb-143">isDefault</span></span>|<span data-ttu-id="092bb-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="092bb-144">Boolean</span></span>| <span data-ttu-id="092bb-145">ConnectorGroup がコネクタの既定のグループであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="092bb-145">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="092bb-146">のみ、1 つのコネクタ グループはデフォルトの connectorGroup をすることができ、システムによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="092bb-146">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="092bb-147">名前</span><span class="sxs-lookup"><span data-stu-id="092bb-147">name</span></span>|<span data-ttu-id="092bb-148">String</span><span class="sxs-lookup"><span data-stu-id="092bb-148">String</span></span>| <span data-ttu-id="092bb-149">ConnectorGroup に関連付けられている名前です。</span><span class="sxs-lookup"><span data-stu-id="092bb-149">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="092bb-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="092bb-150">Relationships</span></span>
| <span data-ttu-id="092bb-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="092bb-151">Relationship</span></span> | <span data-ttu-id="092bb-152">型</span><span class="sxs-lookup"><span data-stu-id="092bb-152">Type</span></span>   |<span data-ttu-id="092bb-153">説明</span><span class="sxs-lookup"><span data-stu-id="092bb-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="092bb-154">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="092bb-154">applications</span></span>|<span data-ttu-id="092bb-155">[アプリケーション](application.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="092bb-155">[application](application.md) collection</span></span>| <span data-ttu-id="092bb-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="092bb-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="092bb-158">メンバー</span><span class="sxs-lookup"><span data-stu-id="092bb-158">members</span></span>|<span data-ttu-id="092bb-159">[コネクタ](connector.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="092bb-159">[connector](connector.md) collection</span></span>| <span data-ttu-id="092bb-p106">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="092bb-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="092bb-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="092bb-162">JSON representation</span></span>

<span data-ttu-id="092bb-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="092bb-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->