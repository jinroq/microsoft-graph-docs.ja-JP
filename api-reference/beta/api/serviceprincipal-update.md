---
title: Serviceprincipal を更新します。
description: Serviceprincipal オブジェクトのプロパティを更新します。
ms.openlocfilehash: a24a8c949d48f577a3d7fe6208a1422819772801
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074002"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="4a5bd-103">Serviceprincipal を更新します。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-103">Update serviceprincipal</span></span>

> <span data-ttu-id="4a5bd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a5bd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a5bd-106">Serviceprincipal オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-106">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a5bd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a5bd-107">Permissions</span></span>
<span data-ttu-id="4a5bd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a5bd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a5bd-110">Permission type</span></span>      | <span data-ttu-id="4a5bd-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a5bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a5bd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a5bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a5bd-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a5bd-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a5bd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a5bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a5bd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-115">Not supported.</span></span>    |
|<span data-ttu-id="4a5bd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a5bd-116">Application</span></span> | <span data-ttu-id="4a5bd-117">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a5bd-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a5bd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a5bd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4a5bd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a5bd-119">Request headers</span></span>
| <span data-ttu-id="4a5bd-120">名前</span><span class="sxs-lookup"><span data-stu-id="4a5bd-120">Name</span></span>       | <span data-ttu-id="4a5bd-121">型</span><span class="sxs-lookup"><span data-stu-id="4a5bd-121">Type</span></span> | <span data-ttu-id="4a5bd-122">説明</span><span class="sxs-lookup"><span data-stu-id="4a5bd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4a5bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a5bd-123">Authorization</span></span>  | <span data-ttu-id="4a5bd-124">string</span><span class="sxs-lookup"><span data-stu-id="4a5bd-124">string</span></span>  | <span data-ttu-id="4a5bd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a5bd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a5bd-127">Request body</span></span>
<span data-ttu-id="4a5bd-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4a5bd-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a5bd-131">Property</span></span>     | <span data-ttu-id="4a5bd-132">型</span><span class="sxs-lookup"><span data-stu-id="4a5bd-132">Type</span></span>   |<span data-ttu-id="4a5bd-133">説明</span><span class="sxs-lookup"><span data-stu-id="4a5bd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a5bd-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="4a5bd-134">accountEnabled</span></span>|<span data-ttu-id="4a5bd-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a5bd-135">Boolean</span></span>|                <span data-ttu-id="4a5bd-136">**true**サービス プリンシパル アカウントは、有効な場合それ以外の場合、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-136">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="4a5bd-137">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a5bd-137">appDisplayName</span></span>|<span data-ttu-id="4a5bd-138">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-138">String</span></span>|<span data-ttu-id="4a5bd-139">関連付けられたアプリケーションによって公開される表示名です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-139">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="4a5bd-140">appId</span><span class="sxs-lookup"><span data-stu-id="4a5bd-140">appId</span></span>|<span data-ttu-id="4a5bd-141">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4a5bd-141">String</span></span>|<span data-ttu-id="4a5bd-142">関連付けられているアプリケーション (その**appId**プロパティの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-142">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="4a5bd-143">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="4a5bd-143">appRoleAssignmentRequired</span></span>|<span data-ttu-id="4a5bd-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a5bd-144">Boolean</span></span>|<span data-ttu-id="4a5bd-145">Azure AD アプリケーションに、ユーザーまたはアクセス トークンの発行は前にユーザーまたはグループに、 **appRoleAssignment**が必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-145">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="4a5bd-146">**メモ**: バージョン 1.5 が必要ですか、null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-146">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="4a5bd-147">appRoles</span><span class="sxs-lookup"><span data-stu-id="4a5bd-147">appRoles</span></span>|<span data-ttu-id="4a5bd-148">エンティティ</span><span class="sxs-lookup"><span data-stu-id="4a5bd-148">appRole</span></span>|<span data-ttu-id="4a5bd-149">アプリケーション ロールは、関連付けられたアプリケーションによって公開されています。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-149">The application roles exposed by the associated application.</span></span> <span data-ttu-id="4a5bd-150">詳細についてはアプリケーション エンティティ**のノート**で**appRoles**プロパティの定義を参照してください: バージョン 1.5 が必要ですか、null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-150">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="4a5bd-151">displayName</span><span class="sxs-lookup"><span data-stu-id="4a5bd-151">displayName</span></span>|<span data-ttu-id="4a5bd-152">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-152">String</span></span>|<span data-ttu-id="4a5bd-153">サービス ・ プリンシパルの表示名です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-153">The display name for the service principal.</span></span>|
|<span data-ttu-id="4a5bd-154">errorUrl</span><span class="sxs-lookup"><span data-stu-id="4a5bd-154">errorUrl</span></span>|<span data-ttu-id="4a5bd-155">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-155">String</span></span>|            |
|<span data-ttu-id="4a5bd-156">ホームページ</span><span class="sxs-lookup"><span data-stu-id="4a5bd-156">homepage</span></span>|<span data-ttu-id="4a5bd-157">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-157">String</span></span>|<span data-ttu-id="4a5bd-158">関連付けられたアプリケーションのホーム ページの URL です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-158">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="4a5bd-159">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="4a5bd-159">keyCredentials</span></span>|<span data-ttu-id="4a5bd-160">keyCredential</span><span class="sxs-lookup"><span data-stu-id="4a5bd-160">keyCredential</span></span>|<span data-ttu-id="4a5bd-161">サービス ・ プリンシパルに関連付けられているキーの資格情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-161">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="4a5bd-162">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-162">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4a5bd-163">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="4a5bd-163">logoutUrl</span></span>|<span data-ttu-id="4a5bd-164">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-164">String</span></span>| <span data-ttu-id="4a5bd-165">[前方チャンネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[背面チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウトのプロトコルを使用してユーザーをログアウトするマイクロソフトの承認のサービスによって使用される URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-165">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="4a5bd-166">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="4a5bd-166">oauth2Permissions</span></span>|<span data-ttu-id="4a5bd-167">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="4a5bd-167">oAuth2Permission</span></span>|<span data-ttu-id="4a5bd-168">関連付けられたアプリケーションによって公開される OAuth 2.0 のアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-168">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="4a5bd-169">詳細については、アプリケーション エンティティの**oauth2Permissions**プロパティの定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-169">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="4a5bd-170">**メモ**: バージョン 1.5 が必要ですか、null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-170">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="4a5bd-171">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="4a5bd-171">passwordCredentials</span></span>|<span data-ttu-id="4a5bd-172">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="4a5bd-172">passwordCredential</span></span>|<span data-ttu-id="4a5bd-173">サービス ・ プリンシパルに関連付けられているパスワード資格情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-173">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="4a5bd-174">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-174">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4a5bd-175">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="4a5bd-175">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="4a5bd-176">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-176">String</span></span>|<span data-ttu-id="4a5bd-177">内部使用専用として予約されています。  </span><span class="sxs-lookup"><span data-stu-id="4a5bd-177">Reserved for internal use only.</span></span> <span data-ttu-id="4a5bd-178">記述したり、それ以外の場合、このプロパティに依存しないでください。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-178">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="4a5bd-179">将来のバージョンで削除する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-179">May be removed in future versions.</span></span>                            <span data-ttu-id="4a5bd-180">**メモ**: バージョン 1.5 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-180">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="4a5bd-181">publisherName</span><span class="sxs-lookup"><span data-stu-id="4a5bd-181">publisherName</span></span>|<span data-ttu-id="4a5bd-182">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4a5bd-182">String</span></span>|<span data-ttu-id="4a5bd-183">関連付けられたアプリケーションが指定されているテナントの表示名です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-183">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="4a5bd-184">replyUrls</span><span class="sxs-lookup"><span data-stu-id="4a5bd-184">replyUrls</span></span>|<span data-ttu-id="4a5bd-185">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-185">String</span></span>|<span data-ttu-id="4a5bd-186">ユーザー トークン用に送信される、関連するアプリケーション、またはリダイレクトを使用して記号を OAuth 2.0 の Uri の認証コードをアクセス トークンは、関連付けられたアプリケーション用に送信される Url です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-186">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="4a5bd-187">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-187">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4a5bd-188">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="4a5bd-188">samlMetadataUrl</span></span>|<span data-ttu-id="4a5bd-189">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-189">String</span></span>|            |
|<span data-ttu-id="4a5bd-190">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="4a5bd-190">servicePrincipalNames</span></span>|<span data-ttu-id="4a5bd-191">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-191">String</span></span>|<span data-ttu-id="4a5bd-192">関連付けられたアプリケーションを識別する Uri。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-192">The URIs that identify the associated application.</span></span> <span data-ttu-id="4a5bd-193">詳細情報は、「[アプリケーションのオブジェクトおよびオブジェクトのサービス プリンシパル](https://msdn.microsoft.com/library/azure/dn132633.aspx)です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-193">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="4a5bd-194">**メモ**: null を許容しない、 **any**演算子は、複数値を持つプロパティのフィルター式に必要な詳細については、[サポートされているクエリ、フィルター、およびページングのオプション](https://msdn.microsoft.com/library/azure/dn727074.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-194">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="4a5bd-195">タグの前に追加されるマークアップ</span><span class="sxs-lookup"><span data-stu-id="4a5bd-195">tags</span></span>|<span data-ttu-id="4a5bd-196">String</span><span class="sxs-lookup"><span data-stu-id="4a5bd-196">String</span></span>|                                        <span data-ttu-id="4a5bd-197">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-197">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="4a5bd-198">応答</span><span class="sxs-lookup"><span data-stu-id="4a5bd-198">Response</span></span>

<span data-ttu-id="4a5bd-199">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[servicePrincipal](../resources/serviceprincipal.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-199">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a5bd-200">例</span><span class="sxs-lookup"><span data-stu-id="4a5bd-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a5bd-201">要求</span><span class="sxs-lookup"><span data-stu-id="4a5bd-201">Request</span></span>
<span data-ttu-id="4a5bd-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-202">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4a5bd-203">応答</span><span class="sxs-lookup"><span data-stu-id="4a5bd-203">Response</span></span>
<span data-ttu-id="4a5bd-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a5bd-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->