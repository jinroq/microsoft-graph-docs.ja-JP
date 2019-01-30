---
title: user の作成
description: 新しいユーザーを作成するのにには、この API を使用します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9d1e98ffa4be67141d1e5ae679f9f51a71ef92fd
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642528"
---
# <a name="create-user"></a><span data-ttu-id="5b7fc-103">user の作成</span><span class="sxs-lookup"><span data-stu-id="5b7fc-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b7fc-104">新しいユーザーを作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-104">Use this API to create a new user.</span></span>
<span data-ttu-id="5b7fc-105">要求の本体には、作成するユーザーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-105">The request body contains the user to create.</span></span> <span data-ttu-id="5b7fc-106">最低限、ユーザーの必要なプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="5b7fc-107">その他の書き込み可能なプロパティを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-107">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b7fc-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b7fc-108">Permissions</span></span>
<span data-ttu-id="5b7fc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b7fc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b7fc-111">Permission type</span></span>      | <span data-ttu-id="5b7fc-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b7fc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b7fc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b7fc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b7fc-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b7fc-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b7fc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b7fc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b7fc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-116">Not supported.</span></span>    |
|<span data-ttu-id="5b7fc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b7fc-117">Application</span></span> | <span data-ttu-id="5b7fc-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b7fc-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b7fc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b7fc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="5b7fc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b7fc-120">Request headers</span></span>
| <span data-ttu-id="5b7fc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b7fc-121">Header</span></span>       | <span data-ttu-id="5b7fc-122">値</span><span class="sxs-lookup"><span data-stu-id="5b7fc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b7fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b7fc-123">Authorization</span></span>  | <span data-ttu-id="5b7fc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b7fc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b7fc-126">Content-Type</span></span>  | <span data-ttu-id="5b7fc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5b7fc-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b7fc-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b7fc-128">Request body</span></span>
<span data-ttu-id="5b7fc-129">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="5b7fc-130">次の表に、ユーザーの作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="5b7fc-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5b7fc-131">Parameter</span></span> | <span data-ttu-id="5b7fc-132">型</span><span class="sxs-lookup"><span data-stu-id="5b7fc-132">Type</span></span> | <span data-ttu-id="5b7fc-133">説明</span><span class="sxs-lookup"><span data-stu-id="5b7fc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b7fc-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="5b7fc-134">accountEnabled</span></span> |<span data-ttu-id="5b7fc-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="5b7fc-135">boolean</span></span> |<span data-ttu-id="5b7fc-136">アカウントが有効な場合は true。それ以外の場合は false。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="5b7fc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5b7fc-137">displayName</span></span> |<span data-ttu-id="5b7fc-138">string</span><span class="sxs-lookup"><span data-stu-id="5b7fc-138">string</span></span> |<span data-ttu-id="5b7fc-139">ユーザーのアドレス帳に表示される名前。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="5b7fc-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="5b7fc-140">onPremisesImmutableId</span></span> |<span data-ttu-id="5b7fc-141">string</span><span class="sxs-lookup"><span data-stu-id="5b7fc-141">string</span></span> |<span data-ttu-id="5b7fc-142">ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="5b7fc-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="5b7fc-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5b7fc-143">mailNickname</span></span> |<span data-ttu-id="5b7fc-144">string</span><span class="sxs-lookup"><span data-stu-id="5b7fc-144">string</span></span> |<span data-ttu-id="5b7fc-145">ユーザーのメール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="5b7fc-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="5b7fc-146">passwordProfile</span></span>|[<span data-ttu-id="5b7fc-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="5b7fc-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="5b7fc-148">ユーザーのパスワード プロファイル。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-148">The password profile for the user.</span></span>|
|<span data-ttu-id="5b7fc-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5b7fc-149">userPrincipalName</span></span> |<span data-ttu-id="5b7fc-150">string</span><span class="sxs-lookup"><span data-stu-id="5b7fc-150">string</span></span> |<span data-ttu-id="5b7fc-151">ユーザー プリンシパル名 (someuser@contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="5b7fc-152">**ユーザー**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用すること、`POST`操作し、作成時にユーザー インスタンスに独自のデータにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-152">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="5b7fc-153">応答</span><span class="sxs-lookup"><span data-stu-id="5b7fc-153">Response</span></span>

<span data-ttu-id="5b7fc-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-154">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b7fc-155">例</span><span class="sxs-lookup"><span data-stu-id="5b7fc-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b7fc-156">要求</span><span class="sxs-lookup"><span data-stu-id="5b7fc-156">Request</span></span>
<span data-ttu-id="5b7fc-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-157">Here is an example of the request.</span></span>
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
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="5b7fc-158">要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-158">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5b7fc-159">応答</span><span class="sxs-lookup"><span data-stu-id="5b7fc-159">Response</span></span>
<span data-ttu-id="5b7fc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b7fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5b7fc-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="5b7fc-163">See also</span></span>

- [<span data-ttu-id="5b7fc-164">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="5b7fc-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5b7fc-165">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="5b7fc-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5b7fc-166">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="5b7fc-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
