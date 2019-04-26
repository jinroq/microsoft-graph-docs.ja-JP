---
title: businessflowtemplate リソースの種類
description: azure ad access レビュー機能では、は`businesFlowTemplate` azure ad ビジネスフローテンプレートを表します。 グループのゲストメンバーを確認するなどのテンプレートの識別子は、アクセスレビューを作成するときに発信者によって提供されます。
localization_priority: Normal
ms.openlocfilehash: 0cca72bc8ccd372cdaf9952b385bc63f81b0631d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338831"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="f2c6c-104">businessflowtemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2c6c-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c6c-105">azure ad [access レビュー](accessreviews-root.md)機能では、は`businesFlowTemplate` azure ad ビジネスフローテンプレートを表します。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="f2c6c-106">グループのゲストメンバーを確認するなどのテンプレートの識別子は、アクセスレビューを作成するときに発信者によって提供されます。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="f2c6c-107">ビジネスフローテンプレートオブジェクトは、グローバル管理者がテナントを介してアクセスレビュー機能を使用すると、自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="f2c6c-108">追加のビジネスフローテンプレートを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="f2c6c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2c6c-109">Methods</span></span>

| <span data-ttu-id="f2c6c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2c6c-110">Method</span></span>           | <span data-ttu-id="f2c6c-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2c6c-111">Return Type</span></span>    |<span data-ttu-id="f2c6c-112">説明</span><span class="sxs-lookup"><span data-stu-id="f2c6c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2c6c-113">businessflowtemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f2c6c-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="f2c6c-114">[businessflowtemplate](businessflowtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f2c6c-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="f2c6c-115">レビューにアクセスするための適切なビジネスフローテンプレートを取得します。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2c6c-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2c6c-116">Properties</span></span>
| <span data-ttu-id="f2c6c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2c6c-117">Property</span></span>     | <span data-ttu-id="f2c6c-118">型</span><span class="sxs-lookup"><span data-stu-id="f2c6c-118">Type</span></span>   |<span data-ttu-id="f2c6c-119">説明</span><span class="sxs-lookup"><span data-stu-id="f2c6c-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f2c6c-120">ビジネスフローテンプレートの機能割り当て識別子</span><span class="sxs-lookup"><span data-stu-id="f2c6c-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="f2c6c-121">ビジネスフローテンプレートの名前</span><span class="sxs-lookup"><span data-stu-id="f2c6c-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="f2c6c-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2c6c-122">Relationships</span></span>

<span data-ttu-id="f2c6c-123">なし。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="f2c6c-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2c6c-124">See also</span></span>

| <span data-ttu-id="f2c6c-125">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2c6c-125">Method</span></span>           | <span data-ttu-id="f2c6c-126">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2c6c-126">Return Type</span></span>    |<span data-ttu-id="f2c6c-127">説明</span><span class="sxs-lookup"><span data-stu-id="f2c6c-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2c6c-128">accessreview を作成する</span><span class="sxs-lookup"><span data-stu-id="f2c6c-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="f2c6c-129">accessreview</span><span class="sxs-lookup"><span data-stu-id="f2c6c-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="f2c6c-130">新しい accessreview を作成します。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f2c6c-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2c6c-131">JSON representation</span></span>

<span data-ttu-id="f2c6c-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2c6c-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
