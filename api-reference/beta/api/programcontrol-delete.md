---
title: デバッギングを削除します。
description: Azure AD のレビュー機能にアクセス、デバッギング オブジェクトを削除します。  プログラムからのアクセス レビューのリンクを解除します。
localization_priority: Normal
ms.openlocfilehash: 7510dfe80f758a75f190402d3ae426138e60bbed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510835"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="9cc11-104">デバッギングを削除します。</span><span class="sxs-lookup"><span data-stu-id="9cc11-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc11-105">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、[デバッギング](../resources/programcontrol.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9cc11-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="9cc11-106">プログラムからのアクセス レビューのリンクを解除します。</span><span class="sxs-lookup"><span data-stu-id="9cc11-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cc11-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9cc11-107">Permissions</span></span>
<span data-ttu-id="9cc11-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cc11-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc11-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9cc11-110">Permission type</span></span>                        | <span data-ttu-id="9cc11-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9cc11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cc11-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9cc11-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cc11-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="9cc11-113"></span></span>  <span data-ttu-id="9cc11-114">サインインしているユーザーは、ディレクトリの役割、デバッギングを削除することを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9cc11-114">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="9cc11-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9cc11-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc11-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cc11-116">Not supported.</span></span> |
|<span data-ttu-id="9cc11-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9cc11-117">Application</span></span>                            | <span data-ttu-id="9cc11-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9cc11-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cc11-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9cc11-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="9cc11-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9cc11-120">Request headers</span></span>
| <span data-ttu-id="9cc11-121">名前</span><span class="sxs-lookup"><span data-stu-id="9cc11-121">Name</span></span>         | <span data-ttu-id="9cc11-122">型</span><span class="sxs-lookup"><span data-stu-id="9cc11-122">Type</span></span>        | <span data-ttu-id="9cc11-123">説明</span><span class="sxs-lookup"><span data-stu-id="9cc11-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9cc11-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc11-124">Authorization</span></span> | <span data-ttu-id="9cc11-125">string</span><span class="sxs-lookup"><span data-stu-id="9cc11-125">string</span></span> | <span data-ttu-id="9cc11-126">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="9cc11-126">Bearer \{token\}.</span></span> <span data-ttu-id="9cc11-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="9cc11-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cc11-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9cc11-128">Request body</span></span>
<span data-ttu-id="9cc11-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9cc11-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9cc11-130">応答</span><span class="sxs-lookup"><span data-stu-id="9cc11-130">Response</span></span>
<span data-ttu-id="9cc11-p106">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9cc11-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc11-133">例</span><span class="sxs-lookup"><span data-stu-id="9cc11-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cc11-134">要求</span><span class="sxs-lookup"><span data-stu-id="9cc11-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="9cc11-135">応答</span><span class="sxs-lookup"><span data-stu-id="9cc11-135">Response</span></span>
><span data-ttu-id="9cc11-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9cc11-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
