---
title: デバッギングのリソースの種類
description: Azure AD にアクセスが機能を確認、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンクするコントロールを表します。
localization_priority: Normal
ms.openlocfilehash: 82d9263a909fb11e688ffa6b27f0cf92601ae9e9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576557"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="9f3d7-103">デバッギングのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f3d7-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f3d7-104">Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンク、コントロールを表します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="9f3d7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f3d7-105">Methods</span></span>

| <span data-ttu-id="9f3d7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f3d7-106">Method</span></span>           | <span data-ttu-id="9f3d7-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9f3d7-107">Return Type</span></span>    |<span data-ttu-id="9f3d7-108">説明</span><span class="sxs-lookup"><span data-stu-id="9f3d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f3d7-109">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="9f3d7-110">デバッギング</span><span class="sxs-lookup"><span data-stu-id="9f3d7-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="9f3d7-111">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="9f3d7-112">デバッギングを削除します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="9f3d7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-113">None.</span></span>   |   <span data-ttu-id="9f3d7-114">デバッギングをプログラムから削除します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="9f3d7-115">リスト programControls</span><span class="sxs-lookup"><span data-stu-id="9f3d7-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="9f3d7-116">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9f3d7-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="9f3d7-117">テナント内のすべてのプログラム間でコントロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="9f3d7-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f3d7-118">Permissions</span></span>

|<span data-ttu-id="9f3d7-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f3d7-119">Permission type</span></span>                        | <span data-ttu-id="9f3d7-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f3d7-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f3d7-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f3d7-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f3d7-122">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f3d7-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="9f3d7-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f3d7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f3d7-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-124">Not supported.</span></span> |
|<span data-ttu-id="9f3d7-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f3d7-125">Application</span></span>                            | <span data-ttu-id="9f3d7-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="9f3d7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3d7-127">Properties</span></span>
| <span data-ttu-id="9f3d7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3d7-128">Property</span></span>     | <span data-ttu-id="9f3d7-129">型</span><span class="sxs-lookup"><span data-stu-id="9f3d7-129">Type</span></span>   |<span data-ttu-id="9f3d7-130">説明</span><span class="sxs-lookup"><span data-stu-id="9f3d7-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="9f3d7-131">プログラムとコントロール間のリンクの機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="9f3d7-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="9f3d7-132">プログラムの programId このコントロールは、一部です。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="9f3d7-133">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="9f3d7-134">コントロールの処理、特にアクセスの id を確認します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="9f3d7-135">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="9f3d7-136">ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="9f3d7-137">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="9f3d7-138">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="9f3d7-139">コントロールのライフ サイクルの状態です。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="9f3d7-140">作成日付と時刻のコントロールです。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="9f3d7-141">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="9f3d7-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="9f3d7-142">プログラムのコントロールを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-142">The user who created the program control.</span></span>                                               |
| `resource`               | [<span data-ttu-id="9f3d7-143">programResource</span><span class="sxs-lookup"><span data-stu-id="9f3d7-143">programResource</span></span>](programresource.md)       | <span data-ttu-id="9f3d7-144">リソース、グループ、または、アプリケーションは、このプログラムの制御のアクセスの確認の対象となります。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-144">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="9f3d7-145">関係</span><span class="sxs-lookup"><span data-stu-id="9f3d7-145">Relationships</span></span>
| <span data-ttu-id="9f3d7-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f3d7-146">Relationship</span></span> | <span data-ttu-id="9f3d7-147">型</span><span class="sxs-lookup"><span data-stu-id="9f3d7-147">Type</span></span>   |<span data-ttu-id="9f3d7-148">説明</span><span class="sxs-lookup"><span data-stu-id="9f3d7-148">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="9f3d7-149">プログラム</span><span class="sxs-lookup"><span data-stu-id="9f3d7-149">program</span></span>](program.md)               | <span data-ttu-id="9f3d7-150">このコントロールの一部であるプログラムです。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-150">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="9f3d7-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f3d7-151">See also</span></span>

| <span data-ttu-id="9f3d7-152">メソッド</span><span class="sxs-lookup"><span data-stu-id="9f3d7-152">Method</span></span>           | <span data-ttu-id="9f3d7-153">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9f3d7-153">Return Type</span></span>    |<span data-ttu-id="9f3d7-154">説明</span><span class="sxs-lookup"><span data-stu-id="9f3d7-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f3d7-155">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="9f3d7-155">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="9f3d7-156">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9f3d7-156">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="9f3d7-157">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-157">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="9f3d7-158">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="9f3d7-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="9f3d7-159">[programControlType](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9f3d7-159">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="9f3d7-160">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-160">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f3d7-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f3d7-161">JSON representation</span></span>

<span data-ttu-id="9f3d7-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="9f3d7-163">ProgramResource 複合型</span><span class="sxs-lookup"><span data-stu-id="9f3d7-163">The programResource complex type</span></span>

<span data-ttu-id="9f3d7-164">プログラム コントロール オブジェクトに含まれている、プログラムのリソースは、アクセス確認の対象であるオブジェクトへの参照の表現です。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-164">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="9f3d7-165">このタイプから継承`microsoft.graph.identity`があり、1 つの追加のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-165">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="9f3d7-166">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3d7-166">Property</span></span>     | <span data-ttu-id="9f3d7-167">型</span><span class="sxs-lookup"><span data-stu-id="9f3d7-167">Type</span></span>   |<span data-ttu-id="9f3d7-168">説明</span><span class="sxs-lookup"><span data-stu-id="9f3d7-168">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="9f3d7-169">グループ、またはアプリケーションがあるかどうかを示す、リソースの種類です。</span><span class="sxs-lookup"><span data-stu-id="9f3d7-169">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
