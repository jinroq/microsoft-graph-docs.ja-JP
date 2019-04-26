---
title: programcontrol リソースの種類
description: Azure AD access レビュー機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。
localization_priority: Normal
ms.openlocfilehash: 7d194f3e80f44eb57be0deb7d2ffd71624c385d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344023"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="d8a2b-103">programcontrol リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8a2b-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8a2b-104">Azure AD [access レビュー](accessreviews-root.md)機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="d8a2b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8a2b-105">Methods</span></span>

| <span data-ttu-id="d8a2b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8a2b-106">Method</span></span>           | <span data-ttu-id="d8a2b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8a2b-107">Return Type</span></span>    |<span data-ttu-id="d8a2b-108">説明</span><span class="sxs-lookup"><span data-stu-id="d8a2b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8a2b-109">programcontrol を作成する</span><span class="sxs-lookup"><span data-stu-id="d8a2b-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="d8a2b-110">programcontrol</span><span class="sxs-lookup"><span data-stu-id="d8a2b-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="d8a2b-111">プログラムに programcontrol を追加します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="d8a2b-112">programcontrol の削除</span><span class="sxs-lookup"><span data-stu-id="d8a2b-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="d8a2b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-113">None.</span></span>   |   <span data-ttu-id="d8a2b-114">プログラムから programcontrol を削除します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="d8a2b-115">programcontrols のリスト</span><span class="sxs-lookup"><span data-stu-id="d8a2b-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="d8a2b-116">[programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d8a2b-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="d8a2b-117">テナント内のすべてのプログラムでコントロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-117">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8a2b-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8a2b-118">Properties</span></span>
| <span data-ttu-id="d8a2b-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8a2b-119">Property</span></span>     | <span data-ttu-id="d8a2b-120">型</span><span class="sxs-lookup"><span data-stu-id="d8a2b-120">Type</span></span>   |<span data-ttu-id="d8a2b-121">説明</span><span class="sxs-lookup"><span data-stu-id="d8a2b-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="d8a2b-122">プログラムとコントロール間のリンクの機能割り当て識別子</span><span class="sxs-lookup"><span data-stu-id="d8a2b-122">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="d8a2b-123">このコントロールが含まれるプログラムの programid。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-123">The programId of the program this control is a part of.</span></span> <span data-ttu-id="d8a2b-124">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-124">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="d8a2b-125">コントロールの controlId (特にアクセスレビューの識別子)。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-125">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="d8a2b-126">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-126">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="d8a2b-127">programcontroltype には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-127">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="d8a2b-128">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-128">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="d8a2b-129">コントロールの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-129">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="d8a2b-130">コントロールのライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-130">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="d8a2b-131">プログラムコントロールの作成日時。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-131">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="d8a2b-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d8a2b-132">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="d8a2b-133">プログラムコントロールを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-133">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="d8a2b-134">このプログラムコントロールのアクセスレビューによって対象となるリソース、グループ、またはアプリ。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-134">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="d8a2b-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8a2b-135">Relationships</span></span>
| <span data-ttu-id="d8a2b-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8a2b-136">Relationship</span></span> | <span data-ttu-id="d8a2b-137">型</span><span class="sxs-lookup"><span data-stu-id="d8a2b-137">Type</span></span>   |<span data-ttu-id="d8a2b-138">説明</span><span class="sxs-lookup"><span data-stu-id="d8a2b-138">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="d8a2b-139">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8a2b-139">program</span></span>](program.md)               | <span data-ttu-id="d8a2b-140">このコントロールが含まれているプログラム。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-140">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="d8a2b-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8a2b-141">See also</span></span>

| <span data-ttu-id="d8a2b-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8a2b-142">Method</span></span>           | <span data-ttu-id="d8a2b-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8a2b-143">Return Type</span></span>    |<span data-ttu-id="d8a2b-144">説明</span><span class="sxs-lookup"><span data-stu-id="d8a2b-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8a2b-145">プログラムの programcontrols を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d8a2b-145">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="d8a2b-146">[programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d8a2b-146">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="d8a2b-147">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-147">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="d8a2b-148">programcontroltypes のリスト</span><span class="sxs-lookup"><span data-stu-id="d8a2b-148">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="d8a2b-149">[programcontroltype](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d8a2b-149">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="d8a2b-150">プログラムコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-150">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8a2b-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8a2b-151">JSON representation</span></span>

<span data-ttu-id="d8a2b-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-152">Here is a JSON representation of the resource.</span></span>

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
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="d8a2b-153">programresource 複合型</span><span class="sxs-lookup"><span data-stu-id="d8a2b-153">The programResource complex type</span></span>

<span data-ttu-id="d8a2b-154">program control オブジェクト内に含まれるプログラムリソースは、アクセスレビューのターゲットであるオブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-154">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="d8a2b-155">この型はから`microsoft.graph.identity`継承され、さらに1つのプロパティが追加されています。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-155">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="d8a2b-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8a2b-156">Property</span></span>     | <span data-ttu-id="d8a2b-157">型</span><span class="sxs-lookup"><span data-stu-id="d8a2b-157">Type</span></span>   |<span data-ttu-id="d8a2b-158">説明</span><span class="sxs-lookup"><span data-stu-id="d8a2b-158">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="d8a2b-159">リソースの種類。これは、グループであるかアプリであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-159">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="d8a2b-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8a2b-160">JSON representation</span></span>

<span data-ttu-id="d8a2b-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8a2b-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programResource"
}-->

```json
{
 "type": "string"
}

```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
