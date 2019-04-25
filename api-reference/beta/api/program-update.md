---
title: プログラムの更新
description: Azure AD access レビュー機能で、既存のプログラムオブジェクトを更新します。
localization_priority: Normal
ms.openlocfilehash: 75562aac5a7b3f3aaef0c8a1251d32a7728813aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538548"
---
# <a name="update-program"></a><span data-ttu-id="37142-103">プログラムの更新</span><span class="sxs-lookup"><span data-stu-id="37142-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37142-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、既存の[プログラム](../resources/program.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="37142-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37142-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37142-105">Permissions</span></span>
<span data-ttu-id="37142-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37142-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37142-108">Permission type</span></span>                        | <span data-ttu-id="37142-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37142-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="37142-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37142-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="37142-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="37142-111"></span></span>  <span data-ttu-id="37142-112">また、サインインしているユーザーは、プログラムの更新を許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="37142-112">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="37142-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37142-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37142-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37142-114">Not supported.</span></span> |
|<span data-ttu-id="37142-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37142-115">Application</span></span>                            | <span data-ttu-id="37142-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37142-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37142-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37142-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="37142-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37142-118">Request headers</span></span>
| <span data-ttu-id="37142-119">名前</span><span class="sxs-lookup"><span data-stu-id="37142-119">Name</span></span>         | <span data-ttu-id="37142-120">型</span><span class="sxs-lookup"><span data-stu-id="37142-120">Type</span></span>        | <span data-ttu-id="37142-121">説明</span><span class="sxs-lookup"><span data-stu-id="37142-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="37142-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37142-122">Authorization</span></span> | <span data-ttu-id="37142-123">string</span><span class="sxs-lookup"><span data-stu-id="37142-123">string</span></span> | <span data-ttu-id="37142-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="37142-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37142-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="37142-126">Request body</span></span>
<span data-ttu-id="37142-127">要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="37142-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="37142-128">次の表は、プログラムの更新時に提供できるプロパティを示しています。</span><span class="sxs-lookup"><span data-stu-id="37142-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="37142-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37142-129">Property</span></span>     | <span data-ttu-id="37142-130">型</span><span class="sxs-lookup"><span data-stu-id="37142-130">Type</span></span>        | <span data-ttu-id="37142-131">説明</span><span class="sxs-lookup"><span data-stu-id="37142-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="37142-132">プログラムの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="37142-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="37142-133">プログラムの説明。</span><span class="sxs-lookup"><span data-stu-id="37142-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="37142-134">応答</span><span class="sxs-lookup"><span data-stu-id="37142-134">Response</span></span>
<span data-ttu-id="37142-135">成功した場合、このメソッド`204, Accepted`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="37142-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37142-136">例</span><span class="sxs-lookup"><span data-stu-id="37142-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37142-137">要求</span><span class="sxs-lookup"><span data-stu-id="37142-137">Request</span></span>
<span data-ttu-id="37142-138">要求本文で、変更する[プログラム](../resources/program.md)オブジェクトのパラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="37142-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a><span data-ttu-id="37142-139">応答</span><span class="sxs-lookup"><span data-stu-id="37142-139">Response</span></span>
><span data-ttu-id="37142-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="37142-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="37142-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="37142-142">See also</span></span>

| <span data-ttu-id="37142-143">メソッド</span><span class="sxs-lookup"><span data-stu-id="37142-143">Method</span></span>           | <span data-ttu-id="37142-144">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="37142-144">Return Type</span></span>    |<span data-ttu-id="37142-145">説明</span><span class="sxs-lookup"><span data-stu-id="37142-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37142-146">プログラムの programcontrols を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="37142-146">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="37142-147">[programcontrol](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="37142-147">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="37142-148">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="37142-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="37142-149">programcontrol を作成する</span><span class="sxs-lookup"><span data-stu-id="37142-149">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="37142-150">programcontrol</span><span class="sxs-lookup"><span data-stu-id="37142-150">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="37142-151">プログラムに programcontrol を追加します。</span><span class="sxs-lookup"><span data-stu-id="37142-151">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
