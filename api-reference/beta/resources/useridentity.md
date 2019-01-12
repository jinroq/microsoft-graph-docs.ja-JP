---
title: 型を割り当てられていません
description: 'Azure AD のレビューにアクセスして、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80e8cc68d4fc2f642be6c748b762fe47c7489d59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932281"
---
# <a name="useridentity-type"></a><span data-ttu-id="a1fd8-103">型を割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="a1fd8-103">userIdentity type</span></span>

> <span data-ttu-id="a1fd8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1fd8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1fd8-106">Azure AD[アクセスの確認](accessreviews-root.md)をするは、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-106">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="a1fd8-107">Azure AD の監査ログのコンテキストでは、開始、または監査活動の影響を受けたユーザーの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-107">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="a1fd8-108">このタイプは、[アイデンティティ](identity.md)を継承し、追加の 1 つのプロパティ、ユーザーのユーザー プリンシパル名を持ちます。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-108">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="a1fd8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1fd8-109">Methods</span></span>

<span data-ttu-id="a1fd8-110">なし</span><span class="sxs-lookup"><span data-stu-id="a1fd8-110">None.</span></span>  <span data-ttu-id="a1fd8-111">要求の本文にこの型のオブジェクトを含めますと[、accessReview を作成](../api/accessreview-create.md)します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-111">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a1fd8-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1fd8-112">Properties</span></span>
| <span data-ttu-id="a1fd8-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1fd8-113">Property</span></span>     | <span data-ttu-id="a1fd8-114">種類</span><span class="sxs-lookup"><span data-stu-id="a1fd8-114">Type</span></span>   |<span data-ttu-id="a1fd8-115">説明</span><span class="sxs-lookup"><span data-stu-id="a1fd8-115">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="a1fd8-116">Id の表示名です。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-116">The identity's display name.</span></span> <span data-ttu-id="a1fd8-117">このできない可能性がある利用可能なまたは最新の状態に注意してください。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-117">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="a1fd8-118">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-118">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="a1fd8-119">アクティビティ (監査ログのみ) を実行するユーザーによって使用されるクライアントの IP アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="a1fd8-120">ユーザーの userPrincipalName 属性です。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-120">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="a1fd8-121">注釈</span><span class="sxs-lookup"><span data-stu-id="a1fd8-121">Remarks</span></span>

<span data-ttu-id="a1fd8-p104">状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="a1fd8-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1fd8-124">Relationships</span></span>

<span data-ttu-id="a1fd8-125">なし。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="a1fd8-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="a1fd8-126">See also</span></span>

| <span data-ttu-id="a1fd8-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1fd8-127">Method</span></span>           | <span data-ttu-id="a1fd8-128">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1fd8-128">Return Type</span></span>    |<span data-ttu-id="a1fd8-129">説明</span><span class="sxs-lookup"><span data-stu-id="a1fd8-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1fd8-130">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-130">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="a1fd8-131">コレクションを[割り当てられていません](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="a1fd8-131">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="a1fd8-132">AccessReview のレビュー担当者を取得します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-132">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="a1fd8-133">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-133">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="a1fd8-134">なし。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-134">None.</span></span>   |   <span data-ttu-id="a1fd8-135">AccessReview には、レビュー担当者を追加します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-135">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="a1fd8-136">AccessReview のレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-136">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="a1fd8-137">なし。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-137">None.</span></span>  |   <span data-ttu-id="a1fd8-138">AccessReview からレビュー担当者を削除します。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-138">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1fd8-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1fd8-139">JSON representation</span></span>

<span data-ttu-id="a1fd8-140">ここでは、型の JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="a1fd8-140">Here is a JSON representation of the type.</span></span>

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
