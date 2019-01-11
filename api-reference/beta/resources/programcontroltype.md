---
title: programControlType リソースの種類
description: 'Azure AD にアクセスが機能を確認、アクセス確認の種類を示すために、プログラムにコントロールをコントロールに関連付けることが、ときにプログラムのコントロールの種類を使用します。  '
localization_priority: Normal
ms.openlocfilehash: 0091c23fd5d537e7c1fd62051778e56b510a3dab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808233"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="f5caa-103">programControlType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5caa-103">programControlType resource type</span></span>

> <span data-ttu-id="f5caa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5caa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5caa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5caa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5caa-106">機能では、Azure AD[アクセスの確認](accessreviews-root.md)は、プログラムのコントロールの種類はコントロールは、アクセス確認の種類を示すためにも、プログラムにコントロールを関連付ける場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f5caa-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="f5caa-107">プログラムのコントロール型オブジェクトは、グローバル管理者 onboards アクセスを使用するテナント機能を確認するときに自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="f5caa-107">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="f5caa-108">コントロールの種類を追加したプログラムは作成されません。</span><span class="sxs-lookup"><span data-stu-id="f5caa-108">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="f5caa-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5caa-109">Methods</span></span>

| <span data-ttu-id="f5caa-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5caa-110">Method</span></span>           | <span data-ttu-id="f5caa-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5caa-111">Return Type</span></span>    |<span data-ttu-id="f5caa-112">説明</span><span class="sxs-lookup"><span data-stu-id="f5caa-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5caa-113">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="f5caa-113">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="f5caa-114">[programControlType](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f5caa-114">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="f5caa-115">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f5caa-115">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="f5caa-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5caa-116">Properties</span></span>
| <span data-ttu-id="f5caa-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5caa-117">Property</span></span>     | <span data-ttu-id="f5caa-118">種類</span><span class="sxs-lookup"><span data-stu-id="f5caa-118">Type</span></span>   |<span data-ttu-id="f5caa-119">説明</span><span class="sxs-lookup"><span data-stu-id="f5caa-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="f5caa-120">プログラムのコントロールの種類の機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="f5caa-120">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="f5caa-121">プログラムのコントロールの種類の名前</span><span class="sxs-lookup"><span data-stu-id="f5caa-121">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="f5caa-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5caa-122">Relationships</span></span>

<span data-ttu-id="f5caa-123">なし。</span><span class="sxs-lookup"><span data-stu-id="f5caa-123">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="f5caa-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5caa-124">See also</span></span>

| <span data-ttu-id="f5caa-125">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5caa-125">Method</span></span>           | <span data-ttu-id="f5caa-126">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5caa-126">Return Type</span></span>    |<span data-ttu-id="f5caa-127">説明</span><span class="sxs-lookup"><span data-stu-id="f5caa-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5caa-128">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="f5caa-128">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="f5caa-129">デバッギング</span><span class="sxs-lookup"><span data-stu-id="f5caa-129">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="f5caa-130">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="f5caa-130">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f5caa-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5caa-131">JSON representation</span></span>

<span data-ttu-id="f5caa-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5caa-132">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
