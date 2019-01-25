---
title: 更新プログラム
description: Azure AD のレビュー機能にアクセス、既存のプログラム オブジェクトを更新します。
localization_priority: Normal
ms.openlocfilehash: 75562aac5a7b3f3aaef0c8a1251d32a7728813aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529923"
---
# <a name="update-program"></a><span data-ttu-id="be7e8-103">更新プログラム</span><span class="sxs-lookup"><span data-stu-id="be7e8-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be7e8-104">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、既存の[プログラム](../resources/program.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="be7e8-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be7e8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be7e8-105">Permissions</span></span>
<span data-ttu-id="be7e8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be7e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be7e8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be7e8-108">Permission type</span></span>                        | <span data-ttu-id="be7e8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be7e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="be7e8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be7e8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="be7e8-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="be7e8-111"></span></span>  <span data-ttu-id="be7e8-112">サインインしているユーザーは、プログラムを更新することを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="be7e8-112">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="be7e8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be7e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be7e8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be7e8-114">Not supported.</span></span> |
|<span data-ttu-id="be7e8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be7e8-115">Application</span></span>                            | <span data-ttu-id="be7e8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be7e8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be7e8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be7e8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="be7e8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be7e8-118">Request headers</span></span>
| <span data-ttu-id="be7e8-119">名前</span><span class="sxs-lookup"><span data-stu-id="be7e8-119">Name</span></span>         | <span data-ttu-id="be7e8-120">型</span><span class="sxs-lookup"><span data-stu-id="be7e8-120">Type</span></span>        | <span data-ttu-id="be7e8-121">説明</span><span class="sxs-lookup"><span data-stu-id="be7e8-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="be7e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be7e8-122">Authorization</span></span> | <span data-ttu-id="be7e8-123">string</span><span class="sxs-lookup"><span data-stu-id="be7e8-123">string</span></span> | <span data-ttu-id="be7e8-124">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="be7e8-124">Bearer \{token\}.</span></span> <span data-ttu-id="be7e8-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="be7e8-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be7e8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="be7e8-126">Request body</span></span>
<span data-ttu-id="be7e8-127">要求の本文には、[プログラム](../resources/program.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="be7e8-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="be7e8-128">プログラムを更新するときに指定できるプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="be7e8-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="be7e8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be7e8-129">Property</span></span>     | <span data-ttu-id="be7e8-130">型</span><span class="sxs-lookup"><span data-stu-id="be7e8-130">Type</span></span>        | <span data-ttu-id="be7e8-131">説明</span><span class="sxs-lookup"><span data-stu-id="be7e8-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="be7e8-132">プログラムの名前です。</span><span class="sxs-lookup"><span data-stu-id="be7e8-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="be7e8-133">プログラムの説明です。</span><span class="sxs-lookup"><span data-stu-id="be7e8-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="be7e8-134">応答</span><span class="sxs-lookup"><span data-stu-id="be7e8-134">Response</span></span>
<span data-ttu-id="be7e8-135">かどうかは成功すると、このメソッドが返されます、 `204, Accepted` 、応答の本体で応答コードと[プログラム](../resources/program.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="be7e8-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be7e8-136">例</span><span class="sxs-lookup"><span data-stu-id="be7e8-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be7e8-137">要求</span><span class="sxs-lookup"><span data-stu-id="be7e8-137">Request</span></span>
<span data-ttu-id="be7e8-138">要求の本文には、[プログラム](../resources/program.md)オブジェクトのパラメーターを変更するのに JSON 形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="be7e8-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="be7e8-139">応答</span><span class="sxs-lookup"><span data-stu-id="be7e8-139">Response</span></span>
><span data-ttu-id="be7e8-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="be7e8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="be7e8-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="be7e8-142">See also</span></span>

| <span data-ttu-id="be7e8-143">メソッド</span><span class="sxs-lookup"><span data-stu-id="be7e8-143">Method</span></span>           | <span data-ttu-id="be7e8-144">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be7e8-144">Return Type</span></span>    |<span data-ttu-id="be7e8-145">説明</span><span class="sxs-lookup"><span data-stu-id="be7e8-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be7e8-146">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="be7e8-146">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="be7e8-147">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="be7e8-147">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="be7e8-148">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="be7e8-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="be7e8-149">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="be7e8-149">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="be7e8-150">デバッギング</span><span class="sxs-lookup"><span data-stu-id="be7e8-150">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="be7e8-151">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="be7e8-151">Add a programControl to a program.</span></span>|

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
