---
title: connectorGroup リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517499"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="2fa0c-103">connectorGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2fa0c-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="2fa0c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fa0c-104">Methods</span></span>

| <span data-ttu-id="2fa0c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fa0c-105">Method</span></span>           | <span data-ttu-id="2fa0c-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2fa0c-106">Return Type</span></span>    |<span data-ttu-id="2fa0c-107">説明</span><span class="sxs-lookup"><span data-stu-id="2fa0c-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2fa0c-108">ConnectorGroup を取得します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="2fa0c-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="2fa0c-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="2fa0c-110">ConnectorGroup オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="2fa0c-111">アプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="2fa0c-112">application</span><span class="sxs-lookup"><span data-stu-id="2fa0c-112">application</span></span>](application.md)| <span data-ttu-id="2fa0c-113">コネクタ グループにアプリケーションを関連付けるアプリケーションのコレクションへの投稿。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="2fa0c-114">アプリケーション一覧</span><span class="sxs-lookup"><span data-stu-id="2fa0c-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="2fa0c-115">[アプリケーション](application.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fa0c-115">[application](application.md) collection</span></span>| <span data-ttu-id="2fa0c-116">関連付けられているアプリケーション オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="2fa0c-117">コネクタを作成します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="2fa0c-118">Connector</span><span class="sxs-lookup"><span data-stu-id="2fa0c-118">connector</span></span>](connector.md)| <span data-ttu-id="2fa0c-119">図形をグループ化するメンバーのコレクションへの投稿、コネクタを追加します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="2fa0c-120">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2fa0c-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="2fa0c-121">[コネクタ](connector.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="2fa0c-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="2fa0c-122">コネクタ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="2fa0c-123">Update</span><span class="sxs-lookup"><span data-stu-id="2fa0c-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="2fa0c-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="2fa0c-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="2fa0c-125">ConnectorGroup オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="2fa0c-126">Delete</span><span class="sxs-lookup"><span data-stu-id="2fa0c-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="2fa0c-127">なし</span><span class="sxs-lookup"><span data-stu-id="2fa0c-127">None</span></span> |<span data-ttu-id="2fa0c-128">ConnectorGroup オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-128">Delete connectorGroup object.</span></span> <span data-ttu-id="2fa0c-129">すべてのコネクタは、コネクタのグループを削除する前に削除をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="2fa0c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fa0c-130">Properties</span></span>
| <span data-ttu-id="2fa0c-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fa0c-131">Property</span></span>     | <span data-ttu-id="2fa0c-132">型</span><span class="sxs-lookup"><span data-stu-id="2fa0c-132">Type</span></span>   |<span data-ttu-id="2fa0c-133">説明</span><span class="sxs-lookup"><span data-stu-id="2fa0c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fa0c-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="2fa0c-134">connectorGroupType</span></span>|<span data-ttu-id="2fa0c-135">string</span><span class="sxs-lookup"><span data-stu-id="2fa0c-135">string</span></span>| <span data-ttu-id="2fa0c-136">グループで使用するコネクタの種類です。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="2fa0c-137">使用可能な値: `applicationProxy`。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="2fa0c-138">id</span><span class="sxs-lookup"><span data-stu-id="2fa0c-138">id</span></span>|<span data-ttu-id="2fa0c-139">String</span><span class="sxs-lookup"><span data-stu-id="2fa0c-139">String</span></span>| <span data-ttu-id="2fa0c-140">ConnectorGroup のオブジェクト id</span><span class="sxs-lookup"><span data-stu-id="2fa0c-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="2fa0c-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="2fa0c-141">isDefault</span></span>|<span data-ttu-id="2fa0c-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="2fa0c-142">Boolean</span></span>| <span data-ttu-id="2fa0c-143">ConnectorGroup がコネクタの既定のグループであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="2fa0c-144">のみ、1 つのコネクタ グループはデフォルトの connectorGroup をすることができ、システムによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="2fa0c-145">name</span><span class="sxs-lookup"><span data-stu-id="2fa0c-145">name</span></span>|<span data-ttu-id="2fa0c-146">String</span><span class="sxs-lookup"><span data-stu-id="2fa0c-146">String</span></span>| <span data-ttu-id="2fa0c-147">ConnectorGroup に関連付けられている名前です。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fa0c-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2fa0c-148">Relationships</span></span>
| <span data-ttu-id="2fa0c-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2fa0c-149">Relationship</span></span> | <span data-ttu-id="2fa0c-150">型</span><span class="sxs-lookup"><span data-stu-id="2fa0c-150">Type</span></span>   |<span data-ttu-id="2fa0c-151">説明</span><span class="sxs-lookup"><span data-stu-id="2fa0c-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fa0c-152">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2fa0c-152">applications</span></span>|<span data-ttu-id="2fa0c-153">[アプリケーション](application.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fa0c-153">[application](application.md) collection</span></span>| <span data-ttu-id="2fa0c-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="2fa0c-156">members</span><span class="sxs-lookup"><span data-stu-id="2fa0c-156">members</span></span>|<span data-ttu-id="2fa0c-157">[コネクタ](connector.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="2fa0c-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="2fa0c-p105">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2fa0c-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2fa0c-160">JSON representation</span></span>

<span data-ttu-id="2fa0c-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2fa0c-161">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
