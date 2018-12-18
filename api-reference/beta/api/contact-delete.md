---
title: 連絡先を削除する
description: 連絡先を削除します。
author: angelgolfer-ms
ms.openlocfilehash: a8f1ea8c1ee0f202e60d4efb05f65022a9269c01
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319272"
---
# <a name="delete-contact"></a><span data-ttu-id="425e3-103">連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="425e3-103">Delete contact</span></span>

> <span data-ttu-id="425e3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="425e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="425e3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="425e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="425e3-106">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="425e3-106">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="425e3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="425e3-107">Permissions</span></span>
<span data-ttu-id="425e3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="425e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="425e3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="425e3-110">Permission type</span></span>      | <span data-ttu-id="425e3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="425e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="425e3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="425e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="425e3-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="425e3-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="425e3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="425e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="425e3-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="425e3-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="425e3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="425e3-116">Application</span></span> | <span data-ttu-id="425e3-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="425e3-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="425e3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="425e3-118">HTTP request</span></span>
<span data-ttu-id="425e3-119"><!-- { "blockType": "ignored" } -->[連絡先](../resources/contact.md)ユーザーの既定の[contactFolder](../resources/contactfolder.md)からです。</span><span class="sxs-lookup"><span data-stu-id="425e3-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="425e3-120">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="425e3-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="425e3-121">[にお問い合わせください](../resources/contact.md) [contactFolder](../resources/mailfolder.md)の子フォルダーに含まれています。</span><span class="sxs-lookup"><span data-stu-id="425e3-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="425e3-122">次の例は、入れ子のレベルを 1 つを示していますが、連絡先を子の子でというように配置できます。</span><span class="sxs-lookup"><span data-stu-id="425e3-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="425e3-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="425e3-123">Request headers</span></span>
| <span data-ttu-id="425e3-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="425e3-124">Header</span></span>       | <span data-ttu-id="425e3-125">値</span><span class="sxs-lookup"><span data-stu-id="425e3-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="425e3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="425e3-126">Authorization</span></span>  | <span data-ttu-id="425e3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="425e3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="425e3-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="425e3-129">Request body</span></span>
<span data-ttu-id="425e3-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="425e3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="425e3-131">応答</span><span class="sxs-lookup"><span data-stu-id="425e3-131">Response</span></span>

<span data-ttu-id="425e3-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="425e3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="425e3-134">例</span><span class="sxs-lookup"><span data-stu-id="425e3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="425e3-135">要求</span><span class="sxs-lookup"><span data-stu-id="425e3-135">Request</span></span>
<span data-ttu-id="425e3-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="425e3-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="425e3-137">応答</span><span class="sxs-lookup"><span data-stu-id="425e3-137">Response</span></span>
<span data-ttu-id="425e3-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="425e3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->