---
title: オープン拡張機能を削除する
description: '指定されたリソースのインスタンスからオープン拡張機能 (openTypeExtension オブジェクト) を削除します。 '
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: a12ec2f482497b9d7e92067b001a58d05d378ddb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976432"
---
# <a name="delete-open-extension"></a><span data-ttu-id="092b7-103">オープン拡張機能を削除する</span><span class="sxs-lookup"><span data-stu-id="092b7-103">Delete open extension</span></span>

<span data-ttu-id="092b7-104">指定されたリソースのインスタンスからオープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) オブジェクト) を削除します。</span><span class="sxs-lookup"><span data-stu-id="092b7-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="092b7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="092b7-105">Permissions</span></span>

<span data-ttu-id="092b7-106">拡張機能を削除するリソースと、要求されたアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可は、この API を呼び出すために必要な最低限の特権です。</span><span class="sxs-lookup"><span data-stu-id="092b7-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="092b7-107">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="092b7-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="092b7-108">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="092b7-108">Supported resource</span></span> | <span data-ttu-id="092b7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="092b7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="092b7-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="092b7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="092b7-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="092b7-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="092b7-112">device</span><span class="sxs-lookup"><span data-stu-id="092b7-112">device</span></span>](../resources/device.md) | <span data-ttu-id="092b7-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="092b7-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="092b7-114">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="092b7-114">Not supported</span></span> | <span data-ttu-id="092b7-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="092b7-116">イベント</span><span class="sxs-lookup"><span data-stu-id="092b7-116">event</span></span>](../resources/event.md) | <span data-ttu-id="092b7-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="092b7-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="092b7-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="092b7-120">グループ</span><span class="sxs-lookup"><span data-stu-id="092b7-120">group</span></span>](../resources/group.md) | <span data-ttu-id="092b7-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="092b7-122">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="092b7-122">Not supported</span></span> | <span data-ttu-id="092b7-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-123">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="092b7-124">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="092b7-124">group event</span></span>](../resources/event.md) | <span data-ttu-id="092b7-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="092b7-126">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="092b7-126">Not supported</span></span> | <span data-ttu-id="092b7-127">非サポート</span><span class="sxs-lookup"><span data-stu-id="092b7-127">Not supported</span></span> |
| [<span data-ttu-id="092b7-128">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="092b7-128">group post</span></span>](../resources/post.md) | <span data-ttu-id="092b7-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="092b7-130">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="092b7-130">Not supported</span></span> | <span data-ttu-id="092b7-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="092b7-132">メッセージ</span><span class="sxs-lookup"><span data-stu-id="092b7-132">message</span></span>](../resources/message.md) | <span data-ttu-id="092b7-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-133">Mail.ReadWrite</span></span> | <span data-ttu-id="092b7-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-134">Mail.ReadWrite</span></span> | <span data-ttu-id="092b7-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="092b7-136">組織</span><span class="sxs-lookup"><span data-stu-id="092b7-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="092b7-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="092b7-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="092b7-138">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="092b7-138">Not supported</span></span> | <span data-ttu-id="092b7-139">非サポート</span><span class="sxs-lookup"><span data-stu-id="092b7-139">Not supported</span></span> |
| [<span data-ttu-id="092b7-140">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="092b7-140">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="092b7-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="092b7-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="092b7-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="092b7-144">user</span><span class="sxs-lookup"><span data-stu-id="092b7-144">user</span></span>](../resources/user.md) | <span data-ttu-id="092b7-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-145">User.ReadWrite.All</span></span> | <span data-ttu-id="092b7-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="092b7-146">User.ReadWrite</span></span> | <span data-ttu-id="092b7-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092b7-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="092b7-148">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="092b7-148">HTTP request</span></span>
<span data-ttu-id="092b7-149">要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `DELETE` を行います。</span><span class="sxs-lookup"><span data-stu-id="092b7-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="092b7-p102">**注:** 上記の構文は、拡張機能の削除元となるリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を削除できます。</span><span class="sxs-lookup"><span data-stu-id="092b7-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="092b7-152">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="092b7-152">Path parameters</span></span>
|<span data-ttu-id="092b7-153">パラメーター</span><span class="sxs-lookup"><span data-stu-id="092b7-153">Parameter</span></span>|<span data-ttu-id="092b7-154">型</span><span class="sxs-lookup"><span data-stu-id="092b7-154">Type</span></span>|<span data-ttu-id="092b7-155">説明</span><span class="sxs-lookup"><span data-stu-id="092b7-155">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="092b7-156">id</span><span class="sxs-lookup"><span data-stu-id="092b7-156">id</span></span>|<span data-ttu-id="092b7-157">string</span><span class="sxs-lookup"><span data-stu-id="092b7-157">string</span></span>|<span data-ttu-id="092b7-p103">対応するコレクションのインスタンスの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="092b7-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="092b7-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="092b7-160">extensionId</span></span>|<span data-ttu-id="092b7-161">string</span><span class="sxs-lookup"><span data-stu-id="092b7-161">string</span></span>|<span data-ttu-id="092b7-p104">これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="092b7-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="092b7-165">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="092b7-165">Request headers</span></span>
| <span data-ttu-id="092b7-166">名前</span><span class="sxs-lookup"><span data-stu-id="092b7-166">Name</span></span>       | <span data-ttu-id="092b7-167">値</span><span class="sxs-lookup"><span data-stu-id="092b7-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="092b7-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="092b7-168">Authorization</span></span> | <span data-ttu-id="092b7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="092b7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="092b7-171">要求本文</span><span class="sxs-lookup"><span data-stu-id="092b7-171">Request body</span></span>
<span data-ttu-id="092b7-172">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="092b7-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="092b7-173">応答</span><span class="sxs-lookup"><span data-stu-id="092b7-173">Response</span></span>

<span data-ttu-id="092b7-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="092b7-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="092b7-176">例</span><span class="sxs-lookup"><span data-stu-id="092b7-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="092b7-177">要求</span><span class="sxs-lookup"><span data-stu-id="092b7-177">Request</span></span>
<span data-ttu-id="092b7-178">最初の例では、名前で拡張情報を参照し、指定されたメッセージの拡張情報を削除します。</span><span class="sxs-lookup"><span data-stu-id="092b7-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="092b7-179">プロトコル</span><span class="sxs-lookup"><span data-stu-id="092b7-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="092b7-180">C#</span><span class="sxs-lookup"><span data-stu-id="092b7-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="092b7-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="092b7-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="092b7-182">目的-C</span><span class="sxs-lookup"><span data-stu-id="092b7-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="092b7-183">Java</span><span class="sxs-lookup"><span data-stu-id="092b7-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="092b7-184">2 番目の例では、指定されたグループ イベントの拡張機能を削除します。</span><span class="sxs-lookup"><span data-stu-id="092b7-184">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="092b7-185">応答</span><span class="sxs-lookup"><span data-stu-id="092b7-185">Response</span></span>
<span data-ttu-id="092b7-186">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="092b7-186">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
