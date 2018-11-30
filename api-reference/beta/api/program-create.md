---
title: プログラムを作成します。
description: Azure AD のレビュー機能にアクセス、新しいプログラム オブジェクトを作成します。
ms.openlocfilehash: 1ac3fa1f0b555fc92449adf0e57217d0a7d50375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072486"
---
# <a name="create-program"></a><span data-ttu-id="f9c3f-103">プログラムを作成します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-103">Create program</span></span>

> <span data-ttu-id="f9c3f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9c3f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9c3f-106">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[プログラム](../resources/program.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9c3f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f9c3f-107">Permissions</span></span>
<span data-ttu-id="f9c3f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9c3f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9c3f-110">Permission type</span></span>                        | <span data-ttu-id="f9c3f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9c3f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9c3f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9c3f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9c3f-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f9c3f-113"></span></span>  <span data-ttu-id="f9c3f-114">サインインしているユーザーは、プログラムを作成することを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="f9c3f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9c3f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9c3f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-116">Not supported.</span></span> |
|<span data-ttu-id="f9c3f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9c3f-117">Application</span></span>                            | <span data-ttu-id="f9c3f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9c3f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9c3f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="f9c3f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9c3f-120">Request headers</span></span>
| <span data-ttu-id="f9c3f-121">名前</span><span class="sxs-lookup"><span data-stu-id="f9c3f-121">Name</span></span>         | <span data-ttu-id="f9c3f-122">型</span><span class="sxs-lookup"><span data-stu-id="f9c3f-122">Type</span></span>        | <span data-ttu-id="f9c3f-123">説明</span><span class="sxs-lookup"><span data-stu-id="f9c3f-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f9c3f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9c3f-124">Authorization</span></span> | <span data-ttu-id="f9c3f-125">string</span><span class="sxs-lookup"><span data-stu-id="f9c3f-125">string</span></span> | <span data-ttu-id="f9c3f-126">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-126">Bearer \{token\}.</span></span> <span data-ttu-id="f9c3f-127">必須。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9c3f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9c3f-128">Request body</span></span>
<span data-ttu-id="f9c3f-129">要求の本文には、[プログラム](../resources/program.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="f9c3f-130">プログラムを作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="f9c3f-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9c3f-131">Property</span></span>     | <span data-ttu-id="f9c3f-132">型</span><span class="sxs-lookup"><span data-stu-id="f9c3f-132">Type</span></span>        | <span data-ttu-id="f9c3f-133">説明</span><span class="sxs-lookup"><span data-stu-id="f9c3f-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="f9c3f-134">プログラムの名前です。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="f9c3f-135">プログラムの説明です。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="f9c3f-136">応答</span><span class="sxs-lookup"><span data-stu-id="f9c3f-136">Response</span></span>
<span data-ttu-id="f9c3f-137">かどうかは成功すると、このメソッドが返されます、 `201, Created` 、応答の本体で応答コードと[プログラム](../resources/program.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9c3f-138">例</span><span class="sxs-lookup"><span data-stu-id="f9c3f-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9c3f-139">要求</span><span class="sxs-lookup"><span data-stu-id="f9c3f-139">Request</span></span>
<span data-ttu-id="f9c3f-140">要求の本文には、[プログラム](../resources/program.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f9c3f-141">応答</span><span class="sxs-lookup"><span data-stu-id="f9c3f-141">Response</span></span>
><span data-ttu-id="f9c3f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f9c3f-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="f9c3f-144">See also</span></span>

| <span data-ttu-id="f9c3f-145">メソッド</span><span class="sxs-lookup"><span data-stu-id="f9c3f-145">Method</span></span>           | <span data-ttu-id="f9c3f-146">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f9c3f-146">Return Type</span></span>    |<span data-ttu-id="f9c3f-147">説明</span><span class="sxs-lookup"><span data-stu-id="f9c3f-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f9c3f-148">プログラムを一覧表示</span><span class="sxs-lookup"><span data-stu-id="f9c3f-148">List programs</span></span>](program-list.md) | <span data-ttu-id="f9c3f-149">[プログラム](../resources/program.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="f9c3f-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="f9c3f-150">すべてのプログラムのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="f9c3f-151">プログラムのリスト programControls</span><span class="sxs-lookup"><span data-stu-id="f9c3f-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="f9c3f-152">[デバッギング](../resources/programcontrol.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f9c3f-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="f9c3f-153">プログラムのコントロールのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="f9c3f-154">更新プログラム</span><span class="sxs-lookup"><span data-stu-id="f9c3f-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="f9c3f-155">プログラム</span><span class="sxs-lookup"><span data-stu-id="f9c3f-155">program</span></span>](../resources/program.md)| <span data-ttu-id="f9c3f-156">プログラムを更新します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-156">Update a program.</span></span>|
|[<span data-ttu-id="f9c3f-157">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="f9c3f-158">デバッギング</span><span class="sxs-lookup"><span data-stu-id="f9c3f-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="f9c3f-159">デバッギングをプログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="f9c3f-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->