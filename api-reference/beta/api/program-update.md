---
title: 更新プログラム
description: Azure AD のレビュー機能にアクセス、既存のプログラム オブジェクトを更新します。
ms.openlocfilehash: e3d8ca75683a076f156e359431204517b60e7c6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071833"
---
# <a name="update-program"></a><span data-ttu-id="31e97-103">更新プログラム</span><span class="sxs-lookup"><span data-stu-id="31e97-103">Update program</span></span>

> <span data-ttu-id="31e97-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31e97-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31e97-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e97-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31e97-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、既存の[プログラム](../resources/program.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="31e97-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="31e97-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="31e97-107">Permissions</span></span>
<span data-ttu-id="31e97-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31e97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31e97-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31e97-110">Permission type</span></span>                        | <span data-ttu-id="31e97-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="31e97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="31e97-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31e97-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="31e97-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="31e97-113"></span></span>  <span data-ttu-id="31e97-114">サインインしているユーザーは、プログラムを更新することを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="31e97-114">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="31e97-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31e97-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31e97-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e97-116">Not supported.</span></span> |
|<span data-ttu-id="31e97-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31e97-117">Application</span></span>                            | <span data-ttu-id="31e97-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e97-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31e97-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31e97-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="31e97-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31e97-120">Request headers</span></span>
| <span data-ttu-id="31e97-121">名前</span><span class="sxs-lookup"><span data-stu-id="31e97-121">Name</span></span>         | <span data-ttu-id="31e97-122">型</span><span class="sxs-lookup"><span data-stu-id="31e97-122">Type</span></span>        | <span data-ttu-id="31e97-123">説明</span><span class="sxs-lookup"><span data-stu-id="31e97-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="31e97-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="31e97-124">Authorization</span></span> | <span data-ttu-id="31e97-125">string</span><span class="sxs-lookup"><span data-stu-id="31e97-125">string</span></span> | <span data-ttu-id="31e97-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="31e97-126">Bearer \{token\}.</span></span> <span data-ttu-id="31e97-127">必須。</span><span class="sxs-lookup"><span data-stu-id="31e97-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31e97-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="31e97-128">Request body</span></span>
<span data-ttu-id="31e97-129">要求の本文には、[プログラム](../resources/program.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="31e97-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="31e97-130">プログラムを更新するときに指定できるプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="31e97-130">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="31e97-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31e97-131">Property</span></span>     | <span data-ttu-id="31e97-132">型</span><span class="sxs-lookup"><span data-stu-id="31e97-132">Type</span></span>        | <span data-ttu-id="31e97-133">説明</span><span class="sxs-lookup"><span data-stu-id="31e97-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="31e97-134">プログラムの名前です。</span><span class="sxs-lookup"><span data-stu-id="31e97-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="31e97-135">プログラムの説明です。</span><span class="sxs-lookup"><span data-stu-id="31e97-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="31e97-136">応答</span><span class="sxs-lookup"><span data-stu-id="31e97-136">Response</span></span>
<span data-ttu-id="31e97-137">かどうかは成功すると、このメソッドが返されます、 `204, Accepted` 、応答の本体で応答コードと[プログラム](../resources/program.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="31e97-137">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e97-138">例</span><span class="sxs-lookup"><span data-stu-id="31e97-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31e97-139">要求</span><span class="sxs-lookup"><span data-stu-id="31e97-139">Request</span></span>
<span data-ttu-id="31e97-140">要求の本文には、[プログラム](../resources/program.md)オブジェクトのパラメーターを変更するのに JSON 形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="31e97-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="31e97-141">応答</span><span class="sxs-lookup"><span data-stu-id="31e97-141">Response</span></span>
><span data-ttu-id="31e97-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="31e97-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="31e97-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="31e97-144">See also</span></span>

| <span data-ttu-id="31e97-145">メソッド</span><span class="sxs-lookup"><span data-stu-id="31e97-145">Method</span></span>           | <span data-ttu-id="31e97-146">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="31e97-146">Return Type</span></span>    |<span data-ttu-id="31e97-147">説明</span><span class="sxs-lookup"><span data-stu-id="31e97-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31e97-148">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="31e97-148">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="31e97-149">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="31e97-149">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="31e97-150">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="31e97-150">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="31e97-151">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="31e97-151">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="31e97-152">デバッギング</span><span class="sxs-lookup"><span data-stu-id="31e97-152">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="31e97-153">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="31e97-153">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
