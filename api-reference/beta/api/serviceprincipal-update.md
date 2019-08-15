---
title: Serviceprincipal を更新する
description: Serviceprincipal オブジェクトのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 852ea0467779ba0dab80eb0c571f39b1cf60ed9b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410131"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="67d4d-103">Serviceprincipal を更新する</span><span class="sxs-lookup"><span data-stu-id="67d4d-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67d4d-104">Serviceprincipal オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="67d4d-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67d4d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67d4d-105">Permissions</span></span>
<span data-ttu-id="67d4d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67d4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67d4d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67d4d-108">Permission type</span></span>      | <span data-ttu-id="67d4d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67d4d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67d4d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67d4d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67d4d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67d4d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67d4d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67d4d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67d4d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67d4d-113">Not supported.</span></span>    |
|<span data-ttu-id="67d4d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67d4d-114">Application</span></span> | <span data-ttu-id="67d4d-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67d4d-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67d4d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67d4d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="67d4d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67d4d-117">Request headers</span></span>
| <span data-ttu-id="67d4d-118">名前</span><span class="sxs-lookup"><span data-stu-id="67d4d-118">Name</span></span>       | <span data-ttu-id="67d4d-119">型</span><span class="sxs-lookup"><span data-stu-id="67d4d-119">Type</span></span> | <span data-ttu-id="67d4d-120">説明</span><span class="sxs-lookup"><span data-stu-id="67d4d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67d4d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67d4d-121">Authorization</span></span>  | <span data-ttu-id="67d4d-122">string</span><span class="sxs-lookup"><span data-stu-id="67d4d-122">string</span></span>  | <span data-ttu-id="67d4d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67d4d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67d4d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="67d4d-125">Request body</span></span>
<span data-ttu-id="67d4d-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="67d4d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="67d4d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67d4d-129">Property</span></span>     | <span data-ttu-id="67d4d-130">型</span><span class="sxs-lookup"><span data-stu-id="67d4d-130">Type</span></span>   |<span data-ttu-id="67d4d-131">説明</span><span class="sxs-lookup"><span data-stu-id="67d4d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67d4d-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="67d4d-132">accountEnabled</span></span>|<span data-ttu-id="67d4d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="67d4d-133">Boolean</span></span>|                <span data-ttu-id="67d4d-134">サービス プリンシパルのアカウントが有効な場合は **true**。それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="67d4d-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="67d4d-135">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="67d4d-135">appDisplayName</span></span>|<span data-ttu-id="67d4d-136">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-136">String</span></span>|<span data-ttu-id="67d4d-137">関連付けられているアプリケーションによって公開される表示名。</span><span class="sxs-lookup"><span data-stu-id="67d4d-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="67d4d-138">appId</span><span class="sxs-lookup"><span data-stu-id="67d4d-138">appId</span></span>|<span data-ttu-id="67d4d-139">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-139">String</span></span>|<span data-ttu-id="67d4d-140">関連付けられたアプリケーションの一意の識別子 (その **appId** プロパティ)。</span><span class="sxs-lookup"><span data-stu-id="67d4d-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="67d4d-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="67d4d-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="67d4d-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="67d4d-142">Boolean</span></span>|<span data-ttu-id="67d4d-143">Azure AD からアプリケーションにユーザー トークンまたはアクセス トークンが発行される前に、ユーザーまたはグループに対する **appRoleAssignment** が必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="67d4d-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="67d4d-144">**メモ**: null を許容しないバージョン1.5 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="67d4d-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="67d4d-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="67d4d-145">appRoles</span></span>|<span data-ttu-id="67d4d-146">appRole</span><span class="sxs-lookup"><span data-stu-id="67d4d-146">appRole</span></span>|<span data-ttu-id="67d4d-147">関連付けられているアプリケーションによって公開されるアプリケーション ロール。</span><span class="sxs-lookup"><span data-stu-id="67d4d-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="67d4d-148">詳細については\*\*\*\* 、「アプリケーションエンティティ**メモ**: null 値ではなくバージョン1.5 またはそれ以降が必要」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67d4d-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="67d4d-149">displayName</span><span class="sxs-lookup"><span data-stu-id="67d4d-149">displayName</span></span>|<span data-ttu-id="67d4d-150">文字列</span><span class="sxs-lookup"><span data-stu-id="67d4d-150">String</span></span>|<span data-ttu-id="67d4d-151">サービス プリンシパルの表示名。</span><span class="sxs-lookup"><span data-stu-id="67d4d-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="67d4d-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="67d4d-152">errorUrl</span></span>|<span data-ttu-id="67d4d-153">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-153">String</span></span>|            |
|<span data-ttu-id="67d4d-154">HomePage</span><span class="sxs-lookup"><span data-stu-id="67d4d-154">homepage</span></span>|<span data-ttu-id="67d4d-155">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-155">String</span></span>|<span data-ttu-id="67d4d-156">関連付けられているアプリケーションのホームページの URL。</span><span class="sxs-lookup"><span data-stu-id="67d4d-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="67d4d-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="67d4d-157">keyCredentials</span></span>|<span data-ttu-id="67d4d-158">keyCredential</span><span class="sxs-lookup"><span data-stu-id="67d4d-158">keyCredential</span></span>|<span data-ttu-id="67d4d-159">サービス プリンシパルに関連付けられているキー資格情報のコレクションです。null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="67d4d-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="67d4d-160">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="67d4d-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="67d4d-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="67d4d-161">logoutUrl</span></span>|<span data-ttu-id="67d4d-162">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-162">String</span></span>| <span data-ttu-id="67d4d-163">Microsoft の承認サービスで、[フロント チャネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[バック チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウト プロトコルを使ってユーザーのログアウトするのに使う URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="67d4d-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="67d4d-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="67d4d-164">oauth2Permissions</span></span>|<span data-ttu-id="67d4d-165">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="67d4d-165">oAuth2Permission</span></span>|<span data-ttu-id="67d4d-166">関連付けられているアプリケーションによって公開される OAuth 2.0 のアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="67d4d-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="67d4d-167">さらに詳しい情報については、アプリケーション エンティティの **oauth2Permissions** プロパティの定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67d4d-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="67d4d-168">**メモ**: null を許容しないバージョン1.5 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="67d4d-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="67d4d-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="67d4d-169">passwordCredentials</span></span>|<span data-ttu-id="67d4d-170">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="67d4d-170">passwordCredential</span></span>|<span data-ttu-id="67d4d-171">サービス プリンシパルに関連付けられているパスワード資格情報のコレクションです。null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="67d4d-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="67d4d-172">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="67d4d-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="67d4d-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="67d4d-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="67d4d-174">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-174">String</span></span>|<span data-ttu-id="67d4d-175">内部使用専用に予約済みです。</span><span class="sxs-lookup"><span data-stu-id="67d4d-175">Reserved for internal use only.</span></span> <span data-ttu-id="67d4d-176">このプロパティに書き込みしたり、依存したりしないでください。</span><span class="sxs-lookup"><span data-stu-id="67d4d-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="67d4d-177">将来のバージョンで削除される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="67d4d-177">May be removed in future versions.</span></span>                            <span data-ttu-id="67d4d-178">**メモ**: バージョン1.5 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="67d4d-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="67d4d-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="67d4d-179">publisherName</span></span>|<span data-ttu-id="67d4d-180">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-180">String</span></span>|<span data-ttu-id="67d4d-181">関連付けられたアプリケーションが指定されているテナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="67d4d-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="67d4d-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="67d4d-182">replyUrls</span></span>|<span data-ttu-id="67d4d-183">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-183">String</span></span>|<span data-ttu-id="67d4d-184">関連付けられたアプリケーションにサインインするためにユーザー トークンが送信される URL、または関連付けられたアプリケーションに対して OAuth 2.0 認証コードとアクセス トークンが送信されるリダイレクト URI。</span><span class="sxs-lookup"><span data-stu-id="67d4d-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="67d4d-185">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="67d4d-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="67d4d-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="67d4d-186">samlMetadataUrl</span></span>|<span data-ttu-id="67d4d-187">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-187">String</span></span>|            |
|<span data-ttu-id="67d4d-188">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="67d4d-188">servicePrincipalNames</span></span>|<span data-ttu-id="67d4d-189">String</span><span class="sxs-lookup"><span data-stu-id="67d4d-189">String</span></span>|<span data-ttu-id="67d4d-190">関連するアプリケーションを識別する URI です。</span><span class="sxs-lookup"><span data-stu-id="67d4d-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="67d4d-191">詳細については、「[Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://msdn.microsoft.com/library/azure/dn132633.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67d4d-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="67d4d-192">**メモ**: nullable ではない場合、複数値プロパティのフィルター式には**any**演算子が必要です。詳細については、「[サポートされているクエリ、フィルター、およびページングのオプション](https://msdn.microsoft.com/library/azure/dn727074.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67d4d-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="67d4d-193">タグ</span><span class="sxs-lookup"><span data-stu-id="67d4d-193">tags</span></span>|<span data-ttu-id="67d4d-194">文字列</span><span class="sxs-lookup"><span data-stu-id="67d4d-194">String</span></span>|                                        <span data-ttu-id="67d4d-195">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="67d4d-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="67d4d-196">応答</span><span class="sxs-lookup"><span data-stu-id="67d4d-196">Response</span></span>

<span data-ttu-id="67d4d-197">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[serviceprincipal](../resources/serviceprincipal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67d4d-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67d4d-198">例</span><span class="sxs-lookup"><span data-stu-id="67d4d-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67d4d-199">要求</span><span class="sxs-lookup"><span data-stu-id="67d4d-199">Request</span></span>
<span data-ttu-id="67d4d-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67d4d-200">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="67d4d-201">プロトコル</span><span class="sxs-lookup"><span data-stu-id="67d4d-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="67d4d-202">C#</span><span class="sxs-lookup"><span data-stu-id="67d4d-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67d4d-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67d4d-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="67d4d-204">目的-C</span><span class="sxs-lookup"><span data-stu-id="67d4d-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67d4d-205">応答</span><span class="sxs-lookup"><span data-stu-id="67d4d-205">Response</span></span>
<span data-ttu-id="67d4d-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67d4d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
