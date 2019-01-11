---
title: デバッギングのリソースの種類
description: Azure AD にアクセスが機能を確認、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンクするコントロールを表します。
localization_priority: Normal
ms.openlocfilehash: ddf6e978277ca1801f9126597ac4b3561fe5bfb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817823"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="ab7d0-103">デバッギングのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab7d0-103">programControl resource type</span></span>

> <span data-ttu-id="ab7d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab7d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab7d0-106">Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンク、コントロールを表します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="ab7d0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab7d0-107">Methods</span></span>

| <span data-ttu-id="ab7d0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab7d0-108">Method</span></span>           | <span data-ttu-id="ab7d0-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab7d0-109">Return Type</span></span>    |<span data-ttu-id="ab7d0-110">説明</span><span class="sxs-lookup"><span data-stu-id="ab7d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab7d0-111">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-111">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="ab7d0-112">デバッギング</span><span class="sxs-lookup"><span data-stu-id="ab7d0-112">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="ab7d0-113">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-113">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="ab7d0-114">デバッギングを削除します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-114">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="ab7d0-115">なし。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-115">None.</span></span>   |   <span data-ttu-id="ab7d0-116">デバッギングをプログラムから削除します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-116">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="ab7d0-117">リスト programControls</span><span class="sxs-lookup"><span data-stu-id="ab7d0-117">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="ab7d0-118">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab7d0-118">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="ab7d0-119">テナント内のすべてのプログラム間でコントロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-119">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="ab7d0-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="ab7d0-120">Permissions</span></span>

|<span data-ttu-id="ab7d0-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab7d0-121">Permission type</span></span>                        | <span data-ttu-id="ab7d0-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab7d0-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab7d0-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab7d0-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab7d0-124">ProgramControl.Read.All、ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab7d0-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="ab7d0-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab7d0-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab7d0-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-126">Not supported.</span></span> |
|<span data-ttu-id="ab7d0-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab7d0-127">Application</span></span>                            | <span data-ttu-id="ab7d0-128">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-128">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab7d0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab7d0-129">Properties</span></span>
| <span data-ttu-id="ab7d0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab7d0-130">Property</span></span>     | <span data-ttu-id="ab7d0-131">種類</span><span class="sxs-lookup"><span data-stu-id="ab7d0-131">Type</span></span>   |<span data-ttu-id="ab7d0-132">説明</span><span class="sxs-lookup"><span data-stu-id="ab7d0-132">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="ab7d0-133">プログラムとコントロール間のリンクの機能に割り当てられた識別子</span><span class="sxs-lookup"><span data-stu-id="ab7d0-133">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="ab7d0-134">プログラムの programId このコントロールは、一部です。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="ab7d0-135">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-135">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="ab7d0-136">コントロールの処理、特にアクセスの id を確認します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-136">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="ab7d0-137">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-137">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="ab7d0-138">ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-138">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="ab7d0-139">必要なを作成します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-139">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="ab7d0-140">コントロールの名前です。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-140">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="ab7d0-141">コントロールのライフ サイクルの状態です。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-141">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="ab7d0-142">作成日付と時刻のコントロールです。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-142">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="ab7d0-143">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="ab7d0-143">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="ab7d0-144">プログラムのコントロールを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-144">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="ab7d0-145">リソース、グループ、または、アプリケーションは、このプログラムの制御のアクセスの確認の対象となります。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-145">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="ab7d0-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab7d0-146">Relationships</span></span>
| <span data-ttu-id="ab7d0-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab7d0-147">Relationship</span></span> | <span data-ttu-id="ab7d0-148">型</span><span class="sxs-lookup"><span data-stu-id="ab7d0-148">Type</span></span>   |<span data-ttu-id="ab7d0-149">説明</span><span class="sxs-lookup"><span data-stu-id="ab7d0-149">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="ab7d0-150">プログラム</span><span class="sxs-lookup"><span data-stu-id="ab7d0-150">program</span></span>](program.md)               | <span data-ttu-id="ab7d0-151">このコントロールの一部であるプログラムです。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-151">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="ab7d0-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="ab7d0-152">See also</span></span>

| <span data-ttu-id="ab7d0-153">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab7d0-153">Method</span></span>           | <span data-ttu-id="ab7d0-154">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab7d0-154">Return Type</span></span>    |<span data-ttu-id="ab7d0-155">説明</span><span class="sxs-lookup"><span data-stu-id="ab7d0-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab7d0-156">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="ab7d0-156">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="ab7d0-157">[デバッギング](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab7d0-157">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="ab7d0-158">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-158">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ab7d0-159">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="ab7d0-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="ab7d0-160">[programControlType](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ab7d0-160">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="ab7d0-161">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-161">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab7d0-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab7d0-162">JSON representation</span></span>

<span data-ttu-id="ab7d0-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-163">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="ab7d0-164">ProgramResource 複合型</span><span class="sxs-lookup"><span data-stu-id="ab7d0-164">The programResource complex type</span></span>

<span data-ttu-id="ab7d0-165">プログラム コントロール オブジェクトに含まれている、プログラムのリソースは、アクセス確認の対象であるオブジェクトへの参照の表現です。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-165">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="ab7d0-166">このタイプから継承`microsoft.graph.identity`があり、1 つの追加のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-166">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="ab7d0-167">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab7d0-167">Property</span></span>     | <span data-ttu-id="ab7d0-168">種類</span><span class="sxs-lookup"><span data-stu-id="ab7d0-168">Type</span></span>   |<span data-ttu-id="ab7d0-169">説明</span><span class="sxs-lookup"><span data-stu-id="ab7d0-169">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="ab7d0-170">グループ、またはアプリケーションがあるかどうかを示す、リソースの種類です。</span><span class="sxs-lookup"><span data-stu-id="ab7d0-170">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
