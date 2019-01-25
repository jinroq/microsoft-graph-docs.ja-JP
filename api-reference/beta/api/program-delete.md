---
title: プログラムを削除します。
description: Azure AD のレビュー機能にアクセス、プログラム オブジェクトを削除します。
localization_priority: Normal
ms.openlocfilehash: 930367e6c61d354655e73fb7ece9c8776e15f34e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519508"
---
# <a name="delete-program"></a><span data-ttu-id="f2c7f-103">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c7f-104">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、[プログラム](../resources/program.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="f2c7f-105">まだプログラムを削除しないで`programControl`にリンクして、それらのアクセスのレビュー最初を削除またはプログラムからのリンクを解除し、別のプログラムにリンクします。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="f2c7f-106">また、組み込みの既定のプログラムを削除できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="f2c7f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f2c7f-107">Permissions</span></span>
<span data-ttu-id="f2c7f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c7f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2c7f-110">Permission type</span></span>                        | <span data-ttu-id="f2c7f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2c7f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2c7f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2c7f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2c7f-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f2c7f-113"></span></span>  <span data-ttu-id="f2c7f-114">サインインしているユーザーは、プログラムを作成することを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="f2c7f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2c7f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2c7f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-116">Not supported.</span></span> |
|<span data-ttu-id="f2c7f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2c7f-117">Application</span></span>                            | <span data-ttu-id="f2c7f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2c7f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2c7f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="f2c7f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2c7f-120">Request headers</span></span>
| <span data-ttu-id="f2c7f-121">名前</span><span class="sxs-lookup"><span data-stu-id="f2c7f-121">Name</span></span>         | <span data-ttu-id="f2c7f-122">型</span><span class="sxs-lookup"><span data-stu-id="f2c7f-122">Type</span></span>        | <span data-ttu-id="f2c7f-123">説明</span><span class="sxs-lookup"><span data-stu-id="f2c7f-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f2c7f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2c7f-124">Authorization</span></span> | <span data-ttu-id="f2c7f-125">string</span><span class="sxs-lookup"><span data-stu-id="f2c7f-125">string</span></span> | <span data-ttu-id="f2c7f-126">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="f2c7f-126">Bearer \{token\}.</span></span> <span data-ttu-id="f2c7f-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2c7f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2c7f-128">Request body</span></span>
<span data-ttu-id="f2c7f-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f2c7f-130">応答</span><span class="sxs-lookup"><span data-stu-id="f2c7f-130">Response</span></span>
<span data-ttu-id="f2c7f-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2c7f-133">例</span><span class="sxs-lookup"><span data-stu-id="f2c7f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2c7f-134">要求</span><span class="sxs-lookup"><span data-stu-id="f2c7f-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="f2c7f-135">応答</span><span class="sxs-lookup"><span data-stu-id="f2c7f-135">Response</span></span>
><span data-ttu-id="f2c7f-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f2c7f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
