---
title: プログラムの更新
description: Azure AD access レビュー機能で、既存のプログラムオブジェクトを更新します。
localization_priority: Normal
ms.openlocfilehash: bc4971dd825b031d786d50aeffe3a96eb5a7ef80
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264100"
---
# <a name="update-program"></a><span data-ttu-id="3704e-103">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="3704e-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3704e-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[プログラム](../resources/program.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3704e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3704e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3704e-105">Permissions</span></span>
<span data-ttu-id="3704e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3704e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3704e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3704e-108">Permission type</span></span>                        | <span data-ttu-id="3704e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3704e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3704e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3704e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3704e-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3704e-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="3704e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3704e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3704e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3704e-113">Not supported.</span></span> |
|<span data-ttu-id="3704e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3704e-114">Application</span></span>                            | <span data-ttu-id="3704e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3704e-115">Not supported.</span></span> |

<span data-ttu-id="3704e-116">サインインしているユーザーは、プログラムの更新を許可するディレクトリロールにある必要もあります。</span><span class="sxs-lookup"><span data-stu-id="3704e-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="3704e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3704e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="3704e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3704e-118">Request headers</span></span>
| <span data-ttu-id="3704e-119">名前</span><span class="sxs-lookup"><span data-stu-id="3704e-119">Name</span></span>         | <span data-ttu-id="3704e-120">型</span><span class="sxs-lookup"><span data-stu-id="3704e-120">Type</span></span>        | <span data-ttu-id="3704e-121">説明</span><span class="sxs-lookup"><span data-stu-id="3704e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3704e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3704e-122">Authorization</span></span> | <span data-ttu-id="3704e-123">string</span><span class="sxs-lookup"><span data-stu-id="3704e-123">string</span></span> | <span data-ttu-id="3704e-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="3704e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3704e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3704e-126">Request body</span></span>
<span data-ttu-id="3704e-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3704e-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="3704e-128">次の表は、プログラムの更新時に提供できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="3704e-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="3704e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3704e-129">Property</span></span>     | <span data-ttu-id="3704e-130">型</span><span class="sxs-lookup"><span data-stu-id="3704e-130">Type</span></span>        | <span data-ttu-id="3704e-131">説明</span><span class="sxs-lookup"><span data-stu-id="3704e-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="3704e-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3704e-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="3704e-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="3704e-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="3704e-134">応答</span><span class="sxs-lookup"><span data-stu-id="3704e-134">Response</span></span>
<span data-ttu-id="3704e-135">成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3704e-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3704e-136">例</span><span class="sxs-lookup"><span data-stu-id="3704e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3704e-137">要求</span><span class="sxs-lookup"><span data-stu-id="3704e-137">Request</span></span>
<span data-ttu-id="3704e-138">要求本文で、変更する[プログラム](../resources/program.md)オブジェクトのパラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3704e-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="3704e-139">応答</span><span class="sxs-lookup"><span data-stu-id="3704e-139">Response</span></span>
><span data-ttu-id="3704e-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3704e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3704e-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3704e-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3704e-143">C#</span><span class="sxs-lookup"><span data-stu-id="3704e-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3704e-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="3704e-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_program-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3704e-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="3704e-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_program-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="3704e-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="3704e-146">See also</span></span>

| <span data-ttu-id="3704e-147">メソッド</span><span class="sxs-lookup"><span data-stu-id="3704e-147">Method</span></span>           | <span data-ttu-id="3704e-148">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3704e-148">Return Type</span></span>    |<span data-ttu-id="3704e-149">説明</span><span class="sxs-lookup"><span data-stu-id="3704e-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3704e-150">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3704e-150">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="3704e-151">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3704e-151">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="3704e-152">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3704e-152">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="3704e-153">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="3704e-153">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="3704e-154">programControl</span><span class="sxs-lookup"><span data-stu-id="3704e-154">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="3704e-155">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="3704e-155">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
