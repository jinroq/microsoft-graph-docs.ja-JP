---
title: リスト programControlTypes
description: Azure AD のレビュー機能にアクセス、すべての programControlType オブジェクトを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: ae5a2298d3c0f542f7d8fd766f412b8cf5648730
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860887"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="4ef99-103">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="4ef99-103">List programControlTypes</span></span>

> <span data-ttu-id="4ef99-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4ef99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ef99-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ef99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ef99-106">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、 [programControlType](../resources/programcontroltype.md)のすべてのオブジェクトを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4ef99-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ef99-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ef99-107">Permissions</span></span>
<span data-ttu-id="4ef99-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ef99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef99-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ef99-110">Permission type</span></span>                        | <span data-ttu-id="4ef99-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ef99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ef99-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ef99-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ef99-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="4ef99-113"></span></span>  <span data-ttu-id="4ef99-114">サインインしているユーザーは、プログラムを読むことを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="4ef99-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="4ef99-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ef99-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ef99-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ef99-116">Not supported.</span></span> |
|<span data-ttu-id="4ef99-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ef99-117">Application</span></span>                            | <span data-ttu-id="4ef99-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ef99-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ef99-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ef99-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="4ef99-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ef99-120">Request headers</span></span>
| <span data-ttu-id="4ef99-121">名前</span><span class="sxs-lookup"><span data-stu-id="4ef99-121">Name</span></span>         | <span data-ttu-id="4ef99-122">種類</span><span class="sxs-lookup"><span data-stu-id="4ef99-122">Type</span></span>        | <span data-ttu-id="4ef99-123">説明</span><span class="sxs-lookup"><span data-stu-id="4ef99-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4ef99-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef99-124">Authorization</span></span> | <span data-ttu-id="4ef99-125">string</span><span class="sxs-lookup"><span data-stu-id="4ef99-125">string</span></span> | <span data-ttu-id="4ef99-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="4ef99-126">Bearer \{token\}.</span></span> <span data-ttu-id="4ef99-127">必須。</span><span class="sxs-lookup"><span data-stu-id="4ef99-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ef99-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ef99-128">Request body</span></span>
<span data-ttu-id="4ef99-129">要求の本体を提供する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="4ef99-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="4ef99-130">応答</span><span class="sxs-lookup"><span data-stu-id="4ef99-130">Response</span></span>
<span data-ttu-id="4ef99-131">かどうかは成功すると、このメソッドが返されます、`200, OK`応答コードおよび応答の本文に[programControlType](../resources/programcontroltype.md)オブジェクトの配列。</span><span class="sxs-lookup"><span data-stu-id="4ef99-131">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ef99-132">例</span><span class="sxs-lookup"><span data-stu-id="4ef99-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ef99-133">要求</span><span class="sxs-lookup"><span data-stu-id="4ef99-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="4ef99-134">応答</span><span class="sxs-lookup"><span data-stu-id="4ef99-134">Response</span></span>
><span data-ttu-id="4ef99-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4ef99-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4ef99-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ef99-137">See also</span></span>

| <span data-ttu-id="4ef99-138">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ef99-138">Method</span></span>           | <span data-ttu-id="4ef99-139">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4ef99-139">Return Type</span></span>    |<span data-ttu-id="4ef99-140">説明</span><span class="sxs-lookup"><span data-stu-id="4ef99-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ef99-141">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="4ef99-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="4ef99-142">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4ef99-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="4ef99-143">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ef99-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
