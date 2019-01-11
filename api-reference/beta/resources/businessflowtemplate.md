---
title: businessFlowTemplate リソースの種類
description: Azure AD にアクセス確認機能を`businesFlowTemplate`、Azure AD 業務フローのテンプレートを表します。 グループのゲスト メンバーを確認する場合など、テンプレートの識別子は、呼び出し元によって、アクセス確認を作成するときに提供されます。
localization_priority: Normal
ms.openlocfilehash: cad361d6c2d2aba70b2623ddf272e1eba42fd93b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889027"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="f64f3-104">businessFlowTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f64f3-104">businessFlowTemplate resource type</span></span>

> <span data-ttu-id="f64f3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f64f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f64f3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f64f3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f64f3-107">Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `businesFlowTemplate` 、Azure AD 業務フローのテンプレートを表します。</span><span class="sxs-lookup"><span data-stu-id="f64f3-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="f64f3-108">グループのゲスト メンバーを確認する場合など、テンプレートの識別子は、呼び出し元によって、アクセス確認を作成するときに提供されます。</span><span class="sxs-lookup"><span data-stu-id="f64f3-108">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="f64f3-109">業務フローのテンプレート オブジェクトは、グローバル管理者 onboards アクセスを使用するテナント機能を確認するときに自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="f64f3-109">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="f64f3-110">追加のビジネス フローのテンプレートは作成されません。</span><span class="sxs-lookup"><span data-stu-id="f64f3-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="f64f3-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="f64f3-111">Methods</span></span>

| <span data-ttu-id="f64f3-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="f64f3-112">Method</span></span>           | <span data-ttu-id="f64f3-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f64f3-113">Return Type</span></span>    |<span data-ttu-id="f64f3-114">説明</span><span class="sxs-lookup"><span data-stu-id="f64f3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f64f3-115">リスト businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="f64f3-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="f64f3-116">[businessFlowTemplate](businessflowtemplate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f64f3-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="f64f3-117">レビューにアクセスする適切なビジネス フローのテンプレートを取得します。</span><span class="sxs-lookup"><span data-stu-id="f64f3-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="f64f3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f64f3-118">Properties</span></span>
| <span data-ttu-id="f64f3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f64f3-119">Property</span></span>     | <span data-ttu-id="f64f3-120">種類</span><span class="sxs-lookup"><span data-stu-id="f64f3-120">Type</span></span>   |<span data-ttu-id="f64f3-121">説明</span><span class="sxs-lookup"><span data-stu-id="f64f3-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f64f3-122">業務フローのテンプレートの機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="f64f3-122">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="f64f3-123">業務フローのテンプレートの名前</span><span class="sxs-lookup"><span data-stu-id="f64f3-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="f64f3-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f64f3-124">Relationships</span></span>

<span data-ttu-id="f64f3-125">なし。</span><span class="sxs-lookup"><span data-stu-id="f64f3-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="f64f3-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="f64f3-126">See also</span></span>

| <span data-ttu-id="f64f3-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="f64f3-127">Method</span></span>           | <span data-ttu-id="f64f3-128">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f64f3-128">Return Type</span></span>    |<span data-ttu-id="f64f3-129">説明</span><span class="sxs-lookup"><span data-stu-id="f64f3-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f64f3-130">AccessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="f64f3-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="f64f3-131">accessReview</span><span class="sxs-lookup"><span data-stu-id="f64f3-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="f64f3-132">新しい accessReview を作成します。</span><span class="sxs-lookup"><span data-stu-id="f64f3-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f64f3-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f64f3-133">JSON representation</span></span>

<span data-ttu-id="f64f3-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f64f3-134">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
