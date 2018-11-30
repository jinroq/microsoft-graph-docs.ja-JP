---
title: MailSearchFolder を更新します。
description: MailSearchFolder オブジェクトの書き込み可能なプロパティを更新します。
ms.openlocfilehash: abe32817c45ee1e05fbb251bd46a31941eb4218b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074513"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="5a64a-103">MailSearchFolder を更新します。</span><span class="sxs-lookup"><span data-stu-id="5a64a-103">Update mailSearchFolder</span></span>

> <span data-ttu-id="5a64a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a64a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a64a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a64a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a64a-106">[MailSearchFolder](../resources/mailsearchfolder.md)オブジェクトの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a64a-106">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a64a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5a64a-107">Permissions</span></span>
<span data-ttu-id="5a64a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a64a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a64a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a64a-110">Permission type</span></span>      | <span data-ttu-id="5a64a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a64a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a64a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5a64a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a64a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a64a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5a64a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a64a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a64a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a64a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5a64a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a64a-116">Application</span></span> | <span data-ttu-id="5a64a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a64a-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a64a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a64a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a64a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a64a-119">Request headers</span></span>
| <span data-ttu-id="5a64a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a64a-120">Header</span></span>       | <span data-ttu-id="5a64a-121">値</span><span class="sxs-lookup"><span data-stu-id="5a64a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5a64a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a64a-122">Authorization</span></span>  | <span data-ttu-id="5a64a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5a64a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a64a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a64a-125">Content-Type</span></span>  | <span data-ttu-id="5a64a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5a64a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5a64a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a64a-128">Request body</span></span>
<span data-ttu-id="5a64a-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5a64a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a64a-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a64a-132">Property</span></span>     | <span data-ttu-id="5a64a-133">型</span><span class="sxs-lookup"><span data-stu-id="5a64a-133">Type</span></span>   |<span data-ttu-id="5a64a-134">説明</span><span class="sxs-lookup"><span data-stu-id="5a64a-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a64a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5a64a-135">displayName</span></span> | <span data-ttu-id="5a64a-136">String</span><span class="sxs-lookup"><span data-stu-id="5a64a-136">String</span></span> | <span data-ttu-id="5a64a-137">[MailFolder](../resources/mailfolder.md)の表示名です。</span><span class="sxs-lookup"><span data-stu-id="5a64a-137">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="5a64a-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="5a64a-138">includeNestedFolders</span></span> | <span data-ttu-id="5a64a-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="5a64a-139">Boolean</span></span> | <span data-ttu-id="5a64a-140">どのメールボックス フォルダー階層を走査する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a64a-140">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="5a64a-141">`true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="5a64a-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="5a64a-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="5a64a-142">sourceFolderIDs</span></span> | <span data-ttu-id="5a64a-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5a64a-143">String collection</span></span> | <span data-ttu-id="5a64a-144">メールボックス フォルダーをマイニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a64a-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="5a64a-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="5a64a-145">filterQuery</span></span> | <span data-ttu-id="5a64a-146">String</span><span class="sxs-lookup"><span data-stu-id="5a64a-146">String</span></span> | <span data-ttu-id="5a64a-147">メッセージをフィルタ リングする OData クエリです。</span><span class="sxs-lookup"><span data-stu-id="5a64a-147">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="5a64a-148">応答</span><span class="sxs-lookup"><span data-stu-id="5a64a-148">Response</span></span>
<span data-ttu-id="5a64a-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5a64a-149">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a64a-150">例</span><span class="sxs-lookup"><span data-stu-id="5a64a-150">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5a64a-151">要求</span><span class="sxs-lookup"><span data-stu-id="5a64a-151">Request</span></span>
<span data-ttu-id="5a64a-152">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a64a-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="5a64a-153">応答</span><span class="sxs-lookup"><span data-stu-id="5a64a-153">Response</span></span>
<span data-ttu-id="5a64a-154">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5a64a-154">The following is an example of the response.</span></span>
><span data-ttu-id="5a64a-155">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5a64a-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5a64a-156">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5a64a-156">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
