---
author: kevklam
ms.author: kevinlam
title: アクセス許可の付与
description: 指定したリンクを使用するためのアクセス許可の一覧をユーザーに付与する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4163c93179ecc55b71c76d1d18d64bf8dae36b96
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349566"
---
# <a name="grant-permission"></a><span data-ttu-id="b16e3-103">アクセス許可の付与</span><span class="sxs-lookup"><span data-stu-id="b16e3-103">Grant permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b16e3-104">[アクセス許可][]で表されるリンクへのアクセスをユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="b16e3-104">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="b16e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b16e3-105">Permissions</span></span>

<span data-ttu-id="b16e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b16e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b16e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b16e3-108">Permission type</span></span>                   | <span data-ttu-id="b16e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b16e3-109">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b16e3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b16e3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b16e3-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b16e3-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b16e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b16e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b16e3-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="b16e3-113">Not supported</span></span>    |
|<span data-ttu-id="b16e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b16e3-114">Application</span></span> | <span data-ttu-id="b16e3-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b16e3-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b16e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b16e3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="b16e3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b16e3-117">Request headers</span></span>

| <span data-ttu-id="b16e3-118">名前</span><span class="sxs-lookup"><span data-stu-id="b16e3-118">Name</span></span>          | <span data-ttu-id="b16e3-119">説明</span><span class="sxs-lookup"><span data-stu-id="b16e3-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="b16e3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b16e3-120">Authorization</span></span> | <span data-ttu-id="b16e3-121">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="b16e3-121">Bearer \{token\}.</span></span> <span data-ttu-id="b16e3-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="b16e3-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b16e3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b16e3-123">Request body</span></span>

<span data-ttu-id="b16e3-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b16e3-124">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="b16e3-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b16e3-125">Parameter</span></span>          | <span data-ttu-id="b16e3-126">型</span><span class="sxs-lookup"><span data-stu-id="b16e3-126">Type</span></span>                           | <span data-ttu-id="b16e3-127">説明</span><span class="sxs-lookup"><span data-stu-id="b16e3-127">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="b16e3-128">recipients</span><span class="sxs-lookup"><span data-stu-id="b16e3-128">recipients</span></span>         | <span data-ttu-id="b16e3-129">コレクション ([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="b16e3-129">Collection([driveRecipient][])</span></span> | <span data-ttu-id="b16e3-130">アクセスを受信する受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="b16e3-130">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="b16e3-131">roles</span><span class="sxs-lookup"><span data-stu-id="b16e3-131">roles</span></span>              | <span data-ttu-id="b16e3-132">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="b16e3-132">Collection(String)</span></span>             | <span data-ttu-id="b16e3-133">リンクが "既存のアクセス" リンクの場合は、ユーザーに付与する役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="b16e3-133">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="b16e3-134">それ以外の場合は、リンクのロールと一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b16e3-134">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="b16e3-135">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration-values)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b16e3-135">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="response"></a><span data-ttu-id="b16e3-136">応答</span><span class="sxs-lookup"><span data-stu-id="b16e3-136">Response</span></span>

<span data-ttu-id="b16e3-137">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[permission][]コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b16e3-137">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="b16e3-138">更新されたリンクを表す[アクセス許可][]は、成功時に結果セットで常に返されます。</span><span class="sxs-lookup"><span data-stu-id="b16e3-138">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="b16e3-139">更新されたリンクは、' scope ' プロパティを含む ' link ' ファセットが存在することで識別できます。</span><span class="sxs-lookup"><span data-stu-id="b16e3-139">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="b16e3-140">場合によっては、更新されたリンクの URL が元のリンクと異なる場合があります。その場合は、新しい URL を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b16e3-140">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="b16e3-141">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b16e3-141">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="b16e3-142">例</span><span class="sxs-lookup"><span data-stu-id="b16e3-142">Example</span></span>

<span data-ttu-id="b16e3-143">この例では、リンク上の他の既存のアクセス許可を変更せずに、共有リンクへの john@contoso.com および ryan@external.com アクセスをユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="b16e3-143">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="b16e3-144">要求</span><span class="sxs-lookup"><span data-stu-id="b16e3-144">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b16e3-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b16e3-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST https://graph.microsoft.com/beta/shares/{encoded-sharing-url}/permission/grant
Content-type: application/json

{
  "recipients": [
    {
      "email": "john@contoso.com"
    },
    {
      "email": "ryan@external.com"
    }
  ],
  "roles": ["read"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b16e3-146">C#</span><span class="sxs-lookup"><span data-stu-id="b16e3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b16e3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b16e3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b16e3-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="b16e3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b16e3-149">Java</span><span class="sxs-lookup"><span data-stu-id="b16e3-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b16e3-150">応答</span><span class="sxs-lookup"><span data-stu-id="b16e3-150">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "5fab944a-47ec-48d0-a9b5-5178a926d00f",
      "link": {
        "preventsDownload": false,
        "scope": "users",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/design/EZexPoDjW4dMtKFUfAl6BK4BvIUuss52hLYzihBfx-PD6Q"
      },
      "roles": [
        "read"
      ]
    }
  ]
}
```

><span data-ttu-id="b16e3-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b16e3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="b16e3-153">リンクが[既存の access](../resources/permission.md#existing-access-link)リンクの場合は、次のものを表す追加のアクセス許可が返されます。</span><span class="sxs-lookup"><span data-stu-id="b16e3-153">If the link is an [existing access](../resources/permission.md#existing-access-link) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="b16e3-154">アクセスが正常に付与された受信者を表す、ユーザーの種類のアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="b16e3-154">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="b16e3-155">これらは、 **grantedTo**プロパティのプレゼンスによって識別できます。</span><span class="sxs-lookup"><span data-stu-id="b16e3-155">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="b16e3-156">アクセス権を取得するために、認識されない外部ユーザーに送信する必要がある招待を表すリンクの種類のアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="b16e3-156">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="b16e3-157">これらは、[招待](../resources/sharinginvitation.md)ファセットが存在することによって識別できます。</span><span class="sxs-lookup"><span data-stu-id="b16e3-157">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="b16e3-158">これらのエントリには、招待 URL の[リンク][sharing-link]が含まれており、grantedToIdentities コレクションは、そのリンクを送信するユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="b16e3-158">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "00000000-0000-0000-0000-000000000000",
      "link": {
        "preventsDownload": false,
        "scope": "existingAccess",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/teams/design/shareddocs/Document.docx"
      },
      "roles": [
        "read"
      ]
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "John Smith",
          "email": "john@contoso.com",
          "id": "47aecee2-d061-4730-8ecb-4c61360441ae"
        }
      },
      "id": "aTowIy5mfG1lbWJlcnNoaXB8bGltaXRlZDJAa2xhbW9kYi5vbm1pY3Jvc29mdC5jb20",
      "roles": [
        "read"
      ]
    },
    {
      "grantedToIdentities": [
        {
          "user": {
            "email": "ryan@external.com"
          }
        }
      ],
      "invitation": {
        "signInRequired": true
      },
      "roles": [
        "read"
      ],
      "link": {
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/teams/design/EZexPoDjW4dMtKFUfAl6BK4Bw_F7gFH63O310A7lDtK0mQ"
      }
    }
  ]
}

```

><span data-ttu-id="b16e3-159">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b16e3-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b16e3-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b16e3-160">All the properties will be returned from an actual call.</span></span>



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[permission]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
