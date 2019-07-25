---
title: AccessReview を適用する
description: 'Azure AD access レビュー機能で、完了した accessReview の決定を適用します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a4c94406afbba762f3c461c06f9ba8252a3cbbc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856244"
---
# <a name="apply-accessreview"></a><span data-ttu-id="1c027-104">AccessReview を適用する</span><span class="sxs-lookup"><span data-stu-id="1c027-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c027-105">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、完了した[accessreview](../resources/accessreview.md)の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="1c027-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="1c027-106">ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="1c027-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="1c027-107">終了日に達したか、管理者が手動で停止したためにアクセスレビューが終了し、レビューのために自動適用が構成されていない場合は、[適用] を呼び出して変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="1c027-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="1c027-108">適用が行われるまで、アクセス権を削除するための決定はソースリソースに表示されず、インスタンスのユーザーはグループメンバーシップを保持します。</span><span class="sxs-lookup"><span data-stu-id="1c027-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="1c027-109">[適用] を呼び出すと、レビューの結果が、グループまたはアプリケーションを更新することによって実装されます。</span><span class="sxs-lookup"><span data-stu-id="1c027-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="1c027-110">ユーザーのアクセスがレビューで拒否された場合、管理者がこの API を呼び出すと、Azure AD はそれらのメンバーシップまたはアプリケーション割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="1c027-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="1c027-111">アクセスレビューが完了し、自動適用が構成されると、レビューの状態は [完了] から [中間状態] に変わり、最後に [適用済みの状態] に変わります。</span><span class="sxs-lookup"><span data-stu-id="1c027-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="1c027-112">却下されたユーザーが存在する場合は、リソースグループのメンバーシップまたはアプリの割り当てから数分で削除されることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c027-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="1c027-113">構成済みの自動適用レビュー、または [適用] を選択しても、オンプレミスディレクトリまたは動的グループで発生するグループには影響しません。</span><span class="sxs-lookup"><span data-stu-id="1c027-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="1c027-114">オンプレミスで発生したグループを変更する場合は、結果をダウンロードして、そのディレクトリ内のグループの表現にその変更を適用します。</span><span class="sxs-lookup"><span data-stu-id="1c027-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="1c027-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c027-115">Permissions</span></span>
<span data-ttu-id="1c027-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c027-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c027-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c027-118">Permission type</span></span>                        | <span data-ttu-id="1c027-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c027-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c027-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c027-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c027-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c027-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1c027-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c027-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c027-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c027-123">Not supported.</span></span> |
|<span data-ttu-id="1c027-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c027-124">Application</span></span>                            | <span data-ttu-id="1c027-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c027-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c027-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c027-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="1c027-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c027-127">Request headers</span></span>
| <span data-ttu-id="1c027-128">名前</span><span class="sxs-lookup"><span data-stu-id="1c027-128">Name</span></span>         | <span data-ttu-id="1c027-129">型</span><span class="sxs-lookup"><span data-stu-id="1c027-129">Type</span></span>        | <span data-ttu-id="1c027-130">説明</span><span class="sxs-lookup"><span data-stu-id="1c027-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1c027-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c027-131">Authorization</span></span> | <span data-ttu-id="1c027-132">string</span><span class="sxs-lookup"><span data-stu-id="1c027-132">string</span></span> | <span data-ttu-id="1c027-p107">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c027-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c027-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c027-135">Request body</span></span>
<span data-ttu-id="1c027-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1c027-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1c027-137">応答</span><span class="sxs-lookup"><span data-stu-id="1c027-137">Response</span></span>
<span data-ttu-id="1c027-p108">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1c027-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="1c027-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c027-140">See also</span></span>

- [<span data-ttu-id="1c027-141">アクセスレビューを完了する方法</span><span class="sxs-lookup"><span data-stu-id="1c027-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="1c027-142">例</span><span class="sxs-lookup"><span data-stu-id="1c027-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c027-143">要求</span><span class="sxs-lookup"><span data-stu-id="1c027-143">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c027-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1c027-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c027-145">C#</span><span class="sxs-lookup"><span data-stu-id="1c027-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c027-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c027-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c027-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="1c027-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c027-148">Java</span><span class="sxs-lookup"><span data-stu-id="1c027-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c027-149">応答</span><span class="sxs-lookup"><span data-stu-id="1c027-149">Response</span></span>
><span data-ttu-id="1c027-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1c027-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
