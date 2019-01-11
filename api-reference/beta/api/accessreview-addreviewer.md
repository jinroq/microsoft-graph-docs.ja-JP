---
title: AccessReview の校閲者を追加します。
description: 'Azure AD アクセスのレビュー機能では、レビュー担当者として他のユーザーを追加するのには既存の accessReview オブジェクトを更新します。  この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。 この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。 '
localization_priority: Normal
ms.openlocfilehash: ab339a6538fc41d7e538c51251302c5e589367f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838767"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="92f20-105">AccessReview の校閲者を追加します。</span><span class="sxs-lookup"><span data-stu-id="92f20-105">Add accessReview reviewer</span></span>

> <span data-ttu-id="92f20-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92f20-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92f20-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92f20-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92f20-108">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、レビュー担当者として他のユーザーを追加するのには既存の[accessReview](../resources/accessreview.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="92f20-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="92f20-109">この操作のみ許可されてはまだ完了していない、アクセスの確認のためや、アクセスの確認にのみ、校閲者が明示的に指定されています。</span><span class="sxs-lookup"><span data-stu-id="92f20-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="92f20-110">この操作は、アクセス確認をユーザーが独自のアクセスを確認するには許可されませんし、校閲者として、グループの所有者が割り当てられている、アクセス確認のためではありません。</span><span class="sxs-lookup"><span data-stu-id="92f20-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="92f20-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92f20-111">Permissions</span></span>
<span data-ttu-id="92f20-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92f20-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92f20-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92f20-114">Permission type</span></span>                        | <span data-ttu-id="92f20-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="92f20-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="92f20-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92f20-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="92f20-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f20-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="92f20-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92f20-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92f20-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92f20-119">Not supported.</span></span> |
|<span data-ttu-id="92f20-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92f20-120">Application</span></span>                            | <span data-ttu-id="92f20-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92f20-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92f20-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92f20-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="92f20-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92f20-123">Request headers</span></span>
| <span data-ttu-id="92f20-124">名前</span><span class="sxs-lookup"><span data-stu-id="92f20-124">Name</span></span>         | <span data-ttu-id="92f20-125">種類</span><span class="sxs-lookup"><span data-stu-id="92f20-125">Type</span></span>        | <span data-ttu-id="92f20-126">説明</span><span class="sxs-lookup"><span data-stu-id="92f20-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="92f20-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="92f20-127">Authorization</span></span> | <span data-ttu-id="92f20-128">string</span><span class="sxs-lookup"><span data-stu-id="92f20-128">string</span></span> | <span data-ttu-id="92f20-129">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="92f20-129">Bearer \{token\}.</span></span> <span data-ttu-id="92f20-130">必須。</span><span class="sxs-lookup"><span data-stu-id="92f20-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92f20-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="92f20-131">Request body</span></span>
<span data-ttu-id="92f20-132">要求の本文には、校閲者となるユーザーの ID の JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="92f20-132">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="92f20-133">次の表は、accessReview を更新するときに指定できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="92f20-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="92f20-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92f20-134">Property</span></span>     | <span data-ttu-id="92f20-135">種類</span><span class="sxs-lookup"><span data-stu-id="92f20-135">Type</span></span>        | <span data-ttu-id="92f20-136">説明</span><span class="sxs-lookup"><span data-stu-id="92f20-136">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="92f20-137">ユーザー id。</span><span class="sxs-lookup"><span data-stu-id="92f20-137">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="92f20-138">応答</span><span class="sxs-lookup"><span data-stu-id="92f20-138">Response</span></span>
<span data-ttu-id="92f20-139">かどうかは成功すると、このメソッドが返されます、`201, Created`応答コード。</span><span class="sxs-lookup"><span data-stu-id="92f20-139">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="92f20-140">例</span><span class="sxs-lookup"><span data-stu-id="92f20-140">Example</span></span>

<span data-ttu-id="92f20-141">これは、1 回限り (繰り返し発生しない) のアクセス確認をその他の校閲者の更新の例です。</span><span class="sxs-lookup"><span data-stu-id="92f20-141">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="92f20-142">要求</span><span class="sxs-lookup"><span data-stu-id="92f20-142">Request</span></span>
<span data-ttu-id="92f20-143">要求の本文に、JSON 形式のユーザー オブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="92f20-143">In the request body, supply a JSON representation of the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a><span data-ttu-id="92f20-144">応答</span><span class="sxs-lookup"><span data-stu-id="92f20-144">Response</span></span>
><span data-ttu-id="92f20-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="92f20-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!-- {
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
