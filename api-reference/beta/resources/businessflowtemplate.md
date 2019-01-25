---
title: businessFlowTemplate リソースの種類
description: Azure AD にアクセス確認機能を`businesFlowTemplate`、Azure AD 業務フローのテンプレートを表します。 グループのゲスト メンバーを確認する場合など、テンプレートの識別子は、呼び出し元によって、アクセス確認を作成するときに提供されます。
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529580"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="7f4c0-104">businessFlowTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f4c0-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f4c0-105">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `businesFlowTemplate` 、Azure AD 業務フローのテンプレートを表します。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="7f4c0-106">グループのゲスト メンバーを確認する場合など、テンプレートの識別子は、呼び出し元によって、アクセス確認を作成するときに提供されます。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="7f4c0-107">業務フローのテンプレート オブジェクトは、グローバル管理者 onboards アクセスを使用するテナント機能を確認するときに自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="7f4c0-108">追加のビジネス フローのテンプレートは作成されません。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="7f4c0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f4c0-109">Methods</span></span>

| <span data-ttu-id="7f4c0-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f4c0-110">Method</span></span>           | <span data-ttu-id="7f4c0-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f4c0-111">Return Type</span></span>    |<span data-ttu-id="7f4c0-112">説明</span><span class="sxs-lookup"><span data-stu-id="7f4c0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f4c0-113">リスト businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="7f4c0-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="7f4c0-114">[businessFlowTemplate](businessflowtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7f4c0-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="7f4c0-115">レビューにアクセスする適切なビジネス フローのテンプレートを取得します。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f4c0-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f4c0-116">Properties</span></span>
| <span data-ttu-id="7f4c0-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f4c0-117">Property</span></span>     | <span data-ttu-id="7f4c0-118">型</span><span class="sxs-lookup"><span data-stu-id="7f4c0-118">Type</span></span>   |<span data-ttu-id="7f4c0-119">説明</span><span class="sxs-lookup"><span data-stu-id="7f4c0-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="7f4c0-120">業務フローのテンプレートの機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="7f4c0-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="7f4c0-121">業務フローのテンプレートの名前</span><span class="sxs-lookup"><span data-stu-id="7f4c0-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="7f4c0-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f4c0-122">Relationships</span></span>

<span data-ttu-id="7f4c0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="7f4c0-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="7f4c0-124">See also</span></span>

| <span data-ttu-id="7f4c0-125">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f4c0-125">Method</span></span>           | <span data-ttu-id="7f4c0-126">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f4c0-126">Return Type</span></span>    |<span data-ttu-id="7f4c0-127">説明</span><span class="sxs-lookup"><span data-stu-id="7f4c0-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f4c0-128">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="7f4c0-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="7f4c0-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="7f4c0-130">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7f4c0-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f4c0-131">JSON representation</span></span>

<span data-ttu-id="7f4c0-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f4c0-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
