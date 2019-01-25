---
title: リスト programControls
description: Azure AD アクセスのレビュー機能では、テナント内のすべてのプログラム間でデバッギング オブジェクトがすべてを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 52361e3878445d4f739fd0cd33817d5b254ddc03
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525060"
---
# <a name="list-programcontrols"></a><span data-ttu-id="11748-103">リスト programControls</span><span class="sxs-lookup"><span data-stu-id="11748-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11748-104">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)テナント内のすべてのプログラム間ですべての[デバッギング](../resources/programcontrol.md)オブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="11748-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="11748-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11748-105">Permissions</span></span>
<span data-ttu-id="11748-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11748-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11748-108">Permission type</span></span>                        | <span data-ttu-id="11748-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11748-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="11748-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11748-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="11748-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="11748-111"></span></span>  <span data-ttu-id="11748-112">サインインしているユーザーは、プログラムを読むことを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="11748-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="11748-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11748-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11748-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11748-114">Not supported.</span></span> |
|<span data-ttu-id="11748-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11748-115">Application</span></span>                            | <span data-ttu-id="11748-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11748-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11748-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11748-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="11748-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11748-118">Request headers</span></span>
| <span data-ttu-id="11748-119">名前</span><span class="sxs-lookup"><span data-stu-id="11748-119">Name</span></span>         | <span data-ttu-id="11748-120">型</span><span class="sxs-lookup"><span data-stu-id="11748-120">Type</span></span>        | <span data-ttu-id="11748-121">説明</span><span class="sxs-lookup"><span data-stu-id="11748-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="11748-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11748-122">Authorization</span></span> | <span data-ttu-id="11748-123">string</span><span class="sxs-lookup"><span data-stu-id="11748-123">string</span></span> | <span data-ttu-id="11748-124">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="11748-124">Bearer \{token\}.</span></span> <span data-ttu-id="11748-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="11748-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11748-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="11748-126">Request body</span></span>
<span data-ttu-id="11748-127">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="11748-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="11748-128">応答</span><span class="sxs-lookup"><span data-stu-id="11748-128">Response</span></span>
<span data-ttu-id="11748-129">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文の[デバッギング](../resources/programcontrol.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="11748-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11748-130">例</span><span class="sxs-lookup"><span data-stu-id="11748-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11748-131">要求</span><span class="sxs-lookup"><span data-stu-id="11748-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="11748-132">応答</span><span class="sxs-lookup"><span data-stu-id="11748-132">Response</span></span>
><span data-ttu-id="11748-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="11748-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
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

## <a name="see-also"></a><span data-ttu-id="11748-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="11748-135">See also</span></span>

| <span data-ttu-id="11748-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="11748-136">Method</span></span>           | <span data-ttu-id="11748-137">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="11748-137">Return Type</span></span>    |<span data-ttu-id="11748-138">説明</span><span class="sxs-lookup"><span data-stu-id="11748-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11748-139">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="11748-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="11748-140">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="11748-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="11748-141">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="11748-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
