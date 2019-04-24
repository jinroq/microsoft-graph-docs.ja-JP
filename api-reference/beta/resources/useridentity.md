---
title: useridentity の種類
description: 'azure ad のアクセスレビューの場合、この種類は、アクセスレビューのレビュー担当者のための azure ad ユーザー id を表します。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453979"
---
# <a name="useridentity-type"></a><span data-ttu-id="f7c80-103">useridentity の種類</span><span class="sxs-lookup"><span data-stu-id="f7c80-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c80-104">azure ad の[アクセス](accessreviews-root.md)レビューの場合、この種類は、アクセスレビューのレビュー担当者のための azure ad ユーザー id を表します。</span><span class="sxs-lookup"><span data-stu-id="f7c80-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="f7c80-105">Azure AD 監査ログのコンテキストでは、これは監査アクティビティの開始または影響を受けたユーザー情報を表します。</span><span class="sxs-lookup"><span data-stu-id="f7c80-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="f7c80-106">この型は、 [identity](identity.md)から継承し、ユーザーのユーザープリンシパル名である1つの追加のプロパティを持ちます。</span><span class="sxs-lookup"><span data-stu-id="f7c80-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="f7c80-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7c80-107">Methods</span></span>

<span data-ttu-id="f7c80-108">なし。</span><span class="sxs-lookup"><span data-stu-id="f7c80-108">None.</span></span>  <span data-ttu-id="f7c80-109">[accessreview を作成](../api/accessreview-create.md)するときに、要求の本文にこの種類のオブジェクトを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f7c80-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f7c80-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c80-110">Properties</span></span>
| <span data-ttu-id="f7c80-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c80-111">Property</span></span>     | <span data-ttu-id="f7c80-112">型</span><span class="sxs-lookup"><span data-stu-id="f7c80-112">Type</span></span>   |<span data-ttu-id="f7c80-113">説明</span><span class="sxs-lookup"><span data-stu-id="f7c80-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="f7c80-114">id の表示名。</span><span class="sxs-lookup"><span data-stu-id="f7c80-114">The identity's display name.</span></span> <span data-ttu-id="f7c80-115">これは、常に有効であったり、最新ではない場合があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f7c80-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="f7c80-116">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f7c80-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="f7c80-117">ユーザーがアクティビティを実行するときに使用するクライアント IP アドレスを示します (監査ログのみ)。</span><span class="sxs-lookup"><span data-stu-id="f7c80-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="f7c80-118">ユーザーの userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="f7c80-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="f7c80-119">注釈</span><span class="sxs-lookup"><span data-stu-id="f7c80-119">Remarks</span></span>

<span data-ttu-id="f7c80-p103">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="f7c80-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="f7c80-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7c80-122">Relationships</span></span>

<span data-ttu-id="f7c80-123">なし。</span><span class="sxs-lookup"><span data-stu-id="f7c80-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="f7c80-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="f7c80-124">See also</span></span>

| <span data-ttu-id="f7c80-125">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7c80-125">Method</span></span>           | <span data-ttu-id="f7c80-126">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f7c80-126">Return Type</span></span>    |<span data-ttu-id="f7c80-127">説明</span><span class="sxs-lookup"><span data-stu-id="f7c80-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7c80-128">アクセスレビューのレビュー担当者を取得する</span><span class="sxs-lookup"><span data-stu-id="f7c80-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="f7c80-129">[useridentity](useridentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f7c80-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="f7c80-130">accessreview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="f7c80-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="f7c80-131">accessreview レビュー担当者を追加する</span><span class="sxs-lookup"><span data-stu-id="f7c80-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="f7c80-132">なし。</span><span class="sxs-lookup"><span data-stu-id="f7c80-132">None.</span></span>   |   <span data-ttu-id="f7c80-133">閲覧者を accessreview に追加します。</span><span class="sxs-lookup"><span data-stu-id="f7c80-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="f7c80-134">accessreview レビュー担当者を削除する</span><span class="sxs-lookup"><span data-stu-id="f7c80-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="f7c80-135">なし。</span><span class="sxs-lookup"><span data-stu-id="f7c80-135">None.</span></span>  |   <span data-ttu-id="f7c80-136">accessreview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="f7c80-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7c80-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7c80-137">JSON representation</span></span>

<span data-ttu-id="f7c80-138">この型の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7c80-138">Here is a JSON representation of the type.</span></span>

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
