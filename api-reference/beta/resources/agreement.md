---
title: 契約のリソースの種類
description: テナントのカスタマイズ可能な使用許諾契約書が作成され、Azure Active Directory (AD の Azure) を使用して管理する条件を表します。 機能を管理、Azure Active Directory の使用条件に従って、シナリオを作成し、次のメソッドを使用できます。
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513852"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="07006-104">契約のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="07006-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07006-105">テナントのカスタマイズ可能な使用許諾契約書が作成され、Azure Active Directory (AD の Azure) を使用して管理する条件を表します。</span><span class="sxs-lookup"><span data-stu-id="07006-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="07006-106">作成し、シナリオに基づく[Azure Active Directory の使用条件の機能](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)を管理するのには、次のメソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="07006-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="07006-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="07006-107">Methods</span></span>

| <span data-ttu-id="07006-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="07006-108">Method</span></span>       | <span data-ttu-id="07006-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="07006-109">Return Type</span></span> | <span data-ttu-id="07006-110">説明</span><span class="sxs-lookup"><span data-stu-id="07006-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="07006-111">契約書を作成します。</span><span class="sxs-lookup"><span data-stu-id="07006-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="07006-112">契約</span><span class="sxs-lookup"><span data-stu-id="07006-112">agreement</span></span>](agreement.md) | <span data-ttu-id="07006-113">契約コレクションへの投稿には、新しい契約を作成します。</span><span class="sxs-lookup"><span data-stu-id="07006-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="07006-114">リスト契約</span><span class="sxs-lookup"><span data-stu-id="07006-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="07006-115">[契約](agreement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="07006-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="07006-116">契約オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="07006-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="07006-117">契約を取得します。</span><span class="sxs-lookup"><span data-stu-id="07006-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="07006-118">契約</span><span class="sxs-lookup"><span data-stu-id="07006-118">agreement</span></span>](agreement.md) | <span data-ttu-id="07006-119">契約オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07006-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="07006-120">契約を更新します。</span><span class="sxs-lookup"><span data-stu-id="07006-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="07006-121">契約</span><span class="sxs-lookup"><span data-stu-id="07006-121">agreement</span></span>](agreement.md) | <span data-ttu-id="07006-122">契約オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="07006-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="07006-123">契約を削除します。</span><span class="sxs-lookup"><span data-stu-id="07006-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="07006-124">なし</span><span class="sxs-lookup"><span data-stu-id="07006-124">None</span></span> | <span data-ttu-id="07006-125">契約オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="07006-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="07006-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07006-126">Properties</span></span>
| <span data-ttu-id="07006-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07006-127">Property</span></span>     | <span data-ttu-id="07006-128">型</span><span class="sxs-lookup"><span data-stu-id="07006-128">Type</span></span>        | <span data-ttu-id="07006-129">説明</span><span class="sxs-lookup"><span data-stu-id="07006-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07006-130">displayName</span><span class="sxs-lookup"><span data-stu-id="07006-130">displayName</span></span>|<span data-ttu-id="07006-131">String</span><span class="sxs-lookup"><span data-stu-id="07006-131">String</span></span>|<span data-ttu-id="07006-132">契約書の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="07006-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="07006-133">id</span><span class="sxs-lookup"><span data-stu-id="07006-133">id</span></span>|<span data-ttu-id="07006-134">String</span><span class="sxs-lookup"><span data-stu-id="07006-134">String</span></span>| <span data-ttu-id="07006-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="07006-135">Read-only.</span></span>|
|<span data-ttu-id="07006-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="07006-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="07006-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="07006-137">Boolean</span></span>|<span data-ttu-id="07006-138">ユーザーを展開し、受け入れる前に契約書を表示するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="07006-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07006-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07006-139">Relationships</span></span>
| <span data-ttu-id="07006-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="07006-140">Relationship</span></span> | <span data-ttu-id="07006-141">型</span><span class="sxs-lookup"><span data-stu-id="07006-141">Type</span></span>        | <span data-ttu-id="07006-142">説明</span><span class="sxs-lookup"><span data-stu-id="07006-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07006-143">files</span><span class="sxs-lookup"><span data-stu-id="07006-143">files</span></span>|<span data-ttu-id="07006-144">[agreementFile](agreementfile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="07006-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="07006-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="07006-145">Read-only.</span></span> <span data-ttu-id="07006-146">Pdf は、本契約にリンクされています。</span><span class="sxs-lookup"><span data-stu-id="07006-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07006-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="07006-147">JSON representation</span></span>

<span data-ttu-id="07006-148">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="07006-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
