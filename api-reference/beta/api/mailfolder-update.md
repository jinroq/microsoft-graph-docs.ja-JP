---
title: MailFolder を更新します。
description: MailFolder オブジェクトのプロパティを更新します。
ms.openlocfilehash: 13851d4d538083658abd6ddba7d9368071b5372e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070399"
---
# <a name="update-mailfolder"></a><span data-ttu-id="f0b72-103">MailFolder を更新します。</span><span class="sxs-lookup"><span data-stu-id="f0b72-103">Update mailFolder</span></span>

> <span data-ttu-id="f0b72-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0b72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0b72-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0b72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0b72-106">[MailFolder](../resources/mailfolder.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f0b72-106">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0b72-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0b72-107">Permissions</span></span>
<span data-ttu-id="f0b72-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0b72-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0b72-110">Permission type</span></span>      | <span data-ttu-id="f0b72-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0b72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0b72-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0b72-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0b72-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0b72-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f0b72-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0b72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0b72-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0b72-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f0b72-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0b72-116">Application</span></span> | <span data-ttu-id="f0b72-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0b72-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0b72-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0b72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f0b72-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0b72-119">Request headers</span></span>
| <span data-ttu-id="f0b72-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0b72-120">Header</span></span>       | <span data-ttu-id="f0b72-121">値</span><span class="sxs-lookup"><span data-stu-id="f0b72-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0b72-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0b72-122">Authorization</span></span>  | <span data-ttu-id="f0b72-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0b72-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0b72-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0b72-125">Content-Type</span></span>  | <span data-ttu-id="f0b72-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f0b72-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0b72-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0b72-128">Request body</span></span>
<span data-ttu-id="f0b72-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f0b72-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f0b72-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0b72-132">Property</span></span>     | <span data-ttu-id="f0b72-133">型</span><span class="sxs-lookup"><span data-stu-id="f0b72-133">Type</span></span>   |<span data-ttu-id="f0b72-134">説明</span><span class="sxs-lookup"><span data-stu-id="f0b72-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0b72-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f0b72-135">displayName</span></span>|<span data-ttu-id="f0b72-136">String</span><span class="sxs-lookup"><span data-stu-id="f0b72-136">String</span></span>|<span data-ttu-id="f0b72-137">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="f0b72-137">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="f0b72-138">応答</span><span class="sxs-lookup"><span data-stu-id="f0b72-138">Response</span></span>
<span data-ttu-id="f0b72-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0b72-139">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0b72-140">例</span><span class="sxs-lookup"><span data-stu-id="f0b72-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f0b72-141">要求</span><span class="sxs-lookup"><span data-stu-id="f0b72-141">Request</span></span>
<span data-ttu-id="f0b72-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0b72-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="f0b72-143">応答</span><span class="sxs-lookup"><span data-stu-id="f0b72-143">Response</span></span>
<span data-ttu-id="f0b72-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f0b72-144">The following is an example of the response.</span></span>
><span data-ttu-id="f0b72-145">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f0b72-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f0b72-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f0b72-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
