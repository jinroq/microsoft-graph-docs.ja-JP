---
title: programcontrol リソースの種類
description: Azure AD access レビュー機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563372"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="9b79e-103">programcontrol リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b79e-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b79e-104">Azure AD [access レビュー](accessreviews-root.md)機能では、program control オブジェクトは、アクセスレビューをプログラムにリンクするコントロールを表します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="9b79e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b79e-105">Methods</span></span>

| <span data-ttu-id="9b79e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b79e-106">Method</span></span>           | <span data-ttu-id="9b79e-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9b79e-107">Return Type</span></span>    |<span data-ttu-id="9b79e-108">説明</span><span class="sxs-lookup"><span data-stu-id="9b79e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b79e-109">programcontrol を作成する</span><span class="sxs-lookup"><span data-stu-id="9b79e-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="9b79e-110">programcontrol</span><span class="sxs-lookup"><span data-stu-id="9b79e-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="9b79e-111">プログラムに programcontrol を追加します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="9b79e-112">programcontrol の削除</span><span class="sxs-lookup"><span data-stu-id="9b79e-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="9b79e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9b79e-113">None.</span></span>   |   <span data-ttu-id="9b79e-114">プログラムから programcontrol を削除します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="9b79e-115">programcontrols のリスト</span><span class="sxs-lookup"><span data-stu-id="9b79e-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="9b79e-116">[programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9b79e-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="9b79e-117">テナント内のすべてのプログラムでコントロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="9b79e-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b79e-118">Permissions</span></span>

|<span data-ttu-id="9b79e-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b79e-119">Permission type</span></span>                        | <span data-ttu-id="9b79e-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b79e-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b79e-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b79e-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b79e-122">programcontrol. all、programcontrol.</span><span class="sxs-lookup"><span data-stu-id="9b79e-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="9b79e-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b79e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b79e-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b79e-124">Not supported.</span></span> |
|<span data-ttu-id="9b79e-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b79e-125">Application</span></span>                            | <span data-ttu-id="9b79e-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b79e-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b79e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b79e-127">Properties</span></span>
| <span data-ttu-id="9b79e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b79e-128">Property</span></span>     | <span data-ttu-id="9b79e-129">型</span><span class="sxs-lookup"><span data-stu-id="9b79e-129">Type</span></span>   |<span data-ttu-id="9b79e-130">説明</span><span class="sxs-lookup"><span data-stu-id="9b79e-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="9b79e-131">プログラムとコントロール間のリンクの機能割り当て識別子</span><span class="sxs-lookup"><span data-stu-id="9b79e-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="9b79e-132">このコントロールが含まれるプログラムの programid。</span><span class="sxs-lookup"><span data-stu-id="9b79e-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="9b79e-133">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="9b79e-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="9b79e-134">コントロールの controlId (特にアクセスレビューの識別子)。</span><span class="sxs-lookup"><span data-stu-id="9b79e-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="9b79e-135">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="9b79e-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="9b79e-136">programcontroltype には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。</span><span class="sxs-lookup"><span data-stu-id="9b79e-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="9b79e-137">作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="9b79e-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="9b79e-138">コントロールの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="9b79e-139">コントロールのライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="9b79e-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="9b79e-140">プログラムコントロールの作成日時。</span><span class="sxs-lookup"><span data-stu-id="9b79e-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="9b79e-141">userIdentity</span><span class="sxs-lookup"><span data-stu-id="9b79e-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="9b79e-142">プログラムコントロールを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="9b79e-142">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="9b79e-143">このプログラムコントロールのアクセスレビューによって対象となるリソース、グループ、またはアプリ。</span><span class="sxs-lookup"><span data-stu-id="9b79e-143">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="9b79e-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b79e-144">Relationships</span></span>
| <span data-ttu-id="9b79e-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9b79e-145">Relationship</span></span> | <span data-ttu-id="9b79e-146">型</span><span class="sxs-lookup"><span data-stu-id="9b79e-146">Type</span></span>   |<span data-ttu-id="9b79e-147">説明</span><span class="sxs-lookup"><span data-stu-id="9b79e-147">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="9b79e-148">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b79e-148">program</span></span>](program.md)               | <span data-ttu-id="9b79e-149">このコントロールが含まれているプログラム。</span><span class="sxs-lookup"><span data-stu-id="9b79e-149">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="9b79e-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="9b79e-150">See also</span></span>

| <span data-ttu-id="9b79e-151">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b79e-151">Method</span></span>           | <span data-ttu-id="9b79e-152">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9b79e-152">Return Type</span></span>    |<span data-ttu-id="9b79e-153">説明</span><span class="sxs-lookup"><span data-stu-id="9b79e-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b79e-154">プログラムの programcontrols を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9b79e-154">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="9b79e-155">[programcontrol](programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9b79e-155">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="9b79e-156">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="9b79e-157">programcontroltypes のリスト</span><span class="sxs-lookup"><span data-stu-id="9b79e-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="9b79e-158">[programcontroltype](programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9b79e-158">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="9b79e-159">プログラムコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-159">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9b79e-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b79e-160">JSON representation</span></span>

<span data-ttu-id="9b79e-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b79e-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="9b79e-162">programresource 複合型</span><span class="sxs-lookup"><span data-stu-id="9b79e-162">The programResource complex type</span></span>

<span data-ttu-id="9b79e-163">program control オブジェクト内に含まれるプログラムリソースは、アクセスレビューのターゲットであるオブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-163">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="9b79e-164">この型はから`microsoft.graph.identity`継承され、さらに1つのプロパティが追加されています。</span><span class="sxs-lookup"><span data-stu-id="9b79e-164">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="9b79e-165">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b79e-165">Property</span></span>     | <span data-ttu-id="9b79e-166">型</span><span class="sxs-lookup"><span data-stu-id="9b79e-166">Type</span></span>   |<span data-ttu-id="9b79e-167">説明</span><span class="sxs-lookup"><span data-stu-id="9b79e-167">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="9b79e-168">リソースの種類。これは、グループであるかアプリであるかを示します。</span><span class="sxs-lookup"><span data-stu-id="9b79e-168">Type of the resource, indicating whether it is a group or an app.</span></span> |     


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
