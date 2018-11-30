---
title: PrivilegedRoleSettings を更新します。
description: 役割の設定を特定の役割の設定を更新します。 PrivilegedRoleSettings オブジェクトが返されます。
ms.openlocfilehash: 0e0f6b7253a1c1d8570c0b91fac4b08bbd39dfff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073710"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="6a1c2-104">PrivilegedRoleSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-104">Update privilegedRoleSettings</span></span>

> <span data-ttu-id="6a1c2-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a1c2-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a1c2-107">役割の設定を特定の役割の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-107">Update the role settings for the given role setting.</span></span> <span data-ttu-id="6a1c2-108">[PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a1c2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a1c2-109">Permissions</span></span>

<span data-ttu-id="6a1c2-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="6a1c2-112">**注:** 依頼者は、次のロールのいずれかの必要があります: ロールの権限を持つ管理者、グローバル管理者、セキュリティ管理者、またはセキュリティのリーダーです。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-112">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="6a1c2-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a1c2-113">Permission type</span></span>      | <span data-ttu-id="6a1c2-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a1c2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a1c2-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a1c2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6a1c2-116">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a1c2-116">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a1c2-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a1c2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a1c2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-118">Not supported.</span></span>    |
|<span data-ttu-id="6a1c2-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a1c2-119">Application</span></span> | <span data-ttu-id="6a1c2-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a1c2-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a1c2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="6a1c2-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a1c2-122">Request headers</span></span>
| <span data-ttu-id="6a1c2-123">名前</span><span class="sxs-lookup"><span data-stu-id="6a1c2-123">Name</span></span>      |<span data-ttu-id="6a1c2-124">説明</span><span class="sxs-lookup"><span data-stu-id="6a1c2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a1c2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a1c2-125">Authorization</span></span>  | <span data-ttu-id="6a1c2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a1c2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a1c2-128">Request body</span></span>
<span data-ttu-id="6a1c2-129">要求の本文には、 [privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-129">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="6a1c2-130">役割の設定を更新するときは指定するプロパティを次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-130">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="6a1c2-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a1c2-131">Property</span></span>|<span data-ttu-id="6a1c2-132">型</span><span class="sxs-lookup"><span data-stu-id="6a1c2-132">Type</span></span>|<span data-ttu-id="6a1c2-133">説明</span><span class="sxs-lookup"><span data-stu-id="6a1c2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a1c2-134">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="6a1c2-134">elevationDuration</span></span>|<span data-ttu-id="6a1c2-135">duration</span><span class="sxs-lookup"><span data-stu-id="6a1c2-135">duration</span></span>|<span data-ttu-id="6a1c2-136">ロールが有効な場合の期間です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-136">The duration when the role is activated.</span></span> <span data-ttu-id="6a1c2-137">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-137">Required.</span></span>|
|<span data-ttu-id="6a1c2-138">ID</span><span class="sxs-lookup"><span data-stu-id="6a1c2-138">id</span></span>|<span data-ttu-id="6a1c2-139">文字列</span><span class="sxs-lookup"><span data-stu-id="6a1c2-139">string</span></span>|<span data-ttu-id="6a1c2-140">ロールの設定の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-140">The unique identifier for the role settings.</span></span> <span data-ttu-id="6a1c2-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-141">Read-only.</span></span> <span data-ttu-id="6a1c2-142">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-142">Required.</span></span>|
|<span data-ttu-id="6a1c2-143">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="6a1c2-143">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="6a1c2-144">ブール</span><span class="sxs-lookup"><span data-stu-id="6a1c2-144">boolean</span></span>|<span data-ttu-id="6a1c2-145">**真**mfaOnElevation は、構成可能な場合です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-145">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="6a1c2-146">場合は**false を指定**mfaOnElevation は構成できません。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-146">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="6a1c2-147">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-147">Required.</span></span>|
|<span data-ttu-id="6a1c2-148">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="6a1c2-148">lastGlobalAdmin</span></span>|<span data-ttu-id="6a1c2-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a1c2-149">Boolean</span></span>|<span data-ttu-id="6a1c2-150">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-150">For internal use only.</span></span>|
|<span data-ttu-id="6a1c2-151">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="6a1c2-151">maxElavationDuration</span></span>|<span data-ttu-id="6a1c2-152">duration</span><span class="sxs-lookup"><span data-stu-id="6a1c2-152">duration</span></span>|<span data-ttu-id="6a1c2-153">アクティブ化されたロールの最大の期間です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-153">Maximum duration for the activated role.</span></span> <span data-ttu-id="6a1c2-154">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-154">Required.</span></span>|
|<span data-ttu-id="6a1c2-155">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a1c2-155">mfaOnElevation</span></span>|<span data-ttu-id="6a1c2-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a1c2-156">Boolean</span></span>|<span data-ttu-id="6a1c2-157">**true** MFA は、ロールをアクティブにするために必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-157">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="6a1c2-158">**false**場合は、MFA は、ロールをアクティブにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-158">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="6a1c2-159">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-159">Required.</span></span>|
|<span data-ttu-id="6a1c2-160">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="6a1c2-160">minElevationDuration</span></span>|<span data-ttu-id="6a1c2-161">duration</span><span class="sxs-lookup"><span data-stu-id="6a1c2-161">duration</span></span>|<span data-ttu-id="6a1c2-162">アクティブ化されたロールの最小の期間です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-162">Minimum duration for the activated role.</span></span> <span data-ttu-id="6a1c2-163">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-163">Required.</span></span>|
|<span data-ttu-id="6a1c2-164">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a1c2-164">notificationToUserOnElevation</span></span>|<span data-ttu-id="6a1c2-165">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a1c2-165">Boolean</span></span>|<span data-ttu-id="6a1c2-166">**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-166">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="6a1c2-167">**false**場合は、ロールがアクティブになったときに通知を送信できません。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-167">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="6a1c2-168">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-168">Required.</span></span>|
|<span data-ttu-id="6a1c2-169">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a1c2-169">ticketingInfoOnElevation</span></span>|<span data-ttu-id="6a1c2-170">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a1c2-170">Boolean</span></span>|<span data-ttu-id="6a1c2-171">**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-171">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="6a1c2-172">**false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-172">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="6a1c2-173">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-173">Required.</span></span>|
|<span data-ttu-id="6a1c2-174">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a1c2-174">approvalOnElevation</span></span>|<span data-ttu-id="6a1c2-175">ブール値</span><span class="sxs-lookup"><span data-stu-id="6a1c2-175">Boolean</span></span>|<span data-ttu-id="6a1c2-176">**true の**場合は、承認が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-176">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="6a1c2-177">**false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-177">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="6a1c2-178">必須。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-178">Required.</span></span>|
|<span data-ttu-id="6a1c2-179">approverIds</span><span class="sxs-lookup"><span data-stu-id="6a1c2-179">approverIds</span></span>|<span data-ttu-id="6a1c2-180">配列</span><span class="sxs-lookup"><span data-stu-id="6a1c2-180">array</span></span>|<span data-ttu-id="6a1c2-181">承認 Id、ライセンス認証の必要な場合は承認の一覧です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-181">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="6a1c2-182">応答</span><span class="sxs-lookup"><span data-stu-id="6a1c2-182">Response</span></span>

<span data-ttu-id="6a1c2-183">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-183">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="6a1c2-184">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-184">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6a1c2-185">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-185">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6a1c2-186">例</span><span class="sxs-lookup"><span data-stu-id="6a1c2-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a1c2-187">要求</span><span class="sxs-lookup"><span data-stu-id="6a1c2-187">Request</span></span>
<span data-ttu-id="6a1c2-188">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-188">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6a1c2-189">応答</span><span class="sxs-lookup"><span data-stu-id="6a1c2-189">Response</span></span>
<span data-ttu-id="6a1c2-190">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6a1c2-190">Here is an example of the response.</span></span>

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
