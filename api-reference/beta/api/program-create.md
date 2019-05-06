---
title: プログラムを作成する
description: Azure AD access レビュー機能で、新しいプログラムオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 87f766917499e6e9d1896ccf64f8fbae2bef813b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593668"
---
# <a name="create-program"></a><span data-ttu-id="1dd67-103">プログラムを作成する</span><span class="sxs-lookup"><span data-stu-id="1dd67-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd67-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[プログラム](../resources/program.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1dd67-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1dd67-105">Permissions</span></span>
<span data-ttu-id="1dd67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dd67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd67-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dd67-108">Permission type</span></span>                        | <span data-ttu-id="1dd67-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dd67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dd67-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dd67-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dd67-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd67-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="1dd67-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dd67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd67-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dd67-113">Not supported.</span></span> |
|<span data-ttu-id="1dd67-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dd67-114">Application</span></span>                            | <span data-ttu-id="1dd67-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dd67-115">Not supported.</span></span> |

<span data-ttu-id="1dd67-116">サインインしているユーザーは、プログラムを作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="1dd67-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="1dd67-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dd67-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="1dd67-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dd67-118">Request headers</span></span>
| <span data-ttu-id="1dd67-119">名前</span><span class="sxs-lookup"><span data-stu-id="1dd67-119">Name</span></span>         | <span data-ttu-id="1dd67-120">型</span><span class="sxs-lookup"><span data-stu-id="1dd67-120">Type</span></span>        | <span data-ttu-id="1dd67-121">説明</span><span class="sxs-lookup"><span data-stu-id="1dd67-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1dd67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dd67-122">Authorization</span></span> | <span data-ttu-id="1dd67-123">string</span><span class="sxs-lookup"><span data-stu-id="1dd67-123">string</span></span> | <span data-ttu-id="1dd67-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="1dd67-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dd67-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dd67-126">Request body</span></span>
<span data-ttu-id="1dd67-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="1dd67-128">次の表に、プログラムの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="1dd67-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1dd67-129">Property</span></span>     | <span data-ttu-id="1dd67-130">型</span><span class="sxs-lookup"><span data-stu-id="1dd67-130">Type</span></span>        | <span data-ttu-id="1dd67-131">説明</span><span class="sxs-lookup"><span data-stu-id="1dd67-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="1dd67-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="1dd67-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="1dd67-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="1dd67-134">応答</span><span class="sxs-lookup"><span data-stu-id="1dd67-134">Response</span></span>
<span data-ttu-id="1dd67-135">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dd67-136">例</span><span class="sxs-lookup"><span data-stu-id="1dd67-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dd67-137">要求</span><span class="sxs-lookup"><span data-stu-id="1dd67-137">Request</span></span>
<span data-ttu-id="1dd67-138">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1dd67-139">応答</span><span class="sxs-lookup"><span data-stu-id="1dd67-139">Response</span></span>
><span data-ttu-id="1dd67-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1dd67-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1dd67-142">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1dd67-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1dd67-143">Visual</span><span class="sxs-lookup"><span data-stu-id="1dd67-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1dd67-144">Java</span><span class="sxs-lookup"><span data-stu-id="1dd67-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="1dd67-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="1dd67-145">See also</span></span>

| <span data-ttu-id="1dd67-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="1dd67-146">Method</span></span>           | <span data-ttu-id="1dd67-147">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1dd67-147">Return Type</span></span>    |<span data-ttu-id="1dd67-148">説明</span><span class="sxs-lookup"><span data-stu-id="1dd67-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1dd67-149">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="1dd67-149">List programs</span></span>](program-list.md) | <span data-ttu-id="1dd67-150">[プログラム](../resources/program.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1dd67-150">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="1dd67-151">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-151">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="1dd67-152">プログラムの programControls を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1dd67-152">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="1dd67-153">[Programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1dd67-153">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="1dd67-154">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-154">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="1dd67-155">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="1dd67-155">Update program</span></span>](program-update.md) |  [<span data-ttu-id="1dd67-156">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dd67-156">program</span></span>](../resources/program.md)| <span data-ttu-id="1dd67-157">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-157">Update a program.</span></span>|
|[<span data-ttu-id="1dd67-158">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="1dd67-158">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="1dd67-159">programControl</span><span class="sxs-lookup"><span data-stu-id="1dd67-159">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="1dd67-160">プログラムに programControl を追加します。</span><span class="sxs-lookup"><span data-stu-id="1dd67-160">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
