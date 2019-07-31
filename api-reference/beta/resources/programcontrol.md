---
title: programControl リソースの種類
description: Azure AD access レビュー機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 16824c2ed0c053f0cc4f3a0a2903324ff1a2bf5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965636"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="4bb11-103">programControl リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4bb11-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb11-104">Azure AD [access レビュー](accessreviews-root.md)機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="4bb11-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4bb11-105">Methods</span></span>

| <span data-ttu-id="4bb11-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="4bb11-106">Method</span></span>           | <span data-ttu-id="4bb11-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4bb11-107">Return Type</span></span>    |<span data-ttu-id="4bb11-108">説明</span><span class="sxs-lookup"><span data-stu-id="4bb11-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bb11-109">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="4bb11-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="4bb11-110">programControl</span><span class="sxs-lookup"><span data-stu-id="4bb11-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="4bb11-111">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="4bb11-112">ProgramControl の削除</span><span class="sxs-lookup"><span data-stu-id="4bb11-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="4bb11-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4bb11-113">None.</span></span>   |   <span data-ttu-id="4bb11-114">プログラムから programControl を削除します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="4bb11-115">ProgramControls のリスト</span><span class="sxs-lookup"><span data-stu-id="4bb11-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="4bb11-116">[Programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4bb11-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="4bb11-117">テナント内のすべてのプログラムでコントロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-117">List controls across all programs in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="4bb11-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bb11-118">Properties</span></span>
| <span data-ttu-id="4bb11-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bb11-119">Property</span></span>     | <span data-ttu-id="4bb11-120">型</span><span class="sxs-lookup"><span data-stu-id="4bb11-120">Type</span></span>   |<span data-ttu-id="4bb11-121">説明</span><span class="sxs-lookup"><span data-stu-id="4bb11-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="4bb11-122">プログラムとコントロール間のリンクの機能割り当て識別子</span><span class="sxs-lookup"><span data-stu-id="4bb11-122">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="4bb11-123">このコントロールが含まれるプログラムの programId。</span><span class="sxs-lookup"><span data-stu-id="4bb11-123">The programId of the program this control is a part of.</span></span> <span data-ttu-id="4bb11-124">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="4bb11-124">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="4bb11-125">コントロールの controlId (特にアクセスレビューの識別子)。</span><span class="sxs-lookup"><span data-stu-id="4bb11-125">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="4bb11-126">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="4bb11-126">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="4bb11-127">ProgramControlType には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。</span><span class="sxs-lookup"><span data-stu-id="4bb11-127">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="4bb11-128">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="4bb11-128">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="4bb11-129">コントロールの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-129">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="4bb11-130">コントロールのライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="4bb11-130">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="4bb11-131">プログラムコントロールの作成日時。</span><span class="sxs-lookup"><span data-stu-id="4bb11-131">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="4bb11-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="4bb11-132">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="4bb11-133">プログラムコントロールを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="4bb11-133">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="4bb11-134">このプログラムコントロールのアクセスレビューによって対象となるリソース、グループ、またはアプリ。</span><span class="sxs-lookup"><span data-stu-id="4bb11-134">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="4bb11-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4bb11-135">Relationships</span></span>
| <span data-ttu-id="4bb11-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4bb11-136">Relationship</span></span> | <span data-ttu-id="4bb11-137">型</span><span class="sxs-lookup"><span data-stu-id="4bb11-137">Type</span></span>   |<span data-ttu-id="4bb11-138">説明</span><span class="sxs-lookup"><span data-stu-id="4bb11-138">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="4bb11-139">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bb11-139">program</span></span>](program.md)               | <span data-ttu-id="4bb11-140">このコントロールが含まれているプログラム。</span><span class="sxs-lookup"><span data-stu-id="4bb11-140">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="4bb11-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="4bb11-141">See also</span></span>

| <span data-ttu-id="4bb11-142">メソッド</span><span class="sxs-lookup"><span data-stu-id="4bb11-142">Method</span></span>           | <span data-ttu-id="4bb11-143">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4bb11-143">Return Type</span></span>    |<span data-ttu-id="4bb11-144">説明</span><span class="sxs-lookup"><span data-stu-id="4bb11-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bb11-145">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4bb11-145">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="4bb11-146">[Programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4bb11-146">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="4bb11-147">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-147">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="4bb11-148">ProgramControlTypes のリスト</span><span class="sxs-lookup"><span data-stu-id="4bb11-148">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="4bb11-149">[Programcontroltype](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4bb11-149">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="4bb11-150">プログラムコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-150">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4bb11-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4bb11-151">JSON representation</span></span>

<span data-ttu-id="4bb11-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4bb11-152">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="4bb11-153">ProgramResource 複合型</span><span class="sxs-lookup"><span data-stu-id="4bb11-153">The programResource complex type</span></span>

<span data-ttu-id="4bb11-154">Program control オブジェクト内に含まれるプログラムリソースは、アクセスレビューのターゲットであるオブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-154">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="4bb11-155">この型はから`microsoft.graph.identity`継承され、さらに1つのプロパティが追加されています。</span><span class="sxs-lookup"><span data-stu-id="4bb11-155">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="4bb11-156">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bb11-156">Property</span></span>     | <span data-ttu-id="4bb11-157">型</span><span class="sxs-lookup"><span data-stu-id="4bb11-157">Type</span></span>   |<span data-ttu-id="4bb11-158">説明</span><span class="sxs-lookup"><span data-stu-id="4bb11-158">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="4bb11-159">リソースの種類。これは、グループであるかアプリであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="4bb11-159">Type of the resource, indicating whether it is a group or an app.</span></span> |     

## <a name="json-representation"></a><span data-ttu-id="4bb11-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4bb11-160">JSON representation</span></span>

<span data-ttu-id="4bb11-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4bb11-161">Here is a JSON representation of the resource.</span></span>

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
