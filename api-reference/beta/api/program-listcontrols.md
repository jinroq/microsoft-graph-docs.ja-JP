---
title: プログラムの programControls を一覧表示する
description: Azure AD access レビュー機能で、特定のプログラムにリンクされているすべての programControl オブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: c809bbf95900875d306a8d2cbb0270f832a4968d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875390"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="04bca-103">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="04bca-103">List programControls of a program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04bca-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、特定のプログラムにリンクされているすべての[programcontrol](../resources/programcontrol.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="04bca-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="04bca-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04bca-105">Permissions</span></span>
<span data-ttu-id="04bca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04bca-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04bca-108">Permission type</span></span>                        | <span data-ttu-id="04bca-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04bca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="04bca-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04bca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="04bca-111">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="04bca-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="04bca-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04bca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04bca-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04bca-113">Not supported.</span></span> |
|<span data-ttu-id="04bca-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04bca-114">Application</span></span>                            | <span data-ttu-id="04bca-115">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="04bca-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="04bca-116">サインインしているユーザーは、プログラムを読み取ることができるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="04bca-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="04bca-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04bca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="04bca-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04bca-118">Request headers</span></span>
| <span data-ttu-id="04bca-119">名前</span><span class="sxs-lookup"><span data-stu-id="04bca-119">Name</span></span>         | <span data-ttu-id="04bca-120">型</span><span class="sxs-lookup"><span data-stu-id="04bca-120">Type</span></span>        | <span data-ttu-id="04bca-121">説明</span><span class="sxs-lookup"><span data-stu-id="04bca-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="04bca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04bca-122">Authorization</span></span> | <span data-ttu-id="04bca-123">string</span><span class="sxs-lookup"><span data-stu-id="04bca-123">string</span></span> | <span data-ttu-id="04bca-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="04bca-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04bca-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="04bca-126">Request body</span></span>
<span data-ttu-id="04bca-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="04bca-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="04bca-128">応答</span><span class="sxs-lookup"><span data-stu-id="04bca-128">Response</span></span>
<span data-ttu-id="04bca-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[programcontrol](../resources/programcontrol.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="04bca-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04bca-130">例</span><span class="sxs-lookup"><span data-stu-id="04bca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04bca-131">要求</span><span class="sxs-lookup"><span data-stu-id="04bca-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="04bca-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="04bca-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04bca-133">C#</span><span class="sxs-lookup"><span data-stu-id="04bca-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-from-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04bca-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="04bca-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-from-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04bca-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="04bca-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-from-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="04bca-136">Java</span><span class="sxs-lookup"><span data-stu-id="04bca-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-from-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04bca-137">応答</span><span class="sxs-lookup"><span data-stu-id="04bca-137">Response</span></span>
><span data-ttu-id="04bca-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="04bca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
