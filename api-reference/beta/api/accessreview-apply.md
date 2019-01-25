---
title: AccessReview を適用します。
description: 'Azure AD のレビュー機能にアクセス、完成した accessReview の決定を適用します。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512214"
---
# <a name="apply-accessreview"></a><span data-ttu-id="863df-104">AccessReview を適用します。</span><span class="sxs-lookup"><span data-stu-id="863df-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863df-105">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、完成した[accessReview](../resources/accessreview.md)の決定を適用します。</span><span class="sxs-lookup"><span data-stu-id="863df-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="863df-106">ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="863df-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="863df-107">アクセス確認が完了したら、いずれかの終了日に到達したか、または管理者が手動で停止しているし、自動適用ためにでしたように構成されて、確認のため、変更を適用する適用を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="863df-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="863df-108">適用が行われるまでアクセス権を削除するのには意思決定には表示されませんソース リソースをユーザーがインスタンスにそれらのグループ メンバーシップを保持します。</span><span class="sxs-lookup"><span data-stu-id="863df-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="863df-109">呼び出すことによって適用、レビューの結果は、グループまたはアプリケーションを更新することによって実装されています。</span><span class="sxs-lookup"><span data-stu-id="863df-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="863df-110">ユーザーのアクセスが拒否された場合、レビューに管理者は、この API を呼び出すときに、Azure の AD は、メンバーシップ、またはアプリケーションの割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="863df-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="863df-111">アクセス確認が終了したら、自動適用後に構成していたレビューのステータスが完了から、中間の状態が変更され、最後に適用の状態に変更されます。</span><span class="sxs-lookup"><span data-stu-id="863df-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="863df-112">ことは、数分後にアプリケーションまたはメンバーシップの割り当てをグループ化は、リソースから削除されている場合に、拒否されたユーザーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="863df-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="863df-113">レビューを適用するか、適用を選択すると、構成されている自動設置ディレクトリ内から発信されたグループまたは動的グループに影響がありません。</span><span class="sxs-lookup"><span data-stu-id="863df-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="863df-114">設置型の作成元のグループを変更する場合は、結果をダウンロードし、そのディレクトリ内のグループの形式にこれらの変更を適用します。</span><span class="sxs-lookup"><span data-stu-id="863df-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="863df-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="863df-115">Permissions</span></span>
<span data-ttu-id="863df-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="863df-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="863df-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="863df-118">Permission type</span></span>                        | <span data-ttu-id="863df-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="863df-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="863df-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="863df-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="863df-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="863df-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="863df-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="863df-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="863df-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="863df-123">Not supported.</span></span> |
|<span data-ttu-id="863df-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="863df-124">Application</span></span>                            | <span data-ttu-id="863df-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="863df-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="863df-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="863df-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="863df-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="863df-127">Request headers</span></span>
| <span data-ttu-id="863df-128">名前</span><span class="sxs-lookup"><span data-stu-id="863df-128">Name</span></span>         | <span data-ttu-id="863df-129">型</span><span class="sxs-lookup"><span data-stu-id="863df-129">Type</span></span>        | <span data-ttu-id="863df-130">説明</span><span class="sxs-lookup"><span data-stu-id="863df-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="863df-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="863df-131">Authorization</span></span> | <span data-ttu-id="863df-132">string</span><span class="sxs-lookup"><span data-stu-id="863df-132">string</span></span> | <span data-ttu-id="863df-133">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="863df-133">Bearer \{token\}.</span></span> <span data-ttu-id="863df-134">必須です。</span><span class="sxs-lookup"><span data-stu-id="863df-134">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="863df-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="863df-135">Request body</span></span>
<span data-ttu-id="863df-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="863df-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="863df-137">応答</span><span class="sxs-lookup"><span data-stu-id="863df-137">Response</span></span>
<span data-ttu-id="863df-p108">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="863df-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="863df-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="863df-140">See also</span></span>

- [<span data-ttu-id="863df-141">アクセス確認を実行する方法</span><span class="sxs-lookup"><span data-stu-id="863df-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="863df-142">例</span><span class="sxs-lookup"><span data-stu-id="863df-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="863df-143">要求</span><span class="sxs-lookup"><span data-stu-id="863df-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="863df-144">応答</span><span class="sxs-lookup"><span data-stu-id="863df-144">Response</span></span>
><span data-ttu-id="863df-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="863df-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
