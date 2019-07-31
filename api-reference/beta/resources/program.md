---
title: program リソースの種類
description: 'Azure AD access のレビュー機能であるプログラムは、プログラムコントロールを保持するコンテナーです。 テナントには、1つ以上のプログラムを含めることができます。  各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c6a978ef4bb68c09b2f5659e255d16681c9c805d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965671"
---
# <a name="program-resource-type"></a><span data-ttu-id="09ad0-105">program リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09ad0-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ad0-106">Azure AD access の[レビュー](accessreviews-root.md)機能であるプログラムは、プログラムコントロールを保持するコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="09ad0-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="09ad0-107">テナントには、1つ以上のプログラムを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="09ad0-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="09ad0-108">各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。</span><span class="sxs-lookup"><span data-stu-id="09ad0-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="09ad0-109">Boarded Azure AD アクセスレビューを持つ各テナントには、 `Default program`1 つのプログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="09ad0-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="09ad0-110">グローバル管理者は、コンプライアンスイニシアチブを表すなど、追加のプログラムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="09ad0-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="09ad0-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="09ad0-111">Methods</span></span>

| <span data-ttu-id="09ad0-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="09ad0-112">Method</span></span>           | <span data-ttu-id="09ad0-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09ad0-113">Return Type</span></span>    |<span data-ttu-id="09ad0-114">説明</span><span class="sxs-lookup"><span data-stu-id="09ad0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09ad0-115">プログラムを作成する</span><span class="sxs-lookup"><span data-stu-id="09ad0-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="09ad0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09ad0-116">program</span></span>](program.md)   |   <span data-ttu-id="09ad0-117">新しいプログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="09ad0-117">Create a new program.</span></span>|
|[<span data-ttu-id="09ad0-118">プログラムの削除</span><span class="sxs-lookup"><span data-stu-id="09ad0-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="09ad0-119">なし。</span><span class="sxs-lookup"><span data-stu-id="09ad0-119">None.</span></span>   |   <span data-ttu-id="09ad0-120">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="09ad0-120">Delete a program.</span></span>|
|[<span data-ttu-id="09ad0-121">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="09ad0-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="09ad0-122">[プログラム](program.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09ad0-122">[program](program.md) collection</span></span>|   <span data-ttu-id="09ad0-123">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="09ad0-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="09ad0-124">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="09ad0-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="09ad0-125">[Programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09ad0-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="09ad0-126">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="09ad0-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="09ad0-127">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="09ad0-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="09ad0-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09ad0-128">program</span></span>](program.md)|  <span data-ttu-id="09ad0-129">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="09ad0-129">Update a program.</span></span>|

## <a name="properties"></a><span data-ttu-id="09ad0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09ad0-130">Properties</span></span>
| <span data-ttu-id="09ad0-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09ad0-131">Property</span></span>     | <span data-ttu-id="09ad0-132">型</span><span class="sxs-lookup"><span data-stu-id="09ad0-132">Type</span></span>   |<span data-ttu-id="09ad0-133">説明</span><span class="sxs-lookup"><span data-stu-id="09ad0-133">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="09ad0-134">プログラムの機能割り当て識別子。</span><span class="sxs-lookup"><span data-stu-id="09ad0-134">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="09ad0-135">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="09ad0-135">The name of the program.</span></span>  <span data-ttu-id="09ad0-136">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="09ad0-136">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="09ad0-137">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="09ad0-137">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="09ad0-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09ad0-138">Relationships</span></span>
| <span data-ttu-id="09ad0-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09ad0-139">Relationship</span></span> | <span data-ttu-id="09ad0-140">型</span><span class="sxs-lookup"><span data-stu-id="09ad0-140">Type</span></span>   |<span data-ttu-id="09ad0-141">説明</span><span class="sxs-lookup"><span data-stu-id="09ad0-141">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="09ad0-142">programControl</span><span class="sxs-lookup"><span data-stu-id="09ad0-142">programControl</span></span>](programcontrol.md) | <span data-ttu-id="09ad0-143">プログラムに関連付けられているコントロール。</span><span class="sxs-lookup"><span data-stu-id="09ad0-143">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09ad0-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09ad0-144">JSON representation</span></span>

<span data-ttu-id="09ad0-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09ad0-145">Here is a JSON representation of the resource.</span></span>

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
