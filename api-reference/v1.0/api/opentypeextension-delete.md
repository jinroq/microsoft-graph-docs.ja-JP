---
title: オープン拡張機能を削除する
description: '指定されたリソースのインスタンスからオープン拡張機能 (openTypeExtension オブジェクト) を削除します。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: de0e609ba0d10d8d0b96e64f650347fb4f6fded8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562098"
---
# <a name="delete-open-extension"></a><span data-ttu-id="6e655-103">オープン拡張機能を削除する</span><span class="sxs-lookup"><span data-stu-id="6e655-103">Delete open extension</span></span>

<span data-ttu-id="6e655-104">指定されたリソースのインスタンスからオープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) オブジェクト) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6e655-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6e655-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e655-105">Permissions</span></span>

<span data-ttu-id="6e655-106">拡張機能を削除するリソースと、要求されたアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可は、この API を呼び出すために必要な最低限の特権です。</span><span class="sxs-lookup"><span data-stu-id="6e655-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6e655-107">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e655-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e655-108">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="6e655-108">Supported resource</span></span> | <span data-ttu-id="6e655-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e655-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6e655-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e655-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e655-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e655-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="6e655-112">device</span><span class="sxs-lookup"><span data-stu-id="6e655-112">device</span></span>](../resources/device.md) | <span data-ttu-id="6e655-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e655-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="6e655-114">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6e655-114">Not supported</span></span> | <span data-ttu-id="6e655-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="6e655-116">event</span><span class="sxs-lookup"><span data-stu-id="6e655-116">event</span></span>](../resources/event.md) | <span data-ttu-id="6e655-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="6e655-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="6e655-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="6e655-120">グループ</span><span class="sxs-lookup"><span data-stu-id="6e655-120">group</span></span>](../resources/group.md) | <span data-ttu-id="6e655-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="6e655-122">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6e655-122">Not supported</span></span> | <span data-ttu-id="6e655-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-123">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="6e655-124">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="6e655-124">group event</span></span>](../resources/event.md) | <span data-ttu-id="6e655-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="6e655-126">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6e655-126">Not supported</span></span> | <span data-ttu-id="6e655-127">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6e655-127">Not supported</span></span> |
| [<span data-ttu-id="6e655-128">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="6e655-128">group post</span></span>](../resources/post.md) | <span data-ttu-id="6e655-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="6e655-130">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6e655-130">Not supported</span></span> | <span data-ttu-id="6e655-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="6e655-132">メッセージ</span><span class="sxs-lookup"><span data-stu-id="6e655-132">message</span></span>](../resources/message.md) | <span data-ttu-id="6e655-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-133">Mail.ReadWrite</span></span> | <span data-ttu-id="6e655-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-134">Mail.ReadWrite</span></span> | <span data-ttu-id="6e655-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="6e655-136">組織</span><span class="sxs-lookup"><span data-stu-id="6e655-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="6e655-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e655-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="6e655-138">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="6e655-138">Not supported</span></span> | <span data-ttu-id="6e655-139">非サポート</span><span class="sxs-lookup"><span data-stu-id="6e655-139">Not supported</span></span> |
| [<span data-ttu-id="6e655-140">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="6e655-140">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="6e655-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="6e655-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="6e655-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="6e655-144">ユーザー</span><span class="sxs-lookup"><span data-stu-id="6e655-144">user</span></span>](../resources/user.md) | <span data-ttu-id="6e655-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-145">User.ReadWrite.All</span></span> | <span data-ttu-id="6e655-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e655-146">User.ReadWrite</span></span> | <span data-ttu-id="6e655-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e655-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e655-148">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e655-148">HTTP request</span></span>
<span data-ttu-id="6e655-149">要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `DELETE` を行います。</span><span class="sxs-lookup"><span data-stu-id="6e655-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="6e655-p102">**注:** 上記の構文は、拡張機能の削除元となるリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を削除できます。</span><span class="sxs-lookup"><span data-stu-id="6e655-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="6e655-152">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e655-152">Path parameters</span></span>
|<span data-ttu-id="6e655-153">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e655-153">Parameter</span></span>|<span data-ttu-id="6e655-154">型</span><span class="sxs-lookup"><span data-stu-id="6e655-154">Type</span></span>|<span data-ttu-id="6e655-155">説明</span><span class="sxs-lookup"><span data-stu-id="6e655-155">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6e655-156">id</span><span class="sxs-lookup"><span data-stu-id="6e655-156">id</span></span>|<span data-ttu-id="6e655-157">string</span><span class="sxs-lookup"><span data-stu-id="6e655-157">string</span></span>|<span data-ttu-id="6e655-p103">対応するコレクションのインスタンスの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="6e655-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="6e655-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="6e655-160">extensionId</span></span>|<span data-ttu-id="6e655-161">string</span><span class="sxs-lookup"><span data-stu-id="6e655-161">string</span></span>|<span data-ttu-id="6e655-p104">これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="6e655-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6e655-165">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e655-165">Request headers</span></span>
| <span data-ttu-id="6e655-166">名前</span><span class="sxs-lookup"><span data-stu-id="6e655-166">Name</span></span>       | <span data-ttu-id="6e655-167">値</span><span class="sxs-lookup"><span data-stu-id="6e655-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6e655-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e655-168">Authorization</span></span> | <span data-ttu-id="6e655-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e655-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e655-171">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e655-171">Request body</span></span>
<span data-ttu-id="6e655-172">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6e655-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e655-173">応答</span><span class="sxs-lookup"><span data-stu-id="6e655-173">Response</span></span>

<span data-ttu-id="6e655-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6e655-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e655-176">例</span><span class="sxs-lookup"><span data-stu-id="6e655-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e655-177">要求</span><span class="sxs-lookup"><span data-stu-id="6e655-177">Request</span></span>
<span data-ttu-id="6e655-178">最初の例では、名前で拡張情報を参照し、指定されたメッセージの拡張情報を削除します。</span><span class="sxs-lookup"><span data-stu-id="6e655-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="6e655-179">2 番目の例では、指定されたグループ イベントの拡張機能を削除します。</span><span class="sxs-lookup"><span data-stu-id="6e655-179">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="6e655-180">応答</span><span class="sxs-lookup"><span data-stu-id="6e655-180">Response</span></span>
<span data-ttu-id="6e655-181">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6e655-181">Here is an example of the response.</span></span>
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
