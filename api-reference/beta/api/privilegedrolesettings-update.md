---
title: PrivilegedRoleSettings を更新します。
description: 役割の設定を特定の役割の設定を更新します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: 7b49d228372e2fa122f9461706f782c60cfea379
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577271"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="1bc8f-104">PrivilegedRoleSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bc8f-105">役割の設定を特定の役割の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="1bc8f-106">[PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="1bc8f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1bc8f-107">Permissions</span></span>

<span data-ttu-id="1bc8f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="1bc8f-110">**注:** 依頼者は、次のロールのいずれかの必要があります: ロールの権限を持つ管理者、グローバル管理者、セキュリティ管理者、またはセキュリティのリーダーです。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="1bc8f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1bc8f-111">Permission type</span></span>      | <span data-ttu-id="1bc8f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1bc8f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bc8f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1bc8f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1bc8f-114">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1bc8f-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1bc8f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1bc8f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bc8f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-116">Not supported.</span></span>    |
|<span data-ttu-id="1bc8f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1bc8f-117">Application</span></span> | <span data-ttu-id="1bc8f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bc8f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1bc8f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="1bc8f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1bc8f-120">Request headers</span></span>
| <span data-ttu-id="1bc8f-121">名前</span><span class="sxs-lookup"><span data-stu-id="1bc8f-121">Name</span></span>      |<span data-ttu-id="1bc8f-122">説明</span><span class="sxs-lookup"><span data-stu-id="1bc8f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1bc8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bc8f-123">Authorization</span></span>  | <span data-ttu-id="1bc8f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bc8f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1bc8f-126">Request body</span></span>
<span data-ttu-id="1bc8f-127">要求の本文には、 [privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="1bc8f-128">役割の設定を更新するときは指定するプロパティを次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="1bc8f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1bc8f-129">Property</span></span>|<span data-ttu-id="1bc8f-130">型</span><span class="sxs-lookup"><span data-stu-id="1bc8f-130">Type</span></span>|<span data-ttu-id="1bc8f-131">説明</span><span class="sxs-lookup"><span data-stu-id="1bc8f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bc8f-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="1bc8f-132">elevationDuration</span></span> |<span data-ttu-id="1bc8f-133">文字列 (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="1bc8f-133">String (timestamp)</span></span> |<span data-ttu-id="1bc8f-134">ロールが有効な場合の期間です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-134">The duration when the role is activated.</span></span> <span data-ttu-id="1bc8f-135">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-135">Required.</span></span>|
|<span data-ttu-id="1bc8f-136">id</span><span class="sxs-lookup"><span data-stu-id="1bc8f-136">id</span></span>| <span data-ttu-id="1bc8f-137">文字列 (識別子)</span><span class="sxs-lookup"><span data-stu-id="1bc8f-137">string (identifier)</span></span> |<span data-ttu-id="1bc8f-138">ロールの設定の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="1bc8f-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-139">Read-only.</span></span> <span data-ttu-id="1bc8f-140">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-140">Required.</span></span>|
|<span data-ttu-id="1bc8f-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="1bc8f-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="1bc8f-142">boolean</span><span class="sxs-lookup"><span data-stu-id="1bc8f-142">boolean</span></span>|<span data-ttu-id="1bc8f-143">**真**mfaOnElevation は、構成可能な場合です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="1bc8f-144">場合は**false を指定**mfaOnElevation は構成できません。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="1bc8f-145">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-145">Required.</span></span>|
|<span data-ttu-id="1bc8f-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="1bc8f-146">lastGlobalAdmin</span></span>| <span data-ttu-id="1bc8f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bc8f-147">Boolean</span></span> |<span data-ttu-id="1bc8f-148">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-148">For internal use only.</span></span>|
|<span data-ttu-id="1bc8f-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="1bc8f-149">maxElavationDuration</span></span>| <span data-ttu-id="1bc8f-150">文字列 (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="1bc8f-150">String (timestamp)</span></span>|<span data-ttu-id="1bc8f-151">アクティブ化されたロールの最大の期間です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="1bc8f-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-152">Required.</span></span>|
|<span data-ttu-id="1bc8f-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="1bc8f-153">mfaOnElevation</span></span>| <span data-ttu-id="1bc8f-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bc8f-154">Boolean</span></span> |<span data-ttu-id="1bc8f-155">**true** MFA は、ロールをアクティブにするために必要な場合です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="1bc8f-156">**false**場合は、MFA は、ロールをアクティブにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="1bc8f-157">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-157">Required.</span></span>|
|<span data-ttu-id="1bc8f-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="1bc8f-158">minElevationDuration</span></span>| <span data-ttu-id="1bc8f-159">文字列 (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="1bc8f-159">String (timestamp)</span></span> |<span data-ttu-id="1bc8f-160">アクティブ化されたロールの最小の期間です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="1bc8f-161">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-161">Required.</span></span>|
|<span data-ttu-id="1bc8f-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="1bc8f-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="1bc8f-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bc8f-163">Boolean</span></span>|<span data-ttu-id="1bc8f-164">**true**の場合、ロールがアクティブになったときは、エンド ・ ユーザーに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="1bc8f-165">**false**場合は、ロールがアクティブになったときに通知を送信できません。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="1bc8f-166">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-166">Required.</span></span>|
|<span data-ttu-id="1bc8f-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="1bc8f-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="1bc8f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bc8f-168">Boolean</span></span>|<span data-ttu-id="1bc8f-169">**true の**場合は、チケット情報が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="1bc8f-170">**false**場合、チケットの情報が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="1bc8f-171">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-171">Required.</span></span>|
|<span data-ttu-id="1bc8f-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="1bc8f-172">approvalOnElevation</span></span>|<span data-ttu-id="1bc8f-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bc8f-173">Boolean</span></span>|<span data-ttu-id="1bc8f-174">**true の**場合は、承認が必要な場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="1bc8f-175">**false を指定**する場合、承認が必要ない場合は、ロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="1bc8f-176">必須です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-176">Required.</span></span>|
|<span data-ttu-id="1bc8f-177">approverIds</span><span class="sxs-lookup"><span data-stu-id="1bc8f-177">approverIds</span></span>| <span data-ttu-id="1bc8f-178">文字列 (識別子) のコレクション</span><span class="sxs-lookup"><span data-stu-id="1bc8f-178">String (identifier) collection</span></span>|<span data-ttu-id="1bc8f-179">承認 Id、ライセンス認証の必要な場合は承認の一覧です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="1bc8f-180">応答</span><span class="sxs-lookup"><span data-stu-id="1bc8f-180">Response</span></span>

<span data-ttu-id="1bc8f-181">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="1bc8f-182">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="1bc8f-183">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="1bc8f-184">例</span><span class="sxs-lookup"><span data-stu-id="1bc8f-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bc8f-185">要求</span><span class="sxs-lookup"><span data-stu-id="1bc8f-185">Request</span></span>
<span data-ttu-id="1bc8f-186">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-186">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1bc8f-187">応答</span><span class="sxs-lookup"><span data-stu-id="1bc8f-187">Response</span></span>
<span data-ttu-id="1bc8f-188">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1bc8f-188">Here is an example of the response.</span></span>

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
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
