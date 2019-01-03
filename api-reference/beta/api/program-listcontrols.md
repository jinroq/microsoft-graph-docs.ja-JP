---
title: プログラムのリスト programControls
description: Azure AD にアクセスが機能を確認し、すべてのデバッギング オブジェクト、特定のプログラムにリンクされています。
ms.openlocfilehash: 78b28851dadfa1c24bc5bc0556b1c471e7bc09e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066465"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="1de26-103">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="1de26-103">List programControls of a program</span></span>

> <span data-ttu-id="1de26-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1de26-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1de26-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de26-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1de26-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、すべての[デバッギング](../resources/programcontrol.md)オブジェクト、特定のプログラムにリンクされている一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="1de26-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="1de26-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1de26-107">Permissions</span></span>
<span data-ttu-id="1de26-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1de26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1de26-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1de26-110">Permission type</span></span>                        | <span data-ttu-id="1de26-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1de26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1de26-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1de26-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1de26-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="1de26-113"></span></span>  <span data-ttu-id="1de26-114">サインインしているユーザーは、プログラムを読むことを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="1de26-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="1de26-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1de26-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1de26-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de26-116">Not supported.</span></span> |
|<span data-ttu-id="1de26-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1de26-117">Application</span></span>                            | <span data-ttu-id="1de26-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de26-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1de26-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1de26-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="1de26-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1de26-120">Request headers</span></span>
| <span data-ttu-id="1de26-121">名前</span><span class="sxs-lookup"><span data-stu-id="1de26-121">Name</span></span>         | <span data-ttu-id="1de26-122">型</span><span class="sxs-lookup"><span data-stu-id="1de26-122">Type</span></span>        | <span data-ttu-id="1de26-123">説明</span><span class="sxs-lookup"><span data-stu-id="1de26-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1de26-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1de26-124">Authorization</span></span> | <span data-ttu-id="1de26-125">string</span><span class="sxs-lookup"><span data-stu-id="1de26-125">string</span></span> | <span data-ttu-id="1de26-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="1de26-126">Bearer \{token\}.</span></span> <span data-ttu-id="1de26-127">必須。</span><span class="sxs-lookup"><span data-stu-id="1de26-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1de26-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1de26-128">Request body</span></span>
<span data-ttu-id="1de26-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="1de26-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="1de26-130">応答</span><span class="sxs-lookup"><span data-stu-id="1de26-130">Response</span></span>
<span data-ttu-id="1de26-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文の[デバッギング](../resources/programcontrol.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="1de26-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1de26-132">例</span><span class="sxs-lookup"><span data-stu-id="1de26-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1de26-133">要求</span><span class="sxs-lookup"><span data-stu-id="1de26-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs('673a7379-9c38-4f01-bd9d-4fda7260b807')/controls
```

##### <a name="response"></a><span data-ttu-id="1de26-134">応答</span><span class="sxs-lookup"><span data-stu-id="1de26-134">Response</span></span>
><span data-ttu-id="1de26-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1de26-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->