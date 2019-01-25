---
title: 型を割り当てられていません
description: 'Azure AD のレビューにアクセスして、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529468"
---
# <a name="useridentity-type"></a><span data-ttu-id="23618-103">型を割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="23618-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23618-104">Azure AD[アクセスの確認](accessreviews-root.md)をするは、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。</span><span class="sxs-lookup"><span data-stu-id="23618-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="23618-105">Azure AD の監査ログのコンテキストでは、開始、または監査活動の影響を受けたユーザーの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="23618-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="23618-106">このタイプは、[アイデンティティ](identity.md)を継承し、追加の 1 つのプロパティ、ユーザーのユーザー プリンシパル名を持ちます。</span><span class="sxs-lookup"><span data-stu-id="23618-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="23618-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="23618-107">Methods</span></span>

<span data-ttu-id="23618-108">なし</span><span class="sxs-lookup"><span data-stu-id="23618-108">None.</span></span>  <span data-ttu-id="23618-109">要求の本文にこの型のオブジェクトを含めますと[、accessReview を作成](../api/accessreview-create.md)します。</span><span class="sxs-lookup"><span data-stu-id="23618-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="23618-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23618-110">Properties</span></span>
| <span data-ttu-id="23618-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23618-111">Property</span></span>     | <span data-ttu-id="23618-112">型</span><span class="sxs-lookup"><span data-stu-id="23618-112">Type</span></span>   |<span data-ttu-id="23618-113">説明</span><span class="sxs-lookup"><span data-stu-id="23618-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="23618-114">Id の表示名です。</span><span class="sxs-lookup"><span data-stu-id="23618-114">The identity's display name.</span></span> <span data-ttu-id="23618-115">このできない可能性がある利用可能なまたは最新の状態に注意してください。</span><span class="sxs-lookup"><span data-stu-id="23618-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="23618-116">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="23618-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="23618-117">アクティビティ (監査ログのみ) を実行するユーザーによって使用されるクライアントの IP アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="23618-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="23618-118">ユーザーの userPrincipalName 属性です。</span><span class="sxs-lookup"><span data-stu-id="23618-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="23618-119">注釈</span><span class="sxs-lookup"><span data-stu-id="23618-119">Remarks</span></span>

<span data-ttu-id="23618-p103">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="23618-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="23618-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23618-122">Relationships</span></span>

<span data-ttu-id="23618-123">なし。</span><span class="sxs-lookup"><span data-stu-id="23618-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="23618-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="23618-124">See also</span></span>

| <span data-ttu-id="23618-125">メソッド</span><span class="sxs-lookup"><span data-stu-id="23618-125">Method</span></span>           | <span data-ttu-id="23618-126">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="23618-126">Return Type</span></span>    |<span data-ttu-id="23618-127">説明</span><span class="sxs-lookup"><span data-stu-id="23618-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23618-128">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="23618-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="23618-129">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="23618-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="23618-130">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="23618-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="23618-131">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="23618-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="23618-132">なし。</span><span class="sxs-lookup"><span data-stu-id="23618-132">None.</span></span>   |   <span data-ttu-id="23618-133">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="23618-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="23618-134">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="23618-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="23618-135">なし。</span><span class="sxs-lookup"><span data-stu-id="23618-135">None.</span></span>  |   <span data-ttu-id="23618-136">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="23618-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="23618-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23618-137">JSON representation</span></span>

<span data-ttu-id="23618-138">ここでは、型の JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="23618-138">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
 "userPrincipalName": "String"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
