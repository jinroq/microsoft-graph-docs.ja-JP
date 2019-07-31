---
title: アグリーメントリソースの種類
description: Azure Active Directory (Azure AD) で作成および管理されるテナントのカスタマイズ可能な利用規約を表します。 次のメソッドを使用すると、シナリオに従って、Azure Active Directory の使用条件の作成と管理を行うことができます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 31c25211efbca8ae0f52a9348ad0531ea818397f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974533"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="3e21b-104">アグリーメントリソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e21b-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e21b-105">Azure Active Directory (Azure AD) で作成および管理されるテナントのカスタマイズ可能な利用規約を表します。</span><span class="sxs-lookup"><span data-stu-id="3e21b-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="3e21b-106">次のメソッドを使用すると、シナリオに従って、 [Azure Active Directory の使用条件の](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)作成と管理を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="3e21b-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="3e21b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3e21b-107">Methods</span></span>

| <span data-ttu-id="3e21b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3e21b-108">Method</span></span>       | <span data-ttu-id="3e21b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3e21b-109">Return Type</span></span> | <span data-ttu-id="3e21b-110">説明</span><span class="sxs-lookup"><span data-stu-id="3e21b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e21b-111">契約の作成</span><span class="sxs-lookup"><span data-stu-id="3e21b-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="3e21b-112">保証</span><span class="sxs-lookup"><span data-stu-id="3e21b-112">agreement</span></span>](agreement.md) | <span data-ttu-id="3e21b-113">アグリーメントコレクションに投稿して、新しい契約を作成します。</span><span class="sxs-lookup"><span data-stu-id="3e21b-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="3e21b-114">契約を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3e21b-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="3e21b-115">[アグリーメント](agreement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3e21b-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="3e21b-116">アグリーメントオブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3e21b-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="3e21b-117">契約を取得する</span><span class="sxs-lookup"><span data-stu-id="3e21b-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="3e21b-118">保証</span><span class="sxs-lookup"><span data-stu-id="3e21b-118">agreement</span></span>](agreement.md) | <span data-ttu-id="3e21b-119">アグリーメントオブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3e21b-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="3e21b-120">契約を更新する</span><span class="sxs-lookup"><span data-stu-id="3e21b-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="3e21b-121">保証</span><span class="sxs-lookup"><span data-stu-id="3e21b-121">agreement</span></span>](agreement.md) | <span data-ttu-id="3e21b-122">アグリーメントオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3e21b-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="3e21b-123">契約を削除する</span><span class="sxs-lookup"><span data-stu-id="3e21b-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="3e21b-124">None</span><span class="sxs-lookup"><span data-stu-id="3e21b-124">None</span></span> | <span data-ttu-id="3e21b-125">アグリーメントオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="3e21b-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="3e21b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e21b-126">Properties</span></span>
| <span data-ttu-id="3e21b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e21b-127">Property</span></span>     | <span data-ttu-id="3e21b-128">型</span><span class="sxs-lookup"><span data-stu-id="3e21b-128">Type</span></span>        | <span data-ttu-id="3e21b-129">説明</span><span class="sxs-lookup"><span data-stu-id="3e21b-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e21b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="3e21b-130">displayName</span></span>|<span data-ttu-id="3e21b-131">String</span><span class="sxs-lookup"><span data-stu-id="3e21b-131">String</span></span>|<span data-ttu-id="3e21b-132">アグリーメントの表示名。</span><span class="sxs-lookup"><span data-stu-id="3e21b-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="3e21b-133">id</span><span class="sxs-lookup"><span data-stu-id="3e21b-133">id</span></span>|<span data-ttu-id="3e21b-134">String</span><span class="sxs-lookup"><span data-stu-id="3e21b-134">String</span></span>| <span data-ttu-id="3e21b-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3e21b-135">Read-only.</span></span>|
|<span data-ttu-id="3e21b-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="3e21b-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="3e21b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e21b-137">Boolean</span></span>|<span data-ttu-id="3e21b-138">ユーザーが同意する前に、契約を展開して表示する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3e21b-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e21b-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3e21b-139">Relationships</span></span>
| <span data-ttu-id="3e21b-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3e21b-140">Relationship</span></span> | <span data-ttu-id="3e21b-141">型</span><span class="sxs-lookup"><span data-stu-id="3e21b-141">Type</span></span>        | <span data-ttu-id="3e21b-142">説明</span><span class="sxs-lookup"><span data-stu-id="3e21b-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e21b-143">files</span><span class="sxs-lookup"><span data-stu-id="3e21b-143">files</span></span>|<span data-ttu-id="3e21b-144">[agreementFile](agreementfile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3e21b-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="3e21b-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3e21b-145">Read-only.</span></span> <span data-ttu-id="3e21b-146">このアグリーメントにリンクされている Pdf。</span><span class="sxs-lookup"><span data-stu-id="3e21b-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e21b-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e21b-147">JSON representation</span></span>

<span data-ttu-id="3e21b-148">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e21b-148">The following is a JSON representation of the resource.</span></span>

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
