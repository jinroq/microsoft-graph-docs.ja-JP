---
title: アグリーメントリソースの種類
description: azure Active Directory (azure AD) で作成および管理されるテナントのカスタマイズ可能な利用規約を表します。 次のメソッドを使用すると、シナリオに従って、Azure Active Directory の使用条件の作成と管理を行うことができます。
localization_priority: Normal
ms.openlocfilehash: d91cc8f8180ffb706639fb42a8c68d711991602c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339175"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="fd9ed-104">アグリーメントリソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd9ed-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd9ed-105">azure Active Directory (azure AD) で作成および管理されるテナントのカスタマイズ可能な利用規約を表します。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="fd9ed-106">次のメソッドを使用すると、シナリオに従って、 [Azure Active Directory の使用条件の](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)作成と管理を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="fd9ed-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd9ed-107">Methods</span></span>

| <span data-ttu-id="fd9ed-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd9ed-108">Method</span></span>       | <span data-ttu-id="fd9ed-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fd9ed-109">Return Type</span></span> | <span data-ttu-id="fd9ed-110">説明</span><span class="sxs-lookup"><span data-stu-id="fd9ed-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fd9ed-111">契約の作成</span><span class="sxs-lookup"><span data-stu-id="fd9ed-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="fd9ed-112">保証</span><span class="sxs-lookup"><span data-stu-id="fd9ed-112">agreement</span></span>](agreement.md) | <span data-ttu-id="fd9ed-113">アグリーメントコレクションに投稿して、新しい契約を作成します。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="fd9ed-114">契約を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fd9ed-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="fd9ed-115">[アグリーメント](agreement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fd9ed-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="fd9ed-116">アグリーメントオブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="fd9ed-117">契約を取得する</span><span class="sxs-lookup"><span data-stu-id="fd9ed-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="fd9ed-118">保証</span><span class="sxs-lookup"><span data-stu-id="fd9ed-118">agreement</span></span>](agreement.md) | <span data-ttu-id="fd9ed-119">アグリーメントオブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="fd9ed-120">契約を更新する</span><span class="sxs-lookup"><span data-stu-id="fd9ed-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="fd9ed-121">保証</span><span class="sxs-lookup"><span data-stu-id="fd9ed-121">agreement</span></span>](agreement.md) | <span data-ttu-id="fd9ed-122">アグリーメントオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="fd9ed-123">契約を削除する</span><span class="sxs-lookup"><span data-stu-id="fd9ed-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="fd9ed-124">なし</span><span class="sxs-lookup"><span data-stu-id="fd9ed-124">None</span></span> | <span data-ttu-id="fd9ed-125">アグリーメントオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="fd9ed-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd9ed-126">Properties</span></span>
| <span data-ttu-id="fd9ed-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd9ed-127">Property</span></span>     | <span data-ttu-id="fd9ed-128">型</span><span class="sxs-lookup"><span data-stu-id="fd9ed-128">Type</span></span>        | <span data-ttu-id="fd9ed-129">説明</span><span class="sxs-lookup"><span data-stu-id="fd9ed-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd9ed-130">displayName</span><span class="sxs-lookup"><span data-stu-id="fd9ed-130">displayName</span></span>|<span data-ttu-id="fd9ed-131">String</span><span class="sxs-lookup"><span data-stu-id="fd9ed-131">String</span></span>|<span data-ttu-id="fd9ed-132">アグリーメントの表示名。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="fd9ed-133">id</span><span class="sxs-lookup"><span data-stu-id="fd9ed-133">id</span></span>|<span data-ttu-id="fd9ed-134">String</span><span class="sxs-lookup"><span data-stu-id="fd9ed-134">String</span></span>| <span data-ttu-id="fd9ed-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-135">Read-only.</span></span>|
|<span data-ttu-id="fd9ed-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="fd9ed-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="fd9ed-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd9ed-137">Boolean</span></span>|<span data-ttu-id="fd9ed-138">ユーザーが同意する前に、契約を展開して表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd9ed-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd9ed-139">Relationships</span></span>
| <span data-ttu-id="fd9ed-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd9ed-140">Relationship</span></span> | <span data-ttu-id="fd9ed-141">型</span><span class="sxs-lookup"><span data-stu-id="fd9ed-141">Type</span></span>        | <span data-ttu-id="fd9ed-142">説明</span><span class="sxs-lookup"><span data-stu-id="fd9ed-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd9ed-143">files</span><span class="sxs-lookup"><span data-stu-id="fd9ed-143">files</span></span>|<span data-ttu-id="fd9ed-144">[agreementFile](agreementfile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fd9ed-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="fd9ed-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-145">Read-only.</span></span> <span data-ttu-id="fd9ed-146">このアグリーメントにリンクされている pdf。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd9ed-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd9ed-147">JSON representation</span></span>

<span data-ttu-id="fd9ed-148">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd9ed-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
