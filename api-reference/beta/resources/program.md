---
title: program リソースの種類
description: 'Azure AD access のレビュー機能であるプログラムは、プログラムコントロールを保持するコンテナーです。 テナントには、1つ以上のプログラムを含めることができます。  各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563411"
---
# <a name="program-resource-type"></a><span data-ttu-id="ce066-105">program リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce066-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce066-106">Azure AD access の[レビュー](accessreviews-root.md)機能であるプログラムは、プログラムコントロールを保持するコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="ce066-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="ce066-107">テナントには、1つ以上のプログラムを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ce066-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="ce066-108">各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。</span><span class="sxs-lookup"><span data-stu-id="ce066-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="ce066-109">boarded Azure AD アクセスレビューを持つ各テナントには、 `Default program`1 つのプログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="ce066-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="ce066-110">グローバル管理者は、コンプライアンスイニシアチブを表すなど、追加のプログラムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="ce066-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="ce066-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce066-111">Methods</span></span>

| <span data-ttu-id="ce066-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce066-112">Method</span></span>           | <span data-ttu-id="ce066-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce066-113">Return Type</span></span>    |<span data-ttu-id="ce066-114">説明</span><span class="sxs-lookup"><span data-stu-id="ce066-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce066-115">プログラムを作成する</span><span class="sxs-lookup"><span data-stu-id="ce066-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="ce066-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce066-116">program</span></span>](program.md)   |   <span data-ttu-id="ce066-117">新しいプログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="ce066-117">Create a new program.</span></span>|
|[<span data-ttu-id="ce066-118">プログラムの削除</span><span class="sxs-lookup"><span data-stu-id="ce066-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="ce066-119">なし。</span><span class="sxs-lookup"><span data-stu-id="ce066-119">None.</span></span>   |   <span data-ttu-id="ce066-120">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="ce066-120">Delete a program.</span></span>|
|[<span data-ttu-id="ce066-121">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="ce066-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="ce066-122">[プログラム](program.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ce066-122">[program](program.md) collection</span></span>|   <span data-ttu-id="ce066-123">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ce066-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="ce066-124">プログラムの programcontrols を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ce066-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="ce066-125">[programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ce066-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="ce066-126">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ce066-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ce066-127">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="ce066-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="ce066-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce066-128">program</span></span>](program.md)|  <span data-ttu-id="ce066-129">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce066-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="ce066-130">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce066-130">Permissions</span></span>

|<span data-ttu-id="ce066-131">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce066-131">Permission type</span></span>                        | <span data-ttu-id="ce066-132">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce066-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce066-133">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce066-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce066-134">programcontrol. all、programcontrol.</span><span class="sxs-lookup"><span data-stu-id="ce066-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="ce066-135">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce066-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce066-136">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce066-136">Not supported.</span></span> |
|<span data-ttu-id="ce066-137">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce066-137">Application</span></span>                            | <span data-ttu-id="ce066-138">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce066-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="ce066-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce066-139">Properties</span></span>
| <span data-ttu-id="ce066-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce066-140">Property</span></span>     | <span data-ttu-id="ce066-141">型</span><span class="sxs-lookup"><span data-stu-id="ce066-141">Type</span></span>   |<span data-ttu-id="ce066-142">説明</span><span class="sxs-lookup"><span data-stu-id="ce066-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="ce066-143">プログラムの機能割り当て識別子。</span><span class="sxs-lookup"><span data-stu-id="ce066-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="ce066-144">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce066-144">The name of the program.</span></span>  <span data-ttu-id="ce066-145">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="ce066-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="ce066-146">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="ce066-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="ce066-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce066-147">Relationships</span></span>
| <span data-ttu-id="ce066-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce066-148">Relationship</span></span> | <span data-ttu-id="ce066-149">型</span><span class="sxs-lookup"><span data-stu-id="ce066-149">Type</span></span>   |<span data-ttu-id="ce066-150">説明</span><span class="sxs-lookup"><span data-stu-id="ce066-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="ce066-151">programcontrol</span><span class="sxs-lookup"><span data-stu-id="ce066-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="ce066-152">プログラムに関連付けられているコントロール。</span><span class="sxs-lookup"><span data-stu-id="ce066-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce066-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce066-153">JSON representation</span></span>

<span data-ttu-id="ce066-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce066-154">Here is a JSON representation of the resource.</span></span>

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
