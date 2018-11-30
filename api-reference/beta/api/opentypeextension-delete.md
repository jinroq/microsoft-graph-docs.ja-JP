---
title: オープン拡張機能を削除する
description: '指定されたリソースのインスタンスからオープン拡張機能 (openTypeExtension オブジェクト) を削除します。 '
ms.openlocfilehash: 852573241e65e1a68ecbb308a67f79ee4ec14ab8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068359"
---
# <a name="delete-open-extension"></a><span data-ttu-id="4187a-103">オープン拡張機能を削除する</span><span class="sxs-lookup"><span data-stu-id="4187a-103">Delete open extension</span></span>

> <span data-ttu-id="4187a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4187a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4187a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4187a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4187a-106">指定されたリソースのインスタンスからオープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) オブジェクト) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4187a-106">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4187a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4187a-107">Permissions</span></span>

<span data-ttu-id="4187a-108">拡張子を削除するリソース、およびアクセス許可によって委任された (アプリケーション) の種類を要求、次の表で指定されたアクセス許可は、この API を呼び出すために必要最低限の特権。</span><span class="sxs-lookup"><span data-stu-id="4187a-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4187a-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4187a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4187a-110">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="4187a-110">Supported resource</span></span> | <span data-ttu-id="4187a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4187a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4187a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4187a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4187a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4187a-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="4187a-114">device</span><span class="sxs-lookup"><span data-stu-id="4187a-114">device</span></span>](../resources/device.md) | <span data-ttu-id="4187a-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4187a-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="4187a-116">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4187a-116">Not supported</span></span> | <span data-ttu-id="4187a-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="4187a-118">イベント</span><span class="sxs-lookup"><span data-stu-id="4187a-118">event</span></span>](../resources/event.md) | <span data-ttu-id="4187a-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="4187a-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="4187a-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="4187a-122">グループ</span><span class="sxs-lookup"><span data-stu-id="4187a-122">group</span></span>](../resources/group.md) | <span data-ttu-id="4187a-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="4187a-124">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4187a-124">Not supported</span></span> | <span data-ttu-id="4187a-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="4187a-126">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="4187a-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="4187a-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="4187a-128">使用不可</span><span class="sxs-lookup"><span data-stu-id="4187a-128">Not supported</span></span> | <span data-ttu-id="4187a-129">使用不可</span><span class="sxs-lookup"><span data-stu-id="4187a-129">Not supported</span></span> |
| [<span data-ttu-id="4187a-130">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="4187a-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="4187a-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="4187a-132">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4187a-132">Not supported</span></span> | <span data-ttu-id="4187a-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="4187a-134">メッセージ</span><span class="sxs-lookup"><span data-stu-id="4187a-134">message</span></span>](../resources/message.md) | <span data-ttu-id="4187a-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-135">Mail.ReadWrite</span></span> | <span data-ttu-id="4187a-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-136">Mail.ReadWrite</span></span> | <span data-ttu-id="4187a-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="4187a-138">組織</span><span class="sxs-lookup"><span data-stu-id="4187a-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="4187a-139">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4187a-139">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="4187a-140">使用不可</span><span class="sxs-lookup"><span data-stu-id="4187a-140">Not supported</span></span> | <span data-ttu-id="4187a-141">使用不可</span><span class="sxs-lookup"><span data-stu-id="4187a-141">Not supported</span></span> |
| [<span data-ttu-id="4187a-142">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="4187a-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="4187a-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="4187a-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="4187a-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="4187a-146">ユーザー</span><span class="sxs-lookup"><span data-stu-id="4187a-146">user</span></span>](../resources/user.md) | <span data-ttu-id="4187a-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-147">User.ReadWrite.All</span></span> | <span data-ttu-id="4187a-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4187a-148">User.ReadWrite</span></span> | <span data-ttu-id="4187a-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4187a-149">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4187a-150">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4187a-150">HTTP request</span></span>

<span data-ttu-id="4187a-151">要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `DELETE` を行います。</span><span class="sxs-lookup"><span data-stu-id="4187a-151">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{Id}/extensions/{extensionId}
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

><span data-ttu-id="4187a-p103">**注:** 上記の構文は、拡張機能の削除元となるリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を削除できます。</span><span class="sxs-lookup"><span data-stu-id="4187a-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="4187a-154">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="4187a-154">Path parameters</span></span>
|<span data-ttu-id="4187a-155">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="4187a-155">**Parameter**</span></span>|<span data-ttu-id="4187a-156">**型**</span><span class="sxs-lookup"><span data-stu-id="4187a-156">**Type**</span></span>|<span data-ttu-id="4187a-157">**説明**</span><span class="sxs-lookup"><span data-stu-id="4187a-157">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4187a-158">ID</span><span class="sxs-lookup"><span data-stu-id="4187a-158">id</span></span>|<span data-ttu-id="4187a-159">文字列</span><span class="sxs-lookup"><span data-stu-id="4187a-159">string</span></span>|<span data-ttu-id="4187a-p104">対応するコレクションのインスタンスの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="4187a-p104">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="4187a-162">extensionId</span><span class="sxs-lookup"><span data-stu-id="4187a-162">extensionId</span></span>|<span data-ttu-id="4187a-163">文字列</span><span class="sxs-lookup"><span data-stu-id="4187a-163">string</span></span>|<span data-ttu-id="4187a-p105">これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="4187a-p105">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4187a-167">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4187a-167">Request headers</span></span>
| <span data-ttu-id="4187a-168">名前</span><span class="sxs-lookup"><span data-stu-id="4187a-168">Name</span></span>       | <span data-ttu-id="4187a-169">値</span><span class="sxs-lookup"><span data-stu-id="4187a-169">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4187a-170">Authorization</span><span class="sxs-lookup"><span data-stu-id="4187a-170">Authorization</span></span> | <span data-ttu-id="4187a-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4187a-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4187a-173">要求本文</span><span class="sxs-lookup"><span data-stu-id="4187a-173">Request body</span></span>
<span data-ttu-id="4187a-174">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4187a-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4187a-175">応答</span><span class="sxs-lookup"><span data-stu-id="4187a-175">Response</span></span>

<span data-ttu-id="4187a-p107">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4187a-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4187a-178">例</span><span class="sxs-lookup"><span data-stu-id="4187a-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4187a-179">要求</span><span class="sxs-lookup"><span data-stu-id="4187a-179">Request</span></span>
<span data-ttu-id="4187a-180">最初の例では、名前で拡張情報を参照し、指定されたメッセージの拡張情報を削除します。</span><span class="sxs-lookup"><span data-stu-id="4187a-180">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="4187a-181">2 番目の例では、指定されたグループ イベントの拡張機能を削除します。</span><span class="sxs-lookup"><span data-stu-id="4187a-181">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="4187a-182">応答</span><span class="sxs-lookup"><span data-stu-id="4187a-182">Response</span></span>
<span data-ttu-id="4187a-183">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4187a-183">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->