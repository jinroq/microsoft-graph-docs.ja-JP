---
title: Serviceprincipal を更新します。
description: Serviceprincipal オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511661"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="cd37c-103">Serviceprincipal を更新します。</span><span class="sxs-lookup"><span data-stu-id="cd37c-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd37c-104">Serviceprincipal オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cd37c-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd37c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cd37c-105">Permissions</span></span>
<span data-ttu-id="cd37c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd37c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd37c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd37c-108">Permission type</span></span>      | <span data-ttu-id="cd37c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd37c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd37c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd37c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd37c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd37c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd37c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd37c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd37c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-113">Not supported.</span></span>    |
|<span data-ttu-id="cd37c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd37c-114">Application</span></span> | <span data-ttu-id="cd37c-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd37c-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd37c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd37c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cd37c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd37c-117">Request headers</span></span>
| <span data-ttu-id="cd37c-118">名前</span><span class="sxs-lookup"><span data-stu-id="cd37c-118">Name</span></span>       | <span data-ttu-id="cd37c-119">型</span><span class="sxs-lookup"><span data-stu-id="cd37c-119">Type</span></span> | <span data-ttu-id="cd37c-120">説明</span><span class="sxs-lookup"><span data-stu-id="cd37c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd37c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd37c-121">Authorization</span></span>  | <span data-ttu-id="cd37c-122">string</span><span class="sxs-lookup"><span data-stu-id="cd37c-122">string</span></span>  | <span data-ttu-id="cd37c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cd37c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd37c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd37c-125">Request body</span></span>
<span data-ttu-id="cd37c-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="cd37c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cd37c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd37c-129">Property</span></span>     | <span data-ttu-id="cd37c-130">型</span><span class="sxs-lookup"><span data-stu-id="cd37c-130">Type</span></span>   |<span data-ttu-id="cd37c-131">説明</span><span class="sxs-lookup"><span data-stu-id="cd37c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd37c-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="cd37c-132">accountEnabled</span></span>|<span data-ttu-id="cd37c-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="cd37c-133">Boolean</span></span>|                <span data-ttu-id="cd37c-134">**true**サービス プリンシパル アカウントは、有効な場合それ以外の場合、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="cd37c-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="cd37c-135">AppDisplayName</span><span class="sxs-lookup"><span data-stu-id="cd37c-135">appDisplayName</span></span>|<span data-ttu-id="cd37c-136">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-136">String</span></span>|<span data-ttu-id="cd37c-137">関連付けられたアプリケーションによって公開される表示名です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="cd37c-138">appId</span><span class="sxs-lookup"><span data-stu-id="cd37c-138">appId</span></span>|<span data-ttu-id="cd37c-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="cd37c-139">String</span></span>|<span data-ttu-id="cd37c-140">関連付けられているアプリケーション (その**appId**プロパティの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="cd37c-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="cd37c-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="cd37c-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="cd37c-142">Boolean</span></span>|<span data-ttu-id="cd37c-143">Azure AD アプリケーションに、ユーザーまたはアクセス トークンの発行は前にユーザーまたはグループに、 **appRoleAssignment**が必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cd37c-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="cd37c-144">**メモ**: バージョン 1.5 が必要ですか、null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="cd37c-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="cd37c-145">appRoles</span></span>|<span data-ttu-id="cd37c-146">エンティティ</span><span class="sxs-lookup"><span data-stu-id="cd37c-146">appRole</span></span>|<span data-ttu-id="cd37c-147">アプリケーション ロールは、関連付けられたアプリケーションによって公開されています。</span><span class="sxs-lookup"><span data-stu-id="cd37c-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="cd37c-148">詳細についてはアプリケーション エンティティ**のノート**で**appRoles**プロパティの定義を参照してください: バージョン 1.5 が必要ですか、null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="cd37c-149">displayName</span><span class="sxs-lookup"><span data-stu-id="cd37c-149">displayName</span></span>|<span data-ttu-id="cd37c-150">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-150">String</span></span>|<span data-ttu-id="cd37c-151">サービス ・ プリンシパルの表示名です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="cd37c-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="cd37c-152">errorUrl</span></span>|<span data-ttu-id="cd37c-153">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-153">String</span></span>|            |
|<span data-ttu-id="cd37c-154">HomePage</span><span class="sxs-lookup"><span data-stu-id="cd37c-154">homepage</span></span>|<span data-ttu-id="cd37c-155">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-155">String</span></span>|<span data-ttu-id="cd37c-156">関連付けられたアプリケーションのホーム ページの URL です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="cd37c-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="cd37c-157">keyCredentials</span></span>|<span data-ttu-id="cd37c-158">keyCredential</span><span class="sxs-lookup"><span data-stu-id="cd37c-158">keyCredential</span></span>|<span data-ttu-id="cd37c-159">サービス ・ プリンシパルに関連付けられているキーの資格情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cd37c-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="cd37c-160">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="cd37c-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="cd37c-161">logoutUrl</span></span>|<span data-ttu-id="cd37c-162">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-162">String</span></span>| <span data-ttu-id="cd37c-163">[前方チャンネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[背面チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウトのプロトコルを使用してユーザーをログアウトするマイクロソフトの承認のサービスによって使用される URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="cd37c-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="cd37c-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="cd37c-164">oauth2Permissions</span></span>|<span data-ttu-id="cd37c-165">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="cd37c-165">oAuth2Permission</span></span>|<span data-ttu-id="cd37c-166">関連付けられたアプリケーションによって公開される OAuth 2.0 のアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="cd37c-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="cd37c-167">詳細については、アプリケーション エンティティの**oauth2Permissions**プロパティの定義を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd37c-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="cd37c-168">**メモ**: バージョン 1.5 が必要ですか、null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="cd37c-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="cd37c-169">passwordCredentials</span></span>|<span data-ttu-id="cd37c-170">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="cd37c-170">passwordCredential</span></span>|<span data-ttu-id="cd37c-171">サービス ・ プリンシパルに関連付けられているパスワード資格情報のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cd37c-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="cd37c-172">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="cd37c-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="cd37c-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="cd37c-174">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-174">String</span></span>|<span data-ttu-id="cd37c-175">内部使用専用として予約されています。  </span><span class="sxs-lookup"><span data-stu-id="cd37c-175">Reserved for internal use only.</span></span> <span data-ttu-id="cd37c-176">記述したり、それ以外の場合、このプロパティに依存しないでください。</span><span class="sxs-lookup"><span data-stu-id="cd37c-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="cd37c-177">将来のバージョンで削除する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cd37c-177">May be removed in future versions.</span></span>                            <span data-ttu-id="cd37c-178">**メモ**: バージョン 1.5 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="cd37c-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="cd37c-179">publisherName</span></span>|<span data-ttu-id="cd37c-180">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-180">String</span></span>|<span data-ttu-id="cd37c-181">関連付けられたアプリケーションが指定されているテナントの表示名です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="cd37c-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="cd37c-182">replyUrls</span></span>|<span data-ttu-id="cd37c-183">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-183">String</span></span>|<span data-ttu-id="cd37c-184">ユーザー トークン用に送信される、関連するアプリケーション、またはリダイレクトを使用して記号を OAuth 2.0 の Uri の認証コードをアクセス トークンは、関連付けられたアプリケーション用に送信される Url です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="cd37c-185">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="cd37c-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="cd37c-186">samlMetadataUrl</span></span>|<span data-ttu-id="cd37c-187">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-187">String</span></span>|            |
|<span data-ttu-id="cd37c-188">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="cd37c-188">servicePrincipalNames</span></span>|<span data-ttu-id="cd37c-189">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-189">String</span></span>|<span data-ttu-id="cd37c-190">関連付けられたアプリケーションを識別する Uri。</span><span class="sxs-lookup"><span data-stu-id="cd37c-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="cd37c-191">詳細情報は、「[アプリケーションのオブジェクトおよびオブジェクトのサービス プリンシパル](https://msdn.microsoft.com/library/azure/dn132633.aspx)です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="cd37c-192">**メモ**: null を許容しない、 **any**演算子は、複数値を持つプロパティのフィルター式に必要な詳細については、[サポートされているクエリ、フィルター、およびページングのオプション](https://msdn.microsoft.com/library/azure/dn727074.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd37c-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="cd37c-193">タグの前に追加されるマークアップ</span><span class="sxs-lookup"><span data-stu-id="cd37c-193">tags</span></span>|<span data-ttu-id="cd37c-194">String</span><span class="sxs-lookup"><span data-stu-id="cd37c-194">String</span></span>|                                        <span data-ttu-id="cd37c-195">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="cd37c-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="cd37c-196">応答</span><span class="sxs-lookup"><span data-stu-id="cd37c-196">Response</span></span>

<span data-ttu-id="cd37c-197">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[servicePrincipal](../resources/serviceprincipal.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cd37c-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd37c-198">例</span><span class="sxs-lookup"><span data-stu-id="cd37c-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd37c-199">要求</span><span class="sxs-lookup"><span data-stu-id="cd37c-199">Request</span></span>
<span data-ttu-id="cd37c-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd37c-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="cd37c-201">応答</span><span class="sxs-lookup"><span data-stu-id="cd37c-201">Response</span></span>
<span data-ttu-id="cd37c-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cd37c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
