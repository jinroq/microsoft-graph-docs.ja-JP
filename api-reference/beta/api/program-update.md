---
title: プログラムの更新
description: Azure AD access レビュー機能で、既存のプログラムオブジェクトを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 82dc447e977aebd32ed07fa4c623bfcbed9b2464
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360814"
---
# <a name="update-program"></a><span data-ttu-id="ebcd6-103">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="ebcd6-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebcd6-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[プログラム](../resources/program.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebcd6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ebcd6-105">Permissions</span></span>
<span data-ttu-id="ebcd6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcd6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebcd6-108">Permission type</span></span>                        | <span data-ttu-id="ebcd6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebcd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebcd6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebcd6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebcd6-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcd6-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="ebcd6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebcd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcd6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-113">Not supported.</span></span> |
|<span data-ttu-id="ebcd6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebcd6-114">Application</span></span>                            | <span data-ttu-id="ebcd6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-115">Not supported.</span></span> |

<span data-ttu-id="ebcd6-116">サインインしているユーザーは、プログラムの更新を許可するディレクトリロールにある必要もあります。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="ebcd6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebcd6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="ebcd6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebcd6-118">Request headers</span></span>
| <span data-ttu-id="ebcd6-119">名前</span><span class="sxs-lookup"><span data-stu-id="ebcd6-119">Name</span></span>         | <span data-ttu-id="ebcd6-120">型</span><span class="sxs-lookup"><span data-stu-id="ebcd6-120">Type</span></span>        | <span data-ttu-id="ebcd6-121">説明</span><span class="sxs-lookup"><span data-stu-id="ebcd6-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ebcd6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebcd6-122">Authorization</span></span> | <span data-ttu-id="ebcd6-123">string</span><span class="sxs-lookup"><span data-stu-id="ebcd6-123">string</span></span> | <span data-ttu-id="ebcd6-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebcd6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebcd6-126">Request body</span></span>
<span data-ttu-id="ebcd6-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="ebcd6-128">次の表は、プログラムの更新時に提供できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="ebcd6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebcd6-129">Property</span></span>     | <span data-ttu-id="ebcd6-130">型</span><span class="sxs-lookup"><span data-stu-id="ebcd6-130">Type</span></span>        | <span data-ttu-id="ebcd6-131">説明</span><span class="sxs-lookup"><span data-stu-id="ebcd6-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="ebcd6-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="ebcd6-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="ebcd6-134">応答</span><span class="sxs-lookup"><span data-stu-id="ebcd6-134">Response</span></span>
<span data-ttu-id="ebcd6-135">成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebcd6-136">例</span><span class="sxs-lookup"><span data-stu-id="ebcd6-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebcd6-137">要求</span><span class="sxs-lookup"><span data-stu-id="ebcd6-137">Request</span></span>
<span data-ttu-id="ebcd6-138">要求本文で、変更する[プログラム](../resources/program.md)オブジェクトのパラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ebcd6-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ebcd6-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ebcd6-140">C#</span><span class="sxs-lookup"><span data-stu-id="ebcd6-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ebcd6-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebcd6-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ebcd6-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="ebcd6-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ebcd6-143">Java</span><span class="sxs-lookup"><span data-stu-id="ebcd6-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ebcd6-144">応答</span><span class="sxs-lookup"><span data-stu-id="ebcd6-144">Response</span></span>
><span data-ttu-id="ebcd6-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ebcd6-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="ebcd6-147">See also</span></span>

| <span data-ttu-id="ebcd6-148">メソッド</span><span class="sxs-lookup"><span data-stu-id="ebcd6-148">Method</span></span>           | <span data-ttu-id="ebcd6-149">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ebcd6-149">Return Type</span></span>    |<span data-ttu-id="ebcd6-150">説明</span><span class="sxs-lookup"><span data-stu-id="ebcd6-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebcd6-151">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ebcd6-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="ebcd6-152">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ebcd6-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="ebcd6-153">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ebcd6-154">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="ebcd6-154">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="ebcd6-155">programControl</span><span class="sxs-lookup"><span data-stu-id="ebcd6-155">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="ebcd6-156">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="ebcd6-156">Add a programControl to a program.</span></span>|

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
