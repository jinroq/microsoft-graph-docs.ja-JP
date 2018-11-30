---
title: 型を割り当てられていません
description: 'Azure AD のレビューにアクセスして、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。  '
ms.openlocfilehash: 6cbbe7aa017572bcd753a57edbf82751ac4986a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069480"
---
# <a name="useridentity-type"></a><span data-ttu-id="c961f-103">型を割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="c961f-103">userIdentity type</span></span>

> <span data-ttu-id="c961f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c961f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c961f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c961f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c961f-106">Azure AD[アクセスの確認](accessreviews-root.md)をするは、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。</span><span class="sxs-lookup"><span data-stu-id="c961f-106">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="c961f-107">Azure AD の監査ログのコンテキストでは、開始、または監査活動の影響を受けたユーザーの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="c961f-107">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="c961f-108">このタイプは、[アイデンティティ](identity.md)を継承し、追加の 1 つのプロパティ、ユーザーのユーザー プリンシパル名を持ちます。</span><span class="sxs-lookup"><span data-stu-id="c961f-108">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="c961f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c961f-109">Methods</span></span>

<span data-ttu-id="c961f-110">なし</span><span class="sxs-lookup"><span data-stu-id="c961f-110">None.</span></span>  <span data-ttu-id="c961f-111">要求の本文にこの型のオブジェクトを含めますと[、accessReview を作成](../api/accessreview-create.md)します。</span><span class="sxs-lookup"><span data-stu-id="c961f-111">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c961f-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c961f-112">Properties</span></span>
| <span data-ttu-id="c961f-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c961f-113">Property</span></span>     | <span data-ttu-id="c961f-114">型</span><span class="sxs-lookup"><span data-stu-id="c961f-114">Type</span></span>   |<span data-ttu-id="c961f-115">説明</span><span class="sxs-lookup"><span data-stu-id="c961f-115">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="c961f-116">Id の表示名です。</span><span class="sxs-lookup"><span data-stu-id="c961f-116">The identity's display name.</span></span> <span data-ttu-id="c961f-117">このできない可能性がある利用可能なまたは最新の状態に注意してください。</span><span class="sxs-lookup"><span data-stu-id="c961f-117">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="c961f-118">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c961f-118">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="c961f-119">アクティビティ (監査ログのみ) を実行するユーザーによって使用されるクライアントの IP アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="c961f-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="c961f-120">ユーザーの userPrincipalName 属性です。</span><span class="sxs-lookup"><span data-stu-id="c961f-120">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c961f-121">注釈</span><span class="sxs-lookup"><span data-stu-id="c961f-121">Remarks</span></span>

<span data-ttu-id="c961f-p104">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="c961f-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="c961f-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c961f-124">Relationships</span></span>

<span data-ttu-id="c961f-125">なし。</span><span class="sxs-lookup"><span data-stu-id="c961f-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="c961f-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="c961f-126">See also</span></span>

| <span data-ttu-id="c961f-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="c961f-127">Method</span></span>           | <span data-ttu-id="c961f-128">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c961f-128">Return Type</span></span>    |<span data-ttu-id="c961f-129">説明</span><span class="sxs-lookup"><span data-stu-id="c961f-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c961f-130">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="c961f-130">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="c961f-131">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="c961f-131">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="c961f-132">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="c961f-132">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="c961f-133">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="c961f-133">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="c961f-134">なし。</span><span class="sxs-lookup"><span data-stu-id="c961f-134">None.</span></span>   |   <span data-ttu-id="c961f-135">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="c961f-135">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="c961f-136">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="c961f-136">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="c961f-137">なし。</span><span class="sxs-lookup"><span data-stu-id="c961f-137">None.</span></span>  |   <span data-ttu-id="c961f-138">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="c961f-138">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c961f-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c961f-139">JSON representation</span></span>

<span data-ttu-id="c961f-140">ここでは、型の JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="c961f-140">Here is a JSON representation of the type.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
