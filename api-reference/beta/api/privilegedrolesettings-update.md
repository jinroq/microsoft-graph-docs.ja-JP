---
title: PrivilegedRoleSettings の更新
description: 指定した役割設定の役割設定を更新します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f42dca2f592f13bc195c82b234854804ceb864e2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360940"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="c90da-104">PrivilegedRoleSettings の更新</span><span class="sxs-lookup"><span data-stu-id="c90da-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c90da-105">指定した役割設定の役割設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="c90da-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="c90da-106">[PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="c90da-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="c90da-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c90da-107">Permissions</span></span>

<span data-ttu-id="c90da-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c90da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="c90da-110">**注:** 要求者は、特権ロール管理者、全体管理者、セキュリティ管理者、またはセキュリティ閲覧者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c90da-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="c90da-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c90da-111">Permission type</span></span>      | <span data-ttu-id="c90da-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c90da-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c90da-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c90da-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c90da-114">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="c90da-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c90da-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c90da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c90da-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c90da-116">Not supported.</span></span>    |
|<span data-ttu-id="c90da-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c90da-117">Application</span></span> | <span data-ttu-id="c90da-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c90da-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c90da-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c90da-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="c90da-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c90da-120">Request headers</span></span>
| <span data-ttu-id="c90da-121">名前</span><span class="sxs-lookup"><span data-stu-id="c90da-121">Name</span></span>      |<span data-ttu-id="c90da-122">説明</span><span class="sxs-lookup"><span data-stu-id="c90da-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c90da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c90da-123">Authorization</span></span>  | <span data-ttu-id="c90da-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c90da-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c90da-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c90da-126">Request body</span></span>
<span data-ttu-id="c90da-127">要求本文で、 [privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c90da-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="c90da-128">次の表に、役割の設定を更新するときに指定できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c90da-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="c90da-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c90da-129">Property</span></span>|<span data-ttu-id="c90da-130">型</span><span class="sxs-lookup"><span data-stu-id="c90da-130">Type</span></span>|<span data-ttu-id="c90da-131">説明</span><span class="sxs-lookup"><span data-stu-id="c90da-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c90da-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="c90da-132">elevationDuration</span></span>|<span data-ttu-id="c90da-133">duration</span><span class="sxs-lookup"><span data-stu-id="c90da-133">duration</span></span>|<span data-ttu-id="c90da-134">役割がアクティブ化される期間。</span><span class="sxs-lookup"><span data-stu-id="c90da-134">The duration when the role is activated.</span></span> <span data-ttu-id="c90da-135">必須。</span><span class="sxs-lookup"><span data-stu-id="c90da-135">Required.</span></span>|
|<span data-ttu-id="c90da-136">id</span><span class="sxs-lookup"><span data-stu-id="c90da-136">id</span></span>|<span data-ttu-id="c90da-137">string</span><span class="sxs-lookup"><span data-stu-id="c90da-137">string</span></span>|<span data-ttu-id="c90da-138">ロール設定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="c90da-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="c90da-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c90da-139">Read-only.</span></span> <span data-ttu-id="c90da-140">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-140">Required.</span></span>|
|<span data-ttu-id="c90da-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="c90da-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="c90da-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="c90da-142">boolean</span></span>|<span data-ttu-id="c90da-143">**true**の場合は、mfaOnElevation を構成できます。</span><span class="sxs-lookup"><span data-stu-id="c90da-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="c90da-144">mfaOnElevation を構成できない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="c90da-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="c90da-145">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-145">Required.</span></span>|
|<span data-ttu-id="c90da-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="c90da-146">lastGlobalAdmin</span></span>|<span data-ttu-id="c90da-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c90da-147">Boolean</span></span>|<span data-ttu-id="c90da-148">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="c90da-148">For internal use only.</span></span>|
|<span data-ttu-id="c90da-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="c90da-149">maxElavationDuration</span></span>|<span data-ttu-id="c90da-150">duration</span><span class="sxs-lookup"><span data-stu-id="c90da-150">duration</span></span>|<span data-ttu-id="c90da-151">アクティブ化されたロールの最大期間。</span><span class="sxs-lookup"><span data-stu-id="c90da-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="c90da-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-152">Required.</span></span>|
|<span data-ttu-id="c90da-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="c90da-153">mfaOnElevation</span></span>|<span data-ttu-id="c90da-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c90da-154">Boolean</span></span>|<span data-ttu-id="c90da-155">役割をアクティブ化するために MFA が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="c90da-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="c90da-156">役割をアクティブ化するために MFA が必要でない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="c90da-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="c90da-157">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-157">Required.</span></span>|
|<span data-ttu-id="c90da-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="c90da-158">minElevationDuration</span></span>|<span data-ttu-id="c90da-159">duration</span><span class="sxs-lookup"><span data-stu-id="c90da-159">duration</span></span>|<span data-ttu-id="c90da-160">アクティブ化されたロールの最小期間。</span><span class="sxs-lookup"><span data-stu-id="c90da-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="c90da-161">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-161">Required.</span></span>|
|<span data-ttu-id="c90da-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="c90da-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="c90da-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c90da-163">Boolean</span></span>|<span data-ttu-id="c90da-164">**true**の場合は、エンドユーザーに役割がアクティブ化されたときに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="c90da-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="c90da-165">**true**の場合は、役割がアクティブ化されたときに通知を送信しません。</span><span class="sxs-lookup"><span data-stu-id="c90da-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="c90da-166">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-166">Required.</span></span>|
|<span data-ttu-id="c90da-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="c90da-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="c90da-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c90da-168">Boolean</span></span>|<span data-ttu-id="c90da-169">役割をアクティブ化するときに、チケット情報が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="c90da-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="c90da-170">**false**を指定すると、役割をアクティブ化するときに、チケットの情報は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="c90da-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="c90da-171">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-171">Required.</span></span>|
|<span data-ttu-id="c90da-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="c90da-172">approvalOnElevation</span></span>|<span data-ttu-id="c90da-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c90da-173">Boolean</span></span>|<span data-ttu-id="c90da-174">ロールをアクティブ化するときに承認が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="c90da-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="c90da-175">**false**を指定すると、役割をアクティブ化するときに承認が必要ありません。</span><span class="sxs-lookup"><span data-stu-id="c90da-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="c90da-176">必須です。</span><span class="sxs-lookup"><span data-stu-id="c90da-176">Required.</span></span>|
|<span data-ttu-id="c90da-177">承認の検証 Ds</span><span class="sxs-lookup"><span data-stu-id="c90da-177">approverIds</span></span>|<span data-ttu-id="c90da-178">string collection</span><span class="sxs-lookup"><span data-stu-id="c90da-178">string collection</span></span>|<span data-ttu-id="c90da-179">ライセンス認証に承認が必要な場合は、承認 Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="c90da-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="c90da-180">応答</span><span class="sxs-lookup"><span data-stu-id="c90da-180">Response</span></span>

<span data-ttu-id="c90da-181">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c90da-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="c90da-182">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c90da-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c90da-183">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c90da-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c90da-184">例</span><span class="sxs-lookup"><span data-stu-id="c90da-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c90da-185">要求</span><span class="sxs-lookup"><span data-stu-id="c90da-185">Request</span></span>
<span data-ttu-id="c90da-186">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c90da-186">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c90da-187">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c90da-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c90da-188">C#</span><span class="sxs-lookup"><span data-stu-id="c90da-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c90da-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c90da-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c90da-190">目的-C</span><span class="sxs-lookup"><span data-stu-id="c90da-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c90da-191">Java</span><span class="sxs-lookup"><span data-stu-id="c90da-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c90da-192">応答</span><span class="sxs-lookup"><span data-stu-id="c90da-192">Response</span></span>
<span data-ttu-id="c90da-193">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c90da-193">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
