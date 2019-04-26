---
title: programcontroltype リソースの種類
description: 'Azure AD access のレビュー機能では、プログラムにコントロールを関連付けるときにコントロールの種類としてコントロールを使用し、コントロールのアクセスレビューの種類を指定します。  '
localization_priority: Normal
ms.openlocfilehash: 489fa6e5cac31165fec9f7ce9939d58fa84cb1ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344060"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="4367f-103">programcontroltype リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4367f-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4367f-104">Azure AD access の[レビュー](accessreviews-root.md)機能では、プログラムにコントロールを関連付けるときにコントロールの種類としてコントロールを使用し、コントロールのアクセスレビューの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="4367f-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="4367f-105">プログラムコントロールの種類のオブジェクトは、グローバル管理者がテナントを介してアクセスレビュー機能を使用するときに自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="4367f-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="4367f-106">他のプログラムコントロールの種類を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="4367f-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="4367f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4367f-107">Methods</span></span>

| <span data-ttu-id="4367f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4367f-108">Method</span></span>           | <span data-ttu-id="4367f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4367f-109">Return Type</span></span>    |<span data-ttu-id="4367f-110">説明</span><span class="sxs-lookup"><span data-stu-id="4367f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4367f-111">programcontroltypes のリスト</span><span class="sxs-lookup"><span data-stu-id="4367f-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="4367f-112">[programcontroltype](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4367f-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="4367f-113">プログラムコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4367f-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="4367f-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4367f-114">Properties</span></span>
| <span data-ttu-id="4367f-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4367f-115">Property</span></span>     | <span data-ttu-id="4367f-116">型</span><span class="sxs-lookup"><span data-stu-id="4367f-116">Type</span></span>   |<span data-ttu-id="4367f-117">説明</span><span class="sxs-lookup"><span data-stu-id="4367f-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="4367f-118">プログラムコントロール型の機能割り当て識別子</span><span class="sxs-lookup"><span data-stu-id="4367f-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="4367f-119">プログラムコントロールの種類の名前。</span><span class="sxs-lookup"><span data-stu-id="4367f-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="4367f-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4367f-120">Relationships</span></span>

<span data-ttu-id="4367f-121">なし。</span><span class="sxs-lookup"><span data-stu-id="4367f-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="4367f-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="4367f-122">See also</span></span>

| <span data-ttu-id="4367f-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="4367f-123">Method</span></span>           | <span data-ttu-id="4367f-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4367f-124">Return Type</span></span>    |<span data-ttu-id="4367f-125">説明</span><span class="sxs-lookup"><span data-stu-id="4367f-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4367f-126">programcontrol を作成する</span><span class="sxs-lookup"><span data-stu-id="4367f-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="4367f-127">programcontrol</span><span class="sxs-lookup"><span data-stu-id="4367f-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="4367f-128">プログラムに programcontrol を追加します。</span><span class="sxs-lookup"><span data-stu-id="4367f-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4367f-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4367f-129">JSON representation</span></span>

<span data-ttu-id="4367f-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4367f-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
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
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
