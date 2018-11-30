---
title: デバッギングのリソースの種類
description: Azure AD にアクセスが機能を確認、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンクするコントロールを表します。
ms.openlocfilehash: 03e70ffdf0607eeb11abaf1b12065b4092294d23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069482"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="026ff-103">デバッギングのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="026ff-103">programControl resource type</span></span>

> <span data-ttu-id="026ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="026ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="026ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="026ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="026ff-106">Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンク、コントロールを表します。</span><span class="sxs-lookup"><span data-stu-id="026ff-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="026ff-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="026ff-107">Methods</span></span>

| <span data-ttu-id="026ff-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="026ff-108">Method</span></span>           | <span data-ttu-id="026ff-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="026ff-109">Return Type</span></span>    |<span data-ttu-id="026ff-110">説明</span><span class="sxs-lookup"><span data-stu-id="026ff-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="026ff-111">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="026ff-111">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="026ff-112">デバッギング</span><span class="sxs-lookup"><span data-stu-id="026ff-112">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="026ff-113">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="026ff-113">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="026ff-114">デバッギングを削除します。</span><span class="sxs-lookup"><span data-stu-id="026ff-114">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="026ff-115">なし。</span><span class="sxs-lookup"><span data-stu-id="026ff-115">None.</span></span>   |   <span data-ttu-id="026ff-116">デバッギングをプログラムから削除します。</span><span class="sxs-lookup"><span data-stu-id="026ff-116">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="026ff-117">リスト programControls</span><span class="sxs-lookup"><span data-stu-id="026ff-117">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="026ff-118">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="026ff-118">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="026ff-119">テナント内のすべてのプログラム間でコントロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="026ff-119">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="026ff-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="026ff-120">Permissions</span></span>

|<span data-ttu-id="026ff-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="026ff-121">Permission type</span></span>                        | <span data-ttu-id="026ff-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="026ff-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="026ff-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="026ff-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="026ff-124">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="026ff-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="026ff-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="026ff-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="026ff-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="026ff-126">Not supported.</span></span> |
|<span data-ttu-id="026ff-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="026ff-127">Application</span></span>                            | <span data-ttu-id="026ff-128">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="026ff-128">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="026ff-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="026ff-129">Properties</span></span>
| <span data-ttu-id="026ff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="026ff-130">Property</span></span>     | <span data-ttu-id="026ff-131">型</span><span class="sxs-lookup"><span data-stu-id="026ff-131">Type</span></span>   |<span data-ttu-id="026ff-132">説明</span><span class="sxs-lookup"><span data-stu-id="026ff-132">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="026ff-133">プログラムとコントロール間のリンクの機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="026ff-133">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="026ff-134">プログラムの programId このコントロールは、一部です。</span><span class="sxs-lookup"><span data-stu-id="026ff-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="026ff-135">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="026ff-135">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="026ff-136">コントロールの処理、特にアクセスの id を確認します。</span><span class="sxs-lookup"><span data-stu-id="026ff-136">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="026ff-137">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="026ff-137">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="026ff-138">ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。</span><span class="sxs-lookup"><span data-stu-id="026ff-138">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="026ff-139">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="026ff-139">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="026ff-140">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="026ff-140">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="026ff-141">コントロールのライフ サイクルの状態です。</span><span class="sxs-lookup"><span data-stu-id="026ff-141">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="026ff-142">作成日付と時刻のコントロールです。</span><span class="sxs-lookup"><span data-stu-id="026ff-142">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="026ff-143">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="026ff-143">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="026ff-144">プログラムのコントロールを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="026ff-144">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="026ff-145">リソース、グループ、または、アプリケーションは、このプログラムの制御のアクセスの確認の対象となります。</span><span class="sxs-lookup"><span data-stu-id="026ff-145">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="026ff-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="026ff-146">Relationships</span></span>
| <span data-ttu-id="026ff-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="026ff-147">Relationship</span></span> | <span data-ttu-id="026ff-148">型</span><span class="sxs-lookup"><span data-stu-id="026ff-148">Type</span></span>   |<span data-ttu-id="026ff-149">説明</span><span class="sxs-lookup"><span data-stu-id="026ff-149">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="026ff-150">プログラム</span><span class="sxs-lookup"><span data-stu-id="026ff-150">program</span></span>](program.md)               | <span data-ttu-id="026ff-151">このコントロールの一部であるプログラムです。</span><span class="sxs-lookup"><span data-stu-id="026ff-151">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="026ff-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="026ff-152">See also</span></span>

| <span data-ttu-id="026ff-153">メソッド</span><span class="sxs-lookup"><span data-stu-id="026ff-153">Method</span></span>           | <span data-ttu-id="026ff-154">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="026ff-154">Return Type</span></span>    |<span data-ttu-id="026ff-155">説明</span><span class="sxs-lookup"><span data-stu-id="026ff-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="026ff-156">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="026ff-156">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="026ff-157">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="026ff-157">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="026ff-158">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="026ff-158">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="026ff-159">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="026ff-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="026ff-160">[programControlType](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="026ff-160">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="026ff-161">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="026ff-161">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="026ff-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="026ff-162">JSON representation</span></span>

<span data-ttu-id="026ff-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="026ff-163">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="026ff-164">ProgramResource 複合型</span><span class="sxs-lookup"><span data-stu-id="026ff-164">The programResource complex type</span></span>

<span data-ttu-id="026ff-165">プログラム コントロール オブジェクトに含まれている、プログラムのリソースは、アクセス確認の対象であるオブジェクトへの参照の表現です。</span><span class="sxs-lookup"><span data-stu-id="026ff-165">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="026ff-166">このタイプから継承`microsoft.graph.identity`があり、1 つの追加のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="026ff-166">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="026ff-167">プロパティ</span><span class="sxs-lookup"><span data-stu-id="026ff-167">Property</span></span>     | <span data-ttu-id="026ff-168">型</span><span class="sxs-lookup"><span data-stu-id="026ff-168">Type</span></span>   |<span data-ttu-id="026ff-169">説明</span><span class="sxs-lookup"><span data-stu-id="026ff-169">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="026ff-170">グループ、またはアプリケーションがあるかどうかを示す、リソースの種類です。</span><span class="sxs-lookup"><span data-stu-id="026ff-170">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->