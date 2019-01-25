---
title: メッセージを作成する
description: この API を使用して、新しいメッセージを mailFolder 内に作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 868f6e9b753296f6828ec1537eb04ca232c1991e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514930"
---
# <a name="create-message"></a><span data-ttu-id="71c54-103">メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="71c54-103">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71c54-104">この API を使用して、新しいメッセージを mailFolder 内に作成します。</span><span class="sxs-lookup"><span data-stu-id="71c54-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="71c54-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71c54-105">Permissions</span></span>
<span data-ttu-id="71c54-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c54-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71c54-108">Permission type</span></span>      | <span data-ttu-id="71c54-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71c54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71c54-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71c54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71c54-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c54-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71c54-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71c54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71c54-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c54-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71c54-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71c54-114">Application</span></span> | <span data-ttu-id="71c54-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c54-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71c54-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71c54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="71c54-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71c54-117">Request headers</span></span>
| <span data-ttu-id="71c54-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71c54-118">Header</span></span>       | <span data-ttu-id="71c54-119">値</span><span class="sxs-lookup"><span data-stu-id="71c54-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71c54-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c54-120">Authorization</span></span>  | <span data-ttu-id="71c54-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71c54-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="71c54-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71c54-123">Content-Type</span></span>  | <span data-ttu-id="71c54-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="71c54-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71c54-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="71c54-126">Request body</span></span>
<span data-ttu-id="71c54-127">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="71c54-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71c54-128">応答</span><span class="sxs-lookup"><span data-stu-id="71c54-128">Response</span></span>

<span data-ttu-id="71c54-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71c54-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c54-130">例</span><span class="sxs-lookup"><span data-stu-id="71c54-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71c54-131">要求</span><span class="sxs-lookup"><span data-stu-id="71c54-131">Request</span></span>
<span data-ttu-id="71c54-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71c54-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
<span data-ttu-id="71c54-133">要求本文で、[メッセージ](../resources/message.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="71c54-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71c54-134">応答</span><span class="sxs-lookup"><span data-stu-id="71c54-134">Response</span></span>
<span data-ttu-id="71c54-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71c54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-post-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
