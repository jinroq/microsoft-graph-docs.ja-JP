---
title: 連絡先を取得する
description: プロパティと関係の連絡先オブジェクトを取得します。
author: angelgolfer-ms
ms.openlocfilehash: fceda46729f539081458c1f26c5d385a984ed2d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322926"
---
# <a name="get-contact"></a><span data-ttu-id="4e38e-103">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="4e38e-103">Get contact</span></span>

> <span data-ttu-id="4e38e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e38e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e38e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e38e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e38e-106">プロパティと関係の連絡先オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="4e38e-106">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="4e38e-107">2 つシナリオは、アプリケーションが別のユーザーの連絡先フォルダーに連絡先を取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="4e38e-107">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="4e38e-108">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="4e38e-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="4e38e-109">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="4e38e-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="4e38e-110">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e38e-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="4e38e-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4e38e-111">Permissions</span></span>
<span data-ttu-id="4e38e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e38e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e38e-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e38e-114">Permission type</span></span>      | <span data-ttu-id="4e38e-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e38e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e38e-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e38e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4e38e-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e38e-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4e38e-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e38e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e38e-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e38e-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4e38e-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e38e-120">Application</span></span> | <span data-ttu-id="4e38e-121">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e38e-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e38e-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e38e-122">HTTP request</span></span>
<span data-ttu-id="4e38e-123"><!-- { "blockType": "ignored" } -->[連絡先](../resources/contact.md)ユーザーのメールボックスにします。</span><span class="sxs-lookup"><span data-stu-id="4e38e-123"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="4e38e-124">[連絡先](../resources/contact.md)ユーザーの最上位レベル[contactFolder](../resources/contactfolder.md)からです。</span><span class="sxs-lookup"><span data-stu-id="4e38e-124">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="4e38e-125">[にお問い合わせください](../resources/contact.md) [contactFolder](../resources/mailfolder.md)の子フォルダーに含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e38e-125">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="4e38e-126">次の例は、入れ子のレベルを 1 つを示していますが、連絡先を子の子でというように配置できます。</span><span class="sxs-lookup"><span data-stu-id="4e38e-126">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4e38e-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4e38e-127">Optional query parameters</span></span>
|<span data-ttu-id="4e38e-128">名前</span><span class="sxs-lookup"><span data-stu-id="4e38e-128">Name</span></span>|<span data-ttu-id="4e38e-129">値</span><span class="sxs-lookup"><span data-stu-id="4e38e-129">Value</span></span>|<span data-ttu-id="4e38e-130">説明</span><span class="sxs-lookup"><span data-stu-id="4e38e-130">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="4e38e-131">$expand</span><span class="sxs-lookup"><span data-stu-id="4e38e-131">$expand</span></span>|<span data-ttu-id="4e38e-132">文字列</span><span class="sxs-lookup"><span data-stu-id="4e38e-132">string</span></span>|<span data-ttu-id="4e38e-133">展開して応答に含める関係を示すコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="4e38e-133">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="4e38e-134">サポートされている名前の[contact](../resources/contact.md)オブジェクトのリレーションシップのテーブルを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e38e-134">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="4e38e-135">$select</span><span class="sxs-lookup"><span data-stu-id="4e38e-135">$select</span></span>|<span data-ttu-id="4e38e-136">文字列</span><span class="sxs-lookup"><span data-stu-id="4e38e-136">string</span></span>|<span data-ttu-id="4e38e-137">応答に含めるプロパティを示すコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="4e38e-137">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4e38e-138">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e38e-138">Request headers</span></span>
| <span data-ttu-id="4e38e-139">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e38e-139">Header</span></span>       | <span data-ttu-id="4e38e-140">値</span><span class="sxs-lookup"><span data-stu-id="4e38e-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e38e-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e38e-141">Authorization</span></span>  | <span data-ttu-id="4e38e-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4e38e-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e38e-144">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e38e-144">Request body</span></span>
<span data-ttu-id="4e38e-145">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4e38e-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e38e-146">応答</span><span class="sxs-lookup"><span data-stu-id="4e38e-146">Response</span></span>

<span data-ttu-id="4e38e-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4e38e-147">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e38e-148">例</span><span class="sxs-lookup"><span data-stu-id="4e38e-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e38e-149">要求</span><span class="sxs-lookup"><span data-stu-id="4e38e-149">Request</span></span>
<span data-ttu-id="4e38e-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e38e-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
##### <a name="response"></a><span data-ttu-id="4e38e-151">応答</span><span class="sxs-lookup"><span data-stu-id="4e38e-151">Response</span></span>
<span data-ttu-id="4e38e-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e38e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com",
      "type": "unknown"
    },
    {
      "name": "Garth",
      "address": "garth@contoso.onmicrosoft.com",
      "type": "personal"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "assistantName": null,
  "manager": null,
  "phones": [{
    "type": "business",
    "number": "+1 918 555 0101"
  }],
  "postalAddresses": [{
    "type": "business",
    "postOfficeBox": "P.O. Box 100",
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "countryOrRegion": "USA",
    "postalCode": "98121"
  }],
  "spouseName": null,
  "personalNotes": null,
  "children": [], 
  "gender": null,
  "websites": [{
      "type": "work",
      "address": "https://www.contoso.com",
      "name": "Contoso"
  }],
  "weddingAnniversary": null
}
```

## <a name="see-also"></a><span data-ttu-id="4e38e-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e38e-155">See also</span></span>

- [<span data-ttu-id="4e38e-156">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="4e38e-156">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4e38e-157">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="4e38e-157">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->