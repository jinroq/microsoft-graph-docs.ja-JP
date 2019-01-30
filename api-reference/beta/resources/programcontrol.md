---
title: デバッギングのリソースの種類
description: Azure AD にアクセスが機能を確認、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンクするコントロールを表します。
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644008"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="b34cd-103">デバッギングのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="b34cd-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b34cd-104">Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンク、コントロールを表します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="b34cd-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b34cd-105">Methods</span></span>

| <span data-ttu-id="b34cd-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b34cd-106">Method</span></span>           | <span data-ttu-id="b34cd-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b34cd-107">Return Type</span></span>    |<span data-ttu-id="b34cd-108">説明</span><span class="sxs-lookup"><span data-stu-id="b34cd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b34cd-109">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="b34cd-110">デバッギング</span><span class="sxs-lookup"><span data-stu-id="b34cd-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="b34cd-111">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="b34cd-112">デバッギングを削除します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="b34cd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b34cd-113">None.</span></span>   |   <span data-ttu-id="b34cd-114">デバッギングをプログラムから削除します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="b34cd-115">リスト programControls</span><span class="sxs-lookup"><span data-stu-id="b34cd-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="b34cd-116">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b34cd-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="b34cd-117">テナント内のすべてのプログラム間でコントロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="b34cd-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b34cd-118">Permissions</span></span>

|<span data-ttu-id="b34cd-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b34cd-119">Permission type</span></span>                        | <span data-ttu-id="b34cd-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b34cd-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b34cd-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b34cd-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="b34cd-122">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b34cd-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="b34cd-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b34cd-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b34cd-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b34cd-124">Not supported.</span></span> |
|<span data-ttu-id="b34cd-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b34cd-125">Application</span></span>                            | <span data-ttu-id="b34cd-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b34cd-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="b34cd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b34cd-127">Properties</span></span>
| <span data-ttu-id="b34cd-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b34cd-128">Property</span></span>     | <span data-ttu-id="b34cd-129">型</span><span class="sxs-lookup"><span data-stu-id="b34cd-129">Type</span></span>   |<span data-ttu-id="b34cd-130">説明</span><span class="sxs-lookup"><span data-stu-id="b34cd-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="b34cd-131">プログラムとコントロール間のリンクの機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="b34cd-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="b34cd-132">プログラムの programId このコントロールは、一部です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="b34cd-133">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="b34cd-134">コントロールの処理、特にアクセスの id を確認します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="b34cd-135">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="b34cd-136">ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="b34cd-137">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="b34cd-138">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="b34cd-139">コントロールのライフ サイクルの状態です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="b34cd-140">作成日付と時刻のコントロールです。</span><span class="sxs-lookup"><span data-stu-id="b34cd-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="b34cd-141">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="b34cd-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="b34cd-142">プログラムのコントロールを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="b34cd-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="b34cd-143">リソース、グループ、または、アプリケーションは、このプログラムの制御のアクセスの確認の対象となります。</span><span class="sxs-lookup"><span data-stu-id="b34cd-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="b34cd-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b34cd-144">Relationships</span></span>
| <span data-ttu-id="b34cd-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b34cd-145">Relationship</span></span> | <span data-ttu-id="b34cd-146">型</span><span class="sxs-lookup"><span data-stu-id="b34cd-146">Type</span></span>   |<span data-ttu-id="b34cd-147">説明</span><span class="sxs-lookup"><span data-stu-id="b34cd-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="b34cd-148">プログラム</span><span class="sxs-lookup"><span data-stu-id="b34cd-148">program</span></span>](program.md)               | <span data-ttu-id="b34cd-149">このコントロールの一部であるプログラムです。</span><span class="sxs-lookup"><span data-stu-id="b34cd-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="b34cd-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="b34cd-150">See also</span></span>

| <span data-ttu-id="b34cd-151">メソッド</span><span class="sxs-lookup"><span data-stu-id="b34cd-151">Method</span></span>           | <span data-ttu-id="b34cd-152">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b34cd-152">Return Type</span></span>    |<span data-ttu-id="b34cd-153">説明</span><span class="sxs-lookup"><span data-stu-id="b34cd-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b34cd-154">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="b34cd-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="b34cd-155">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b34cd-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="b34cd-156">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b34cd-157">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="b34cd-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="b34cd-158">[programControlType](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b34cd-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="b34cd-159">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b34cd-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b34cd-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b34cd-160">JSON representation</span></span>

<span data-ttu-id="b34cd-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="b34cd-162">ProgramResource 複合型</span><span class="sxs-lookup"><span data-stu-id="b34cd-162">The programResource complex type</span></span>

<span data-ttu-id="b34cd-163">プログラム コントロール オブジェクトに含まれている、プログラムのリソースは、アクセス確認の対象であるオブジェクトへの参照の表現です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="b34cd-164">このタイプから継承`microsoft.graph.identity`があり、1 つの追加のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b34cd-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="b34cd-165">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b34cd-165">Property</span></span>     | <span data-ttu-id="b34cd-166">型</span><span class="sxs-lookup"><span data-stu-id="b34cd-166">Type</span></span>   |<span data-ttu-id="b34cd-167">説明</span><span class="sxs-lookup"><span data-stu-id="b34cd-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="b34cd-168">グループ、またはアプリケーションがあるかどうかを示す、リソースの種類です。</span><span class="sxs-lookup"><span data-stu-id="b34cd-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


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
