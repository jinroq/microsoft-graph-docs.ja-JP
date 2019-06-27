---
title: プログラムを作成する
description: Azure AD access レビュー機能で、新しいプログラムオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 0d2218031e924e7137378a63d932f5533620cc38
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267663"
---
# <a name="create-program"></a><span data-ttu-id="455bb-103">プログラムを作成する</span><span class="sxs-lookup"><span data-stu-id="455bb-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="455bb-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[プログラム](../resources/program.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="455bb-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="455bb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="455bb-105">Permissions</span></span>
<span data-ttu-id="455bb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="455bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="455bb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="455bb-108">Permission type</span></span>                        | <span data-ttu-id="455bb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="455bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="455bb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="455bb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="455bb-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="455bb-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="455bb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="455bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="455bb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="455bb-113">Not supported.</span></span> |
|<span data-ttu-id="455bb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="455bb-114">Application</span></span>                            | <span data-ttu-id="455bb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="455bb-115">Not supported.</span></span> |

<span data-ttu-id="455bb-116">サインインしているユーザーは、プログラムを作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="455bb-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="455bb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="455bb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="455bb-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="455bb-118">Request headers</span></span>
| <span data-ttu-id="455bb-119">名前</span><span class="sxs-lookup"><span data-stu-id="455bb-119">Name</span></span>         | <span data-ttu-id="455bb-120">型</span><span class="sxs-lookup"><span data-stu-id="455bb-120">Type</span></span>        | <span data-ttu-id="455bb-121">説明</span><span class="sxs-lookup"><span data-stu-id="455bb-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="455bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="455bb-122">Authorization</span></span> | <span data-ttu-id="455bb-123">string</span><span class="sxs-lookup"><span data-stu-id="455bb-123">string</span></span> | <span data-ttu-id="455bb-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="455bb-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="455bb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="455bb-126">Request body</span></span>
<span data-ttu-id="455bb-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="455bb-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="455bb-128">次の表に、プログラムの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="455bb-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="455bb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="455bb-129">Property</span></span>     | <span data-ttu-id="455bb-130">型</span><span class="sxs-lookup"><span data-stu-id="455bb-130">Type</span></span>        | <span data-ttu-id="455bb-131">説明</span><span class="sxs-lookup"><span data-stu-id="455bb-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="455bb-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="455bb-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="455bb-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="455bb-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="455bb-134">応答</span><span class="sxs-lookup"><span data-stu-id="455bb-134">Response</span></span>
<span data-ttu-id="455bb-135">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="455bb-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="455bb-136">例</span><span class="sxs-lookup"><span data-stu-id="455bb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="455bb-137">要求</span><span class="sxs-lookup"><span data-stu-id="455bb-137">Request</span></span>
<span data-ttu-id="455bb-138">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="455bb-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="455bb-139">応答</span><span class="sxs-lookup"><span data-stu-id="455bb-139">Response</span></span>
><span data-ttu-id="455bb-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="455bb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="455bb-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="455bb-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="455bb-143">C#</span><span class="sxs-lookup"><span data-stu-id="455bb-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="455bb-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="455bb-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="455bb-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="455bb-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="455bb-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="455bb-146">See also</span></span>

| <span data-ttu-id="455bb-147">メソッド</span><span class="sxs-lookup"><span data-stu-id="455bb-147">Method</span></span>           | <span data-ttu-id="455bb-148">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="455bb-148">Return Type</span></span>    |<span data-ttu-id="455bb-149">説明</span><span class="sxs-lookup"><span data-stu-id="455bb-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="455bb-150">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="455bb-150">List programs</span></span>](program-list.md) | <span data-ttu-id="455bb-151">[プログラム](../resources/program.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="455bb-151">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="455bb-152">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="455bb-152">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="455bb-153">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="455bb-153">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="455bb-154">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="455bb-154">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="455bb-155">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="455bb-155">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="455bb-156">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="455bb-156">Update program</span></span>](program-update.md) |  [<span data-ttu-id="455bb-157">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="455bb-157">program</span></span>](../resources/program.md)| <span data-ttu-id="455bb-158">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="455bb-158">Update a program.</span></span>|
|[<span data-ttu-id="455bb-159">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="455bb-159">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="455bb-160">programControl</span><span class="sxs-lookup"><span data-stu-id="455bb-160">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="455bb-161">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="455bb-161">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
