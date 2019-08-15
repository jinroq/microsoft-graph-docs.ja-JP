---
title: プログラムの更新
description: Azure AD access レビュー機能で、既存のプログラムオブジェクトを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c1f50f81d4c87283ce686da5626b5482055ec5fd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412496"
---
# <a name="update-program"></a><span data-ttu-id="93a72-103">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="93a72-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93a72-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[プログラム](../resources/program.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="93a72-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="93a72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="93a72-105">Permissions</span></span>
<span data-ttu-id="93a72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93a72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93a72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="93a72-108">Permission type</span></span>                        | <span data-ttu-id="93a72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="93a72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="93a72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="93a72-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="93a72-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93a72-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="93a72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="93a72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93a72-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93a72-113">Not supported.</span></span> |
|<span data-ttu-id="93a72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="93a72-114">Application</span></span>                            | <span data-ttu-id="93a72-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93a72-115">Not supported.</span></span> |

<span data-ttu-id="93a72-116">サインインしているユーザーは、プログラムの更新を許可するディレクトリロールにある必要もあります。</span><span class="sxs-lookup"><span data-stu-id="93a72-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="93a72-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="93a72-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="93a72-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="93a72-118">Request headers</span></span>
| <span data-ttu-id="93a72-119">名前</span><span class="sxs-lookup"><span data-stu-id="93a72-119">Name</span></span>         | <span data-ttu-id="93a72-120">型</span><span class="sxs-lookup"><span data-stu-id="93a72-120">Type</span></span>        | <span data-ttu-id="93a72-121">説明</span><span class="sxs-lookup"><span data-stu-id="93a72-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="93a72-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93a72-122">Authorization</span></span> | <span data-ttu-id="93a72-123">string</span><span class="sxs-lookup"><span data-stu-id="93a72-123">string</span></span> | <span data-ttu-id="93a72-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="93a72-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93a72-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="93a72-126">Request body</span></span>
<span data-ttu-id="93a72-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="93a72-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="93a72-128">次の表は、プログラムの更新時に提供できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="93a72-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="93a72-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93a72-129">Property</span></span>     | <span data-ttu-id="93a72-130">型</span><span class="sxs-lookup"><span data-stu-id="93a72-130">Type</span></span>        | <span data-ttu-id="93a72-131">説明</span><span class="sxs-lookup"><span data-stu-id="93a72-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="93a72-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="93a72-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="93a72-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="93a72-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="93a72-134">応答</span><span class="sxs-lookup"><span data-stu-id="93a72-134">Response</span></span>
<span data-ttu-id="93a72-135">成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="93a72-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93a72-136">例</span><span class="sxs-lookup"><span data-stu-id="93a72-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93a72-137">要求</span><span class="sxs-lookup"><span data-stu-id="93a72-137">Request</span></span>
<span data-ttu-id="93a72-138">要求本文で、変更する[プログラム](../resources/program.md)オブジェクトのパラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="93a72-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93a72-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="93a72-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93a72-140">C#</span><span class="sxs-lookup"><span data-stu-id="93a72-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93a72-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93a72-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93a72-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="93a72-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93a72-143">応答</span><span class="sxs-lookup"><span data-stu-id="93a72-143">Response</span></span>
><span data-ttu-id="93a72-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="93a72-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="93a72-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="93a72-146">See also</span></span>

| <span data-ttu-id="93a72-147">メソッド</span><span class="sxs-lookup"><span data-stu-id="93a72-147">Method</span></span>           | <span data-ttu-id="93a72-148">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93a72-148">Return Type</span></span>    |<span data-ttu-id="93a72-149">説明</span><span class="sxs-lookup"><span data-stu-id="93a72-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93a72-150">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="93a72-150">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="93a72-151">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="93a72-151">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="93a72-152">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93a72-152">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="93a72-153">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="93a72-153">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="93a72-154">programControl</span><span class="sxs-lookup"><span data-stu-id="93a72-154">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="93a72-155">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="93a72-155">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
