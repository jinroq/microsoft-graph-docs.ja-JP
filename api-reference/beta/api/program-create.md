---
title: プログラムを作成する
description: Azure AD access レビュー機能で、新しいプログラムオブジェクトを作成します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0a446fd04bd79763120cbaa01134f5cbabbcbf52
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978610"
---
# <a name="create-program"></a><span data-ttu-id="7e0b3-103">プログラムを作成する</span><span class="sxs-lookup"><span data-stu-id="7e0b3-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e0b3-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[プログラム](../resources/program.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e0b3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7e0b3-105">Permissions</span></span>
<span data-ttu-id="7e0b3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e0b3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e0b3-108">Permission type</span></span>                        | <span data-ttu-id="7e0b3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e0b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e0b3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e0b3-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e0b3-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="7e0b3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e0b3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-113">Not supported.</span></span> |
|<span data-ttu-id="7e0b3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e0b3-114">Application</span></span>                            | <span data-ttu-id="7e0b3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-115">Not supported.</span></span> |

<span data-ttu-id="7e0b3-116">サインインしているユーザーは、プログラムを作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="7e0b3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e0b3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="7e0b3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e0b3-118">Request headers</span></span>
| <span data-ttu-id="7e0b3-119">名前</span><span class="sxs-lookup"><span data-stu-id="7e0b3-119">Name</span></span>         | <span data-ttu-id="7e0b3-120">型</span><span class="sxs-lookup"><span data-stu-id="7e0b3-120">Type</span></span>        | <span data-ttu-id="7e0b3-121">説明</span><span class="sxs-lookup"><span data-stu-id="7e0b3-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7e0b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e0b3-122">Authorization</span></span> | <span data-ttu-id="7e0b3-123">string</span><span class="sxs-lookup"><span data-stu-id="7e0b3-123">string</span></span> | <span data-ttu-id="7e0b3-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e0b3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e0b3-126">Request body</span></span>
<span data-ttu-id="7e0b3-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="7e0b3-128">次の表に、プログラムの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="7e0b3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e0b3-129">Property</span></span>     | <span data-ttu-id="7e0b3-130">型</span><span class="sxs-lookup"><span data-stu-id="7e0b3-130">Type</span></span>        | <span data-ttu-id="7e0b3-131">説明</span><span class="sxs-lookup"><span data-stu-id="7e0b3-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="7e0b3-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="7e0b3-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="7e0b3-134">応答</span><span class="sxs-lookup"><span data-stu-id="7e0b3-134">Response</span></span>
<span data-ttu-id="7e0b3-135">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e0b3-136">例</span><span class="sxs-lookup"><span data-stu-id="7e0b3-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e0b3-137">要求</span><span class="sxs-lookup"><span data-stu-id="7e0b3-137">Request</span></span>
<span data-ttu-id="7e0b3-138">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e0b3-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7e0b3-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e0b3-140">C#</span><span class="sxs-lookup"><span data-stu-id="7e0b3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e0b3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e0b3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e0b3-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="7e0b3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e0b3-143">Java</span><span class="sxs-lookup"><span data-stu-id="7e0b3-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-program-from-programs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e0b3-144">応答</span><span class="sxs-lookup"><span data-stu-id="7e0b3-144">Response</span></span>
><span data-ttu-id="7e0b3-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="7e0b3-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e0b3-147">See also</span></span>

| <span data-ttu-id="7e0b3-148">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e0b3-148">Method</span></span>           | <span data-ttu-id="7e0b3-149">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7e0b3-149">Return Type</span></span>    |<span data-ttu-id="7e0b3-150">説明</span><span class="sxs-lookup"><span data-stu-id="7e0b3-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e0b3-151">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="7e0b3-151">List programs</span></span>](program-list.md) | <span data-ttu-id="7e0b3-152">[プログラム](../resources/program.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7e0b3-152">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="7e0b3-153">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-153">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="7e0b3-154">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7e0b3-154">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="7e0b3-155">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7e0b3-155">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="7e0b3-156">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-156">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="7e0b3-157">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="7e0b3-157">Update program</span></span>](program-update.md) |  [<span data-ttu-id="7e0b3-158">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e0b3-158">program</span></span>](../resources/program.md)| <span data-ttu-id="7e0b3-159">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-159">Update a program.</span></span>|
|[<span data-ttu-id="7e0b3-160">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="7e0b3-160">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="7e0b3-161">programControl</span><span class="sxs-lookup"><span data-stu-id="7e0b3-161">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="7e0b3-162">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="7e0b3-162">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
