---
title: program リソースの種類
description: 'Azure AD access のレビュー機能であるプログラムは、プログラムコントロールを保持するコンテナーです。 テナントには、1つ以上のプログラムを含めることができます。  各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。  '
localization_priority: Normal
ms.openlocfilehash: 7c0016cb194acd7ad8533acb34650b57df720ace
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344030"
---
# <a name="program-resource-type"></a><span data-ttu-id="3387f-105">program リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3387f-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3387f-106">Azure AD access の[レビュー](accessreviews-root.md)機能であるプログラムは、プログラムコントロールを保持するコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="3387f-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="3387f-107">テナントには、1つ以上のプログラムを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3387f-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="3387f-108">各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。</span><span class="sxs-lookup"><span data-stu-id="3387f-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="3387f-109">boarded Azure AD アクセスレビューを持つ各テナントには、 `Default program`1 つのプログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="3387f-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="3387f-110">グローバル管理者は、コンプライアンスイニシアチブを表すなど、追加のプログラムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="3387f-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="3387f-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="3387f-111">Methods</span></span>

| <span data-ttu-id="3387f-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="3387f-112">Method</span></span>           | <span data-ttu-id="3387f-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3387f-113">Return Type</span></span>    |<span data-ttu-id="3387f-114">説明</span><span class="sxs-lookup"><span data-stu-id="3387f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3387f-115">プログラムを作成する</span><span class="sxs-lookup"><span data-stu-id="3387f-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="3387f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3387f-116">program</span></span>](program.md)   |   <span data-ttu-id="3387f-117">新しいプログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="3387f-117">Create a new program.</span></span>|
|[<span data-ttu-id="3387f-118">プログラムの削除</span><span class="sxs-lookup"><span data-stu-id="3387f-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="3387f-119">なし。</span><span class="sxs-lookup"><span data-stu-id="3387f-119">None.</span></span>   |   <span data-ttu-id="3387f-120">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="3387f-120">Delete a program.</span></span>|
|[<span data-ttu-id="3387f-121">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="3387f-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="3387f-122">[プログラム](program.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3387f-122">[program](program.md) collection</span></span>|   <span data-ttu-id="3387f-123">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3387f-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="3387f-124">プログラムの programcontrols を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3387f-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="3387f-125">[programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3387f-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="3387f-126">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3387f-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="3387f-127">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="3387f-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="3387f-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3387f-128">program</span></span>](program.md)|  <span data-ttu-id="3387f-129">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="3387f-129">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="3387f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3387f-130">Properties</span></span>
| <span data-ttu-id="3387f-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3387f-131">Property</span></span>     | <span data-ttu-id="3387f-132">型</span><span class="sxs-lookup"><span data-stu-id="3387f-132">Type</span></span>   |<span data-ttu-id="3387f-133">説明</span><span class="sxs-lookup"><span data-stu-id="3387f-133">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="3387f-134">プログラムの機能割り当て識別子。</span><span class="sxs-lookup"><span data-stu-id="3387f-134">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="3387f-135">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3387f-135">The name of the program.</span></span>  <span data-ttu-id="3387f-136">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="3387f-136">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="3387f-137">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="3387f-137">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="3387f-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3387f-138">Relationships</span></span>
| <span data-ttu-id="3387f-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3387f-139">Relationship</span></span> | <span data-ttu-id="3387f-140">型</span><span class="sxs-lookup"><span data-stu-id="3387f-140">Type</span></span>   |<span data-ttu-id="3387f-141">説明</span><span class="sxs-lookup"><span data-stu-id="3387f-141">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="3387f-142">programcontrol</span><span class="sxs-lookup"><span data-stu-id="3387f-142">programControl</span></span>](programcontrol.md) | <span data-ttu-id="3387f-143">プログラムに関連付けられているコントロール。</span><span class="sxs-lookup"><span data-stu-id="3387f-143">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3387f-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3387f-144">JSON representation</span></span>

<span data-ttu-id="3387f-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3387f-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
