---
title: プログラムの更新
description: Azure AD access レビュー機能で、既存のプログラムオブジェクトを更新します。
localization_priority: Normal
ms.openlocfilehash: ca668a84fc39601d94f71c1666b975f3b61a6802
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611165"
---
# <a name="update-program"></a><span data-ttu-id="e1893-103">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="e1893-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1893-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[プログラム](../resources/program.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e1893-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1893-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1893-105">Permissions</span></span>
<span data-ttu-id="e1893-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1893-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1893-108">Permission type</span></span>                        | <span data-ttu-id="e1893-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1893-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1893-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1893-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1893-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1893-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="e1893-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1893-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1893-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1893-113">Not supported.</span></span> |
|<span data-ttu-id="e1893-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1893-114">Application</span></span>                            | <span data-ttu-id="e1893-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1893-115">Not supported.</span></span> |

<span data-ttu-id="e1893-116">サインインしているユーザーは、プログラムの更新を許可するディレクトリロールにある必要もあります。</span><span class="sxs-lookup"><span data-stu-id="e1893-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="e1893-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1893-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="e1893-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1893-118">Request headers</span></span>
| <span data-ttu-id="e1893-119">名前</span><span class="sxs-lookup"><span data-stu-id="e1893-119">Name</span></span>         | <span data-ttu-id="e1893-120">型</span><span class="sxs-lookup"><span data-stu-id="e1893-120">Type</span></span>        | <span data-ttu-id="e1893-121">説明</span><span class="sxs-lookup"><span data-stu-id="e1893-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e1893-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1893-122">Authorization</span></span> | <span data-ttu-id="e1893-123">string</span><span class="sxs-lookup"><span data-stu-id="e1893-123">string</span></span> | <span data-ttu-id="e1893-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1893-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1893-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1893-126">Request body</span></span>
<span data-ttu-id="e1893-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1893-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="e1893-128">次の表は、プログラムの更新時に提供できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="e1893-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="e1893-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1893-129">Property</span></span>     | <span data-ttu-id="e1893-130">型</span><span class="sxs-lookup"><span data-stu-id="e1893-130">Type</span></span>        | <span data-ttu-id="e1893-131">説明</span><span class="sxs-lookup"><span data-stu-id="e1893-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="e1893-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1893-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="e1893-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="e1893-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="e1893-134">応答</span><span class="sxs-lookup"><span data-stu-id="e1893-134">Response</span></span>
<span data-ttu-id="e1893-135">成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1893-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1893-136">例</span><span class="sxs-lookup"><span data-stu-id="e1893-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1893-137">要求</span><span class="sxs-lookup"><span data-stu-id="e1893-137">Request</span></span>
<span data-ttu-id="e1893-138">要求本文で、変更する[プログラム](../resources/program.md)オブジェクトのパラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1893-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="e1893-139">応答</span><span class="sxs-lookup"><span data-stu-id="e1893-139">Response</span></span>
><span data-ttu-id="e1893-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e1893-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1893-142">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="e1893-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1893-143">Visual</span><span class="sxs-lookup"><span data-stu-id="e1893-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1893-144">Java</span><span class="sxs-lookup"><span data-stu-id="e1893-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_program-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="e1893-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1893-145">See also</span></span>

| <span data-ttu-id="e1893-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1893-146">Method</span></span>           | <span data-ttu-id="e1893-147">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e1893-147">Return Type</span></span>    |<span data-ttu-id="e1893-148">説明</span><span class="sxs-lookup"><span data-stu-id="e1893-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1893-149">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e1893-149">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="e1893-150">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e1893-150">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="e1893-151">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e1893-151">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="e1893-152">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="e1893-152">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="e1893-153">programControl</span><span class="sxs-lookup"><span data-stu-id="e1893-153">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="e1893-154">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="e1893-154">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
