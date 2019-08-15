---
title: PrivilegedRoleSettings の更新
description: 指定した役割設定の役割設定を更新します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef9b8db2f4e0d580ec136caa7d827d19f22d6929
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412587"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="900be-104">PrivilegedRoleSettings の更新</span><span class="sxs-lookup"><span data-stu-id="900be-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="900be-105">指定した役割設定の役割設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="900be-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="900be-106">[PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="900be-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="900be-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="900be-107">Permissions</span></span>

<span data-ttu-id="900be-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="900be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="900be-110">**注:** 要求者は、特権ロール管理者、全体管理者、セキュリティ管理者、またはセキュリティ閲覧者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="900be-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="900be-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="900be-111">Permission type</span></span>      | <span data-ttu-id="900be-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="900be-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="900be-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="900be-113">Delegated (work or school account)</span></span> | <span data-ttu-id="900be-114">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="900be-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="900be-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="900be-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="900be-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="900be-116">Not supported.</span></span>    |
|<span data-ttu-id="900be-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="900be-117">Application</span></span> | <span data-ttu-id="900be-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="900be-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="900be-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="900be-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="900be-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="900be-120">Request headers</span></span>
| <span data-ttu-id="900be-121">名前</span><span class="sxs-lookup"><span data-stu-id="900be-121">Name</span></span>      |<span data-ttu-id="900be-122">説明</span><span class="sxs-lookup"><span data-stu-id="900be-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="900be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="900be-123">Authorization</span></span>  | <span data-ttu-id="900be-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="900be-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="900be-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="900be-126">Request body</span></span>
<span data-ttu-id="900be-127">要求本文で、 [privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="900be-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="900be-128">次の表に、役割の設定を更新するときに指定できるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="900be-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="900be-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="900be-129">Property</span></span>|<span data-ttu-id="900be-130">型</span><span class="sxs-lookup"><span data-stu-id="900be-130">Type</span></span>|<span data-ttu-id="900be-131">説明</span><span class="sxs-lookup"><span data-stu-id="900be-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="900be-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="900be-132">elevationDuration</span></span>|<span data-ttu-id="900be-133">duration</span><span class="sxs-lookup"><span data-stu-id="900be-133">duration</span></span>|<span data-ttu-id="900be-134">役割がアクティブ化される期間。</span><span class="sxs-lookup"><span data-stu-id="900be-134">The duration when the role is activated.</span></span> <span data-ttu-id="900be-135">必須。</span><span class="sxs-lookup"><span data-stu-id="900be-135">Required.</span></span>|
|<span data-ttu-id="900be-136">id</span><span class="sxs-lookup"><span data-stu-id="900be-136">id</span></span>|<span data-ttu-id="900be-137">string</span><span class="sxs-lookup"><span data-stu-id="900be-137">string</span></span>|<span data-ttu-id="900be-138">ロール設定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="900be-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="900be-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="900be-139">Read-only.</span></span> <span data-ttu-id="900be-140">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-140">Required.</span></span>|
|<span data-ttu-id="900be-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="900be-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="900be-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="900be-142">boolean</span></span>|<span data-ttu-id="900be-143">**true**の場合は、mfaOnElevation を構成できます。</span><span class="sxs-lookup"><span data-stu-id="900be-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="900be-144">mfaOnElevation を構成できない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="900be-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="900be-145">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-145">Required.</span></span>|
|<span data-ttu-id="900be-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="900be-146">lastGlobalAdmin</span></span>|<span data-ttu-id="900be-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="900be-147">Boolean</span></span>|<span data-ttu-id="900be-148">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="900be-148">For internal use only.</span></span>|
|<span data-ttu-id="900be-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="900be-149">maxElavationDuration</span></span>|<span data-ttu-id="900be-150">duration</span><span class="sxs-lookup"><span data-stu-id="900be-150">duration</span></span>|<span data-ttu-id="900be-151">アクティブ化されたロールの最大期間。</span><span class="sxs-lookup"><span data-stu-id="900be-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="900be-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-152">Required.</span></span>|
|<span data-ttu-id="900be-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="900be-153">mfaOnElevation</span></span>|<span data-ttu-id="900be-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="900be-154">Boolean</span></span>|<span data-ttu-id="900be-155">役割をアクティブ化するために MFA が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="900be-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="900be-156">役割をアクティブ化するために MFA が必要でない場合は**false** 。</span><span class="sxs-lookup"><span data-stu-id="900be-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="900be-157">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-157">Required.</span></span>|
|<span data-ttu-id="900be-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="900be-158">minElevationDuration</span></span>|<span data-ttu-id="900be-159">duration</span><span class="sxs-lookup"><span data-stu-id="900be-159">duration</span></span>|<span data-ttu-id="900be-160">アクティブ化されたロールの最小期間。</span><span class="sxs-lookup"><span data-stu-id="900be-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="900be-161">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-161">Required.</span></span>|
|<span data-ttu-id="900be-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="900be-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="900be-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="900be-163">Boolean</span></span>|<span data-ttu-id="900be-164">**true**の場合は、エンドユーザーに役割がアクティブ化されたときに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="900be-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="900be-165">**true**の場合は、役割がアクティブ化されたときに通知を送信しません。</span><span class="sxs-lookup"><span data-stu-id="900be-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="900be-166">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-166">Required.</span></span>|
|<span data-ttu-id="900be-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="900be-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="900be-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="900be-168">Boolean</span></span>|<span data-ttu-id="900be-169">役割をアクティブ化するときに、チケット情報が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="900be-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="900be-170">**false**を指定すると、役割をアクティブ化するときに、チケットの情報は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="900be-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="900be-171">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-171">Required.</span></span>|
|<span data-ttu-id="900be-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="900be-172">approvalOnElevation</span></span>|<span data-ttu-id="900be-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="900be-173">Boolean</span></span>|<span data-ttu-id="900be-174">ロールをアクティブ化するときに承認が必要な場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="900be-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="900be-175">**false**を指定すると、役割をアクティブ化するときに承認が必要ありません。</span><span class="sxs-lookup"><span data-stu-id="900be-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="900be-176">必須です。</span><span class="sxs-lookup"><span data-stu-id="900be-176">Required.</span></span>|
|<span data-ttu-id="900be-177">承認の検証 Ds</span><span class="sxs-lookup"><span data-stu-id="900be-177">approverIds</span></span>|<span data-ttu-id="900be-178">string collection</span><span class="sxs-lookup"><span data-stu-id="900be-178">string collection</span></span>|<span data-ttu-id="900be-179">ライセンス認証に承認が必要な場合は、承認 Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="900be-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="900be-180">応答</span><span class="sxs-lookup"><span data-stu-id="900be-180">Response</span></span>

<span data-ttu-id="900be-181">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="900be-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="900be-182">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="900be-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="900be-183">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="900be-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="900be-184">例</span><span class="sxs-lookup"><span data-stu-id="900be-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="900be-185">要求</span><span class="sxs-lookup"><span data-stu-id="900be-185">Request</span></span>
<span data-ttu-id="900be-186">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="900be-186">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="900be-187">プロトコル</span><span class="sxs-lookup"><span data-stu-id="900be-187">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="900be-188">C#</span><span class="sxs-lookup"><span data-stu-id="900be-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="900be-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="900be-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="900be-190">目的-C</span><span class="sxs-lookup"><span data-stu-id="900be-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="900be-191">応答</span><span class="sxs-lookup"><span data-stu-id="900be-191">Response</span></span>
<span data-ttu-id="900be-192">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="900be-192">Here is an example of the response.</span></span>
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
