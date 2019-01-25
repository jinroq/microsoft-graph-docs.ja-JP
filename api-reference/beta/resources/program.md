---
title: プログラムのリソースの種類
description: 'Azure AD にアクセスが機能を確認、プログラムは、プログラムのコントロールを保持しているコンテナーです。 テナントは、1 つまたは複数のプログラムを持つことができます。  各コントロールは、アクセス確認をプログラムにリンク、関連のアクセスを見つけやすくすることを確認します。  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515189"
---
# <a name="program-resource-type"></a><span data-ttu-id="706dd-105">プログラムのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="706dd-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="706dd-106">Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムは、プログラムのコントロールを保持している、コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="706dd-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="706dd-107">テナントは、1 つまたは複数のプログラムを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="706dd-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="706dd-108">各コントロールは、アクセス確認をプログラムにリンク、関連のアクセスを見つけやすくすることを確認します。</span><span class="sxs-lookup"><span data-stu-id="706dd-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="706dd-109">各テナントが上に直行し、Azure AD がアクセスのレビューには 1 つのプログラムでは、 `Default program`。</span><span class="sxs-lookup"><span data-stu-id="706dd-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="706dd-110">グローバル管理者は、コンプライアンス ・ イニシアティブを表現するなど、その他のプログラムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="706dd-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="706dd-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="706dd-111">Methods</span></span>

| <span data-ttu-id="706dd-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="706dd-112">Method</span></span>           | <span data-ttu-id="706dd-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="706dd-113">Return Type</span></span>    |<span data-ttu-id="706dd-114">説明</span><span class="sxs-lookup"><span data-stu-id="706dd-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="706dd-115">プログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="706dd-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="706dd-116">プログラム</span><span class="sxs-lookup"><span data-stu-id="706dd-116">program</span></span>](program.md)   |   <span data-ttu-id="706dd-117">新しいプログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="706dd-117">Create a new program.</span></span>|
|[<span data-ttu-id="706dd-118">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="706dd-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="706dd-119">なし。</span><span class="sxs-lookup"><span data-stu-id="706dd-119">None.</span></span>   |   <span data-ttu-id="706dd-120">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="706dd-120">Delete a program.</span></span>|
|[<span data-ttu-id="706dd-121">プログラムを一覧表示</span><span class="sxs-lookup"><span data-stu-id="706dd-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="706dd-122">[プログラム](program.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="706dd-122">[program](program.md) collection</span></span>|   <span data-ttu-id="706dd-123">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="706dd-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="706dd-124">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="706dd-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="706dd-125">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="706dd-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="706dd-126">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="706dd-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="706dd-127">更新プログラム</span><span class="sxs-lookup"><span data-stu-id="706dd-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="706dd-128">プログラム</span><span class="sxs-lookup"><span data-stu-id="706dd-128">program</span></span>](program.md)|  <span data-ttu-id="706dd-129">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="706dd-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="706dd-130">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="706dd-130">Permissions</span></span>

|<span data-ttu-id="706dd-131">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="706dd-131">Permission type</span></span>                        | <span data-ttu-id="706dd-132">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="706dd-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="706dd-133">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="706dd-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="706dd-134">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="706dd-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="706dd-135">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="706dd-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="706dd-136">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="706dd-136">Not supported.</span></span> |
|<span data-ttu-id="706dd-137">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="706dd-137">Application</span></span>                            | <span data-ttu-id="706dd-138">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="706dd-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="706dd-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="706dd-139">Properties</span></span>
| <span data-ttu-id="706dd-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="706dd-140">Property</span></span>     | <span data-ttu-id="706dd-141">型</span><span class="sxs-lookup"><span data-stu-id="706dd-141">Type</span></span>   |<span data-ttu-id="706dd-142">説明</span><span class="sxs-lookup"><span data-stu-id="706dd-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="706dd-143">プログラムの機能に割り当てられる識別子です。</span><span class="sxs-lookup"><span data-stu-id="706dd-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="706dd-144">プログラムの名前です。</span><span class="sxs-lookup"><span data-stu-id="706dd-144">The name of the program.</span></span>  <span data-ttu-id="706dd-145">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="706dd-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="706dd-146">プログラムの説明です。</span><span class="sxs-lookup"><span data-stu-id="706dd-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="706dd-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="706dd-147">Relationships</span></span>
| <span data-ttu-id="706dd-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="706dd-148">Relationship</span></span> | <span data-ttu-id="706dd-149">型</span><span class="sxs-lookup"><span data-stu-id="706dd-149">Type</span></span>   |<span data-ttu-id="706dd-150">説明</span><span class="sxs-lookup"><span data-stu-id="706dd-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="706dd-151">デバッギング</span><span class="sxs-lookup"><span data-stu-id="706dd-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="706dd-152">プログラムに関連付けられているコントロール。</span><span class="sxs-lookup"><span data-stu-id="706dd-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="706dd-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="706dd-153">JSON representation</span></span>

<span data-ttu-id="706dd-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="706dd-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
