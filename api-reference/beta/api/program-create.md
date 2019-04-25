---
title: プログラムを作成する
description: Azure AD access レビュー機能で、新しいプログラムオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538540"
---
# <a name="create-program"></a><span data-ttu-id="ee394-103">プログラムを作成する</span><span class="sxs-lookup"><span data-stu-id="ee394-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee394-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[プログラム](../resources/program.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee394-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee394-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee394-105">Permissions</span></span>
<span data-ttu-id="ee394-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee394-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee394-108">Permission type</span></span>                        | <span data-ttu-id="ee394-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee394-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee394-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee394-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee394-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="ee394-111"></span></span>  <span data-ttu-id="ee394-112">サインインしているユーザーは、プログラムを作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee394-112">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="ee394-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee394-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee394-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee394-114">Not supported.</span></span> |
|<span data-ttu-id="ee394-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee394-115">Application</span></span>                            | <span data-ttu-id="ee394-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee394-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee394-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee394-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="ee394-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee394-118">Request headers</span></span>
| <span data-ttu-id="ee394-119">名前</span><span class="sxs-lookup"><span data-stu-id="ee394-119">Name</span></span>         | <span data-ttu-id="ee394-120">型</span><span class="sxs-lookup"><span data-stu-id="ee394-120">Type</span></span>        | <span data-ttu-id="ee394-121">説明</span><span class="sxs-lookup"><span data-stu-id="ee394-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ee394-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee394-122">Authorization</span></span> | <span data-ttu-id="ee394-123">string</span><span class="sxs-lookup"><span data-stu-id="ee394-123">string</span></span> | <span data-ttu-id="ee394-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee394-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee394-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee394-126">Request body</span></span>
<span data-ttu-id="ee394-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee394-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="ee394-128">次の表に、プログラムの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee394-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="ee394-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee394-129">Property</span></span>     | <span data-ttu-id="ee394-130">型</span><span class="sxs-lookup"><span data-stu-id="ee394-130">Type</span></span>        | <span data-ttu-id="ee394-131">説明</span><span class="sxs-lookup"><span data-stu-id="ee394-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="ee394-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee394-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="ee394-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="ee394-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="ee394-134">応答</span><span class="sxs-lookup"><span data-stu-id="ee394-134">Response</span></span>
<span data-ttu-id="ee394-135">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee394-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee394-136">例</span><span class="sxs-lookup"><span data-stu-id="ee394-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee394-137">要求</span><span class="sxs-lookup"><span data-stu-id="ee394-137">Request</span></span>
<span data-ttu-id="ee394-138">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee394-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="ee394-139">応答</span><span class="sxs-lookup"><span data-stu-id="ee394-139">Response</span></span>
><span data-ttu-id="ee394-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ee394-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ee394-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="ee394-142">See also</span></span>

| <span data-ttu-id="ee394-143">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee394-143">Method</span></span>           | <span data-ttu-id="ee394-144">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ee394-144">Return Type</span></span>    |<span data-ttu-id="ee394-145">説明</span><span class="sxs-lookup"><span data-stu-id="ee394-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ee394-146">プログラムの一覧表示</span><span class="sxs-lookup"><span data-stu-id="ee394-146">List programs</span></span>](program-list.md) | <span data-ttu-id="ee394-147">[プログラム](../resources/program.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ee394-147">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="ee394-148">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ee394-148">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="ee394-149">プログラムの programcontrols を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ee394-149">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="ee394-150">[programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ee394-150">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="ee394-151">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ee394-151">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ee394-152">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="ee394-152">Update program</span></span>](program-update.md) |  [<span data-ttu-id="ee394-153">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee394-153">program</span></span>](../resources/program.md)| <span data-ttu-id="ee394-154">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="ee394-154">Update a program.</span></span>|
|[<span data-ttu-id="ee394-155">programcontrol を作成する</span><span class="sxs-lookup"><span data-stu-id="ee394-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="ee394-156">programcontrol</span><span class="sxs-lookup"><span data-stu-id="ee394-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="ee394-157">プログラムに programcontrol を追加します。</span><span class="sxs-lookup"><span data-stu-id="ee394-157">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
