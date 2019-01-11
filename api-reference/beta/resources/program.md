---
title: プログラムのリソースの種類
description: 'Azure AD にアクセスが機能を確認、プログラムは、プログラムのコントロールを保持しているコンテナーです。 テナントは、1 つまたは複数のプログラムを持つことができます。  各コントロールは、アクセス確認をプログラムにリンク、関連のアクセスを見つけやすくすることを確認します。  '
localization_priority: Normal
ms.openlocfilehash: a342fd159bba3f7e31c55ffab9a64a72353bc7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863904"
---
# <a name="program-resource-type"></a><span data-ttu-id="52ff2-105">プログラムのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="52ff2-105">program resource type</span></span>

> <span data-ttu-id="52ff2-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="52ff2-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52ff2-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52ff2-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52ff2-108">Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムは、プログラムのコントロールを保持している、コンテナーです。</span><span class="sxs-lookup"><span data-stu-id="52ff2-108">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="52ff2-109">テナントは、1 つまたは複数のプログラムを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="52ff2-109">A tenant can have one or more programs.</span></span>  <span data-ttu-id="52ff2-110">各コントロールは、アクセス確認をプログラムにリンク、関連のアクセスを見つけやすくすることを確認します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-110">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="52ff2-111">各テナントが上に直行し、Azure AD がアクセスのレビューには 1 つのプログラムでは、 `Default program`。</span><span class="sxs-lookup"><span data-stu-id="52ff2-111">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="52ff2-112">グローバル管理者は、コンプライアンス ・ イニシアティブを表現するなど、その他のプログラムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="52ff2-112">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="52ff2-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="52ff2-113">Methods</span></span>

| <span data-ttu-id="52ff2-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="52ff2-114">Method</span></span>           | <span data-ttu-id="52ff2-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="52ff2-115">Return Type</span></span>    |<span data-ttu-id="52ff2-116">説明</span><span class="sxs-lookup"><span data-stu-id="52ff2-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52ff2-117">プログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-117">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="52ff2-118">プログラム</span><span class="sxs-lookup"><span data-stu-id="52ff2-118">program</span></span>](program.md)   |   <span data-ttu-id="52ff2-119">新しいプログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-119">Create a new program.</span></span>|
|[<span data-ttu-id="52ff2-120">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-120">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="52ff2-121">なし。</span><span class="sxs-lookup"><span data-stu-id="52ff2-121">None.</span></span>   |   <span data-ttu-id="52ff2-122">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-122">Delete a program.</span></span>|
|[<span data-ttu-id="52ff2-123">プログラムを一覧表示</span><span class="sxs-lookup"><span data-stu-id="52ff2-123">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="52ff2-124">[プログラム](program.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="52ff2-124">[program](program.md) collection</span></span>|   <span data-ttu-id="52ff2-125">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-125">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="52ff2-126">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="52ff2-126">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="52ff2-127">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="52ff2-127">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="52ff2-128">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-128">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="52ff2-129">更新プログラム</span><span class="sxs-lookup"><span data-stu-id="52ff2-129">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="52ff2-130">プログラム</span><span class="sxs-lookup"><span data-stu-id="52ff2-130">program</span></span>](program.md)|  <span data-ttu-id="52ff2-131">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-131">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="52ff2-132">Permissions</span><span class="sxs-lookup"><span data-stu-id="52ff2-132">Permissions</span></span>

|<span data-ttu-id="52ff2-133">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52ff2-133">Permission type</span></span>                        | <span data-ttu-id="52ff2-134">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52ff2-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="52ff2-135">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52ff2-135">Delegated (work or school account)</span></span>     | <span data-ttu-id="52ff2-136">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52ff2-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="52ff2-137">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52ff2-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52ff2-138">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52ff2-138">Not supported.</span></span> |
|<span data-ttu-id="52ff2-139">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52ff2-139">Application</span></span>                            | <span data-ttu-id="52ff2-140">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52ff2-140">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="52ff2-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52ff2-141">Properties</span></span>
| <span data-ttu-id="52ff2-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52ff2-142">Property</span></span>     | <span data-ttu-id="52ff2-143">種類</span><span class="sxs-lookup"><span data-stu-id="52ff2-143">Type</span></span>   |<span data-ttu-id="52ff2-144">説明</span><span class="sxs-lookup"><span data-stu-id="52ff2-144">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="52ff2-145">プログラムの機能に割り当てられる識別子です。</span><span class="sxs-lookup"><span data-stu-id="52ff2-145">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="52ff2-146">プログラムの名前です。</span><span class="sxs-lookup"><span data-stu-id="52ff2-146">The name of the program.</span></span>  <span data-ttu-id="52ff2-147">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="52ff2-147">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="52ff2-148">プログラムの説明です。</span><span class="sxs-lookup"><span data-stu-id="52ff2-148">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="52ff2-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52ff2-149">Relationships</span></span>
| <span data-ttu-id="52ff2-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52ff2-150">Relationship</span></span> | <span data-ttu-id="52ff2-151">型</span><span class="sxs-lookup"><span data-stu-id="52ff2-151">Type</span></span>   |<span data-ttu-id="52ff2-152">説明</span><span class="sxs-lookup"><span data-stu-id="52ff2-152">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="52ff2-153">デバッギング</span><span class="sxs-lookup"><span data-stu-id="52ff2-153">programControl</span></span>](programcontrol.md) | <span data-ttu-id="52ff2-154">プログラムに関連付けられているコントロール。</span><span class="sxs-lookup"><span data-stu-id="52ff2-154">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52ff2-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52ff2-155">JSON representation</span></span>

<span data-ttu-id="52ff2-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52ff2-156">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
