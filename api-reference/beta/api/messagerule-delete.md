---
title: messageRule を削除する
description: 指定した messageRule オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1c2b565baf26ae65729630e0dc44dbe09d745ff6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522855"
---
# <a name="delete-messagerule"></a><span data-ttu-id="e40f4-103">messageRule を削除する</span><span class="sxs-lookup"><span data-stu-id="e40f4-103">Delete messageRule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e40f4-104">指定した [messageRule](../resources/messagerule.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e40f4-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e40f4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e40f4-105">Permissions</span></span>
<span data-ttu-id="e40f4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e40f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e40f4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e40f4-108">Permission type</span></span>      | <span data-ttu-id="e40f4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e40f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e40f4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e40f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e40f4-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e40f4-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e40f4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e40f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e40f4-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e40f4-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e40f4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e40f4-114">Application</span></span> | <span data-ttu-id="e40f4-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e40f4-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e40f4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e40f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e40f4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e40f4-117">Request headers</span></span>
| <span data-ttu-id="e40f4-118">名前</span><span class="sxs-lookup"><span data-stu-id="e40f4-118">Name</span></span>       | <span data-ttu-id="e40f4-119">説明</span><span class="sxs-lookup"><span data-stu-id="e40f4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e40f4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e40f4-120">Authorization</span></span>  | <span data-ttu-id="e40f4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e40f4-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e40f4-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e40f4-123">Request body</span></span>
<span data-ttu-id="e40f4-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e40f4-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e40f4-125">応答</span><span class="sxs-lookup"><span data-stu-id="e40f4-125">Response</span></span>
<span data-ttu-id="e40f4-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e40f4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e40f4-128">例</span><span class="sxs-lookup"><span data-stu-id="e40f4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e40f4-129">要求</span><span class="sxs-lookup"><span data-stu-id="e40f4-129">Request</span></span>
<span data-ttu-id="e40f4-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e40f4-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="e40f4-131">応答</span><span class="sxs-lookup"><span data-stu-id="e40f4-131">Response</span></span>
<span data-ttu-id="e40f4-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e40f4-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/messagerule-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
