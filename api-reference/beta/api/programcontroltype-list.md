---
title: ProgramControlTypes のリスト
description: Azure AD access レビュー機能で、すべての programControlType オブジェクトを一覧表示します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3abefa093250360977daeb26dcaefc3bc5b9b883
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978547"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="86c89-103">ProgramControlTypes のリスト</span><span class="sxs-lookup"><span data-stu-id="86c89-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86c89-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[programcontroltype](../resources/programcontroltype.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="86c89-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="86c89-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86c89-105">Permissions</span></span>
<span data-ttu-id="86c89-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86c89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86c89-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86c89-108">Permission type</span></span>                        | <span data-ttu-id="86c89-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86c89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="86c89-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86c89-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="86c89-111">ProgramControl. All、ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="86c89-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="86c89-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86c89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86c89-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c89-113">Not supported.</span></span> |
|<span data-ttu-id="86c89-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86c89-114">Application</span></span>                            | <span data-ttu-id="86c89-115">ProgramControl. All ', ProgramControl.</span><span class="sxs-lookup"><span data-stu-id="86c89-115">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="86c89-116">サインインしているユーザーは、プログラムを読み取ることができるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="86c89-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="86c89-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86c89-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="86c89-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86c89-118">Request headers</span></span>
| <span data-ttu-id="86c89-119">名前</span><span class="sxs-lookup"><span data-stu-id="86c89-119">Name</span></span>         | <span data-ttu-id="86c89-120">型</span><span class="sxs-lookup"><span data-stu-id="86c89-120">Type</span></span>        | <span data-ttu-id="86c89-121">説明</span><span class="sxs-lookup"><span data-stu-id="86c89-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="86c89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86c89-122">Authorization</span></span> | <span data-ttu-id="86c89-123">string</span><span class="sxs-lookup"><span data-stu-id="86c89-123">string</span></span> | <span data-ttu-id="86c89-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="86c89-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86c89-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="86c89-126">Request body</span></span>
<span data-ttu-id="86c89-127">要求本文を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="86c89-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="86c89-128">応答</span><span class="sxs-lookup"><span data-stu-id="86c89-128">Response</span></span>
<span data-ttu-id="86c89-129">成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[programcontroltype](../resources/programcontroltype.md)オブジェクトの配列を返します。</span><span class="sxs-lookup"><span data-stu-id="86c89-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86c89-130">例</span><span class="sxs-lookup"><span data-stu-id="86c89-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86c89-131">要求</span><span class="sxs-lookup"><span data-stu-id="86c89-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="86c89-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="86c89-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86c89-133">C#</span><span class="sxs-lookup"><span data-stu-id="86c89-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86c89-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="86c89-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86c89-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="86c89-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="86c89-136">Java</span><span class="sxs-lookup"><span data-stu-id="86c89-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontroltype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="86c89-137">応答</span><span class="sxs-lookup"><span data-stu-id="86c89-137">Response</span></span>
><span data-ttu-id="86c89-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="86c89-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="86c89-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="86c89-140">See also</span></span>

| <span data-ttu-id="86c89-141">メソッド</span><span class="sxs-lookup"><span data-stu-id="86c89-141">Method</span></span>           | <span data-ttu-id="86c89-142">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="86c89-142">Return Type</span></span>    |<span data-ttu-id="86c89-143">説明</span><span class="sxs-lookup"><span data-stu-id="86c89-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86c89-144">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="86c89-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="86c89-145">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="86c89-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="86c89-146">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="86c89-146">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
