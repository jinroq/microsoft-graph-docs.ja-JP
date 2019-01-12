---
title: AccessReview を適用します。
description: 'Azure AD のレビュー機能にアクセス、完成した accessReview の決定を適用します。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e230a9638e865fbca69448f3a7683b95db954598
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951335"
---
# <a name="apply-accessreview"></a><span data-ttu-id="e3923-104">AccessReview を適用します。</span><span class="sxs-lookup"><span data-stu-id="e3923-104">Apply accessReview</span></span>

> <span data-ttu-id="e3923-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3923-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3923-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3923-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3923-107">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、完成した[accessReview](../resources/accessreview.md)の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="e3923-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="e3923-108">ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="e3923-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="e3923-109">アクセス確認が完了したら、いずれかの終了日に到達したか、または管理者が手動で停止しているし、自動適用ためにでしたように構成されて、確認のため、変更を適用する適用を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="e3923-109">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="e3923-110">適用が行われるまでアクセス権を削除するのには意思決定には表示されませんソース リソースをユーザーがインスタンスにそれらのグループ メンバーシップを保持します。</span><span class="sxs-lookup"><span data-stu-id="e3923-110">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="e3923-111">呼び出すことによって適用、レビューの結果は、グループまたはアプリケーションを更新することによって実装されています。</span><span class="sxs-lookup"><span data-stu-id="e3923-111">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="e3923-112">ユーザーのアクセスが拒否された場合、レビューに管理者は、この API を呼び出すときに、Azure の AD は、メンバーシップ、またはアプリケーションの割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="e3923-112">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="e3923-113">アクセス確認が終了したら、自動適用後に構成していたレビューのステータスが完了から、中間の状態が変更され、最後に適用の状態に変更されます。</span><span class="sxs-lookup"><span data-stu-id="e3923-113">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="e3923-114">ことは、数分後にアプリケーションまたはメンバーシップの割り当てをグループ化は、リソースから削除されている場合に、拒否されたユーザーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3923-114">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="e3923-115">レビューを適用するか、適用を選択すると、構成されている自動設置ディレクトリ内から発信されたグループまたは動的グループに影響がありません。</span><span class="sxs-lookup"><span data-stu-id="e3923-115">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="e3923-116">設置型の作成元のグループを変更する場合は、結果をダウンロードし、そのディレクトリ内のグループの形式にこれらの変更を適用します。</span><span class="sxs-lookup"><span data-stu-id="e3923-116">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="e3923-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3923-117">Permissions</span></span>
<span data-ttu-id="e3923-p107">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3923-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3923-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3923-120">Permission type</span></span>                        | <span data-ttu-id="e3923-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3923-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3923-122">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3923-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3923-123">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3923-123">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e3923-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3923-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3923-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3923-125">Not supported.</span></span> |
|<span data-ttu-id="e3923-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3923-126">Application</span></span>                            | <span data-ttu-id="e3923-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3923-127">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3923-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3923-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="e3923-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3923-129">Request headers</span></span>
| <span data-ttu-id="e3923-130">名前</span><span class="sxs-lookup"><span data-stu-id="e3923-130">Name</span></span>         | <span data-ttu-id="e3923-131">種類</span><span class="sxs-lookup"><span data-stu-id="e3923-131">Type</span></span>        | <span data-ttu-id="e3923-132">説明</span><span class="sxs-lookup"><span data-stu-id="e3923-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3923-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3923-133">Authorization</span></span> | <span data-ttu-id="e3923-134">string</span><span class="sxs-lookup"><span data-stu-id="e3923-134">string</span></span> | <span data-ttu-id="e3923-135">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="e3923-135">Bearer \{token\}.</span></span> <span data-ttu-id="e3923-136">必須。</span><span class="sxs-lookup"><span data-stu-id="e3923-136">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3923-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3923-137">Request body</span></span>
<span data-ttu-id="e3923-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3923-138">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e3923-139">応答</span><span class="sxs-lookup"><span data-stu-id="e3923-139">Response</span></span>
<span data-ttu-id="e3923-p109">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e3923-p109">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="e3923-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3923-142">See also</span></span>

- [<span data-ttu-id="e3923-143">アクセス確認を実行する方法</span><span class="sxs-lookup"><span data-stu-id="e3923-143">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="e3923-144">例</span><span class="sxs-lookup"><span data-stu-id="e3923-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3923-145">要求</span><span class="sxs-lookup"><span data-stu-id="e3923-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="e3923-146">応答</span><span class="sxs-lookup"><span data-stu-id="e3923-146">Response</span></span>
><span data-ttu-id="e3923-p110">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3923-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
