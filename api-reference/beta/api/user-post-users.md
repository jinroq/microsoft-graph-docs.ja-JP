---
title: user の作成
description: 新しいユーザーを作成するのにには、この API を使用します。
author: dkershaw10
ms.openlocfilehash: ace74039d3740b51487252447ba3d56a018f745e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314855"
---
# <a name="create-user"></a><span data-ttu-id="032a8-103">user の作成</span><span class="sxs-lookup"><span data-stu-id="032a8-103">Create user</span></span>

> <span data-ttu-id="032a8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="032a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="032a8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="032a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="032a8-106">新しいユーザーを作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="032a8-106">Use this API to create a new user.</span></span>
<span data-ttu-id="032a8-107">要求の本体には、作成するユーザーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="032a8-107">The request body contains the user to create.</span></span> <span data-ttu-id="032a8-108">最低限、ユーザーの必要なプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="032a8-108">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="032a8-109">その他の書き込み可能なプロパティを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="032a8-109">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="032a8-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="032a8-110">Permissions</span></span>
<span data-ttu-id="032a8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="032a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="032a8-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="032a8-113">Permission type</span></span>      | <span data-ttu-id="032a8-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="032a8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="032a8-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="032a8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="032a8-116">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="032a8-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="032a8-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="032a8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="032a8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="032a8-118">Not supported.</span></span>    |
|<span data-ttu-id="032a8-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="032a8-119">Application</span></span> | <span data-ttu-id="032a8-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="032a8-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="032a8-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="032a8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="032a8-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="032a8-122">Request headers</span></span>
| <span data-ttu-id="032a8-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="032a8-123">Header</span></span>       | <span data-ttu-id="032a8-124">値</span><span class="sxs-lookup"><span data-stu-id="032a8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="032a8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="032a8-125">Authorization</span></span>  | <span data-ttu-id="032a8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="032a8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="032a8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="032a8-128">Content-Type</span></span>  | <span data-ttu-id="032a8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="032a8-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="032a8-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="032a8-130">Request body</span></span>
<span data-ttu-id="032a8-131">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="032a8-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="032a8-132">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="032a8-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="032a8-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="032a8-133">Parameter</span></span> | <span data-ttu-id="032a8-134">種類</span><span class="sxs-lookup"><span data-stu-id="032a8-134">Type</span></span> | <span data-ttu-id="032a8-135">説明</span><span class="sxs-lookup"><span data-stu-id="032a8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="032a8-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="032a8-136">accountEnabled</span></span> |<span data-ttu-id="032a8-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="032a8-137">boolean</span></span> |<span data-ttu-id="032a8-138">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="032a8-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="032a8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="032a8-139">displayName</span></span> |<span data-ttu-id="032a8-140">string</span><span class="sxs-lookup"><span data-stu-id="032a8-140">string</span></span> |<span data-ttu-id="032a8-141">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="032a8-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="032a8-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="032a8-142">onPremisesImmutableId</span></span> |<span data-ttu-id="032a8-143">string</span><span class="sxs-lookup"><span data-stu-id="032a8-143">string</span></span> |<span data-ttu-id="032a8-144">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="032a8-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="032a8-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="032a8-145">mailNickname</span></span> |<span data-ttu-id="032a8-146">string</span><span class="sxs-lookup"><span data-stu-id="032a8-146">string</span></span> |<span data-ttu-id="032a8-147">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="032a8-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="032a8-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="032a8-148">passwordProfile</span></span>|[<span data-ttu-id="032a8-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="032a8-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="032a8-150">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="032a8-150">The password profile for the user.</span></span>|
|<span data-ttu-id="032a8-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="032a8-151">userPrincipalName</span></span> |<span data-ttu-id="032a8-152">string</span><span class="sxs-lookup"><span data-stu-id="032a8-152">string</span></span> |<span data-ttu-id="032a8-153">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="032a8-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="032a8-154">**ユーザー**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用すること、`POST`操作し、作成時にユーザー インスタンスに独自のデータにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="032a8-154">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="032a8-155">応答</span><span class="sxs-lookup"><span data-stu-id="032a8-155">Response</span></span>

<span data-ttu-id="032a8-156">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="032a8-156">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="032a8-157">例</span><span class="sxs-lookup"><span data-stu-id="032a8-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="032a8-158">要求</span><span class="sxs-lookup"><span data-stu-id="032a8-158">Request</span></span>
<span data-ttu-id="032a8-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="032a8-159">Here is an example of the request.</span></span>
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value@onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="032a8-160">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="032a8-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="032a8-161">応答</span><span class="sxs-lookup"><span data-stu-id="032a8-161">Response</span></span>
<span data-ttu-id="032a8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="032a8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

## <a name="see-also"></a><span data-ttu-id="032a8-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="032a8-165">See also</span></span>

- [<span data-ttu-id="032a8-166">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="032a8-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="032a8-167">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="032a8-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="032a8-168">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="032a8-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
