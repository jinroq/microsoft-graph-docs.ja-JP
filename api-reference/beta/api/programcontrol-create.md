---
title: ProgramControl を作成する
description: Azure AD access レビュー機能で、新しい programControl オブジェクトを作成します。  これにより、アクセスレビューがプログラムにリンクされます。
localization_priority: Normal
ms.openlocfilehash: 822b9c58651eb1a997b00553f34f40e1d7b9886d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268020"
---
# <a name="create-programcontrol"></a><span data-ttu-id="b0b2b-104">ProgramControl を作成する</span><span class="sxs-lookup"><span data-stu-id="b0b2b-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0b2b-105">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[programcontrol](../resources/programcontrol.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="b0b2b-106">これにより、アクセスレビューがプログラムにリンクされます。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-106">This links an access review to a program.</span></span>

<span data-ttu-id="b0b2b-107">この要求を行う前に、発信者が以前に</span><span class="sxs-lookup"><span data-stu-id="b0b2b-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="b0b2b-108">の`programId`値を要求に含めるには、[プログラムを作成](program-create.md)するか、[プログラムを取得](program-list.md)しました。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="b0b2b-109">の`controlId`値を要求に含めるために、[アクセスレビューを作成](accessreview-create.md)するか、[アクセスレビューを取得](accessreview-get.md)しました。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="b0b2b-110">の`controlTypeId`値を要求に含めるために、[プログラムコントロールの種類の一覧を取得](programcontroltype-list.md)しました。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="b0b2b-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0b2b-111">Permissions</span></span>
<span data-ttu-id="b0b2b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0b2b-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0b2b-114">Permission type</span></span>                        | <span data-ttu-id="b0b2b-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0b2b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0b2b-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0b2b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0b2b-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0b2b-117">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="b0b2b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0b2b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0b2b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-119">Not supported.</span></span> |
|<span data-ttu-id="b0b2b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0b2b-120">Application</span></span>                            |  <span data-ttu-id="b0b2b-121">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0b2b-121">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="b0b2b-122">また、サインインしているユーザーは、 **Programcontrol**を作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-122">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="b0b2b-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0b2b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="b0b2b-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0b2b-124">Request headers</span></span>
| <span data-ttu-id="b0b2b-125">名前</span><span class="sxs-lookup"><span data-stu-id="b0b2b-125">Name</span></span>         | <span data-ttu-id="b0b2b-126">型</span><span class="sxs-lookup"><span data-stu-id="b0b2b-126">Type</span></span>        | <span data-ttu-id="b0b2b-127">説明</span><span class="sxs-lookup"><span data-stu-id="b0b2b-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b0b2b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0b2b-128">Authorization</span></span> | <span data-ttu-id="b0b2b-129">string</span><span class="sxs-lookup"><span data-stu-id="b0b2b-129">string</span></span> | <span data-ttu-id="b0b2b-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0b2b-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0b2b-132">Request body</span></span>
<span data-ttu-id="b0b2b-133">要求本文で、 [Programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="b0b2b-134">次の表に、プログラムコントロールの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="b0b2b-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0b2b-135">Property</span></span>     | <span data-ttu-id="b0b2b-136">型</span><span class="sxs-lookup"><span data-stu-id="b0b2b-136">Type</span></span>        | <span data-ttu-id="b0b2b-137">説明</span><span class="sxs-lookup"><span data-stu-id="b0b2b-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="b0b2b-138">このコントロールが一部になるプログラムの programId。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="b0b2b-139">コントロールの controlId (特にアクセスレビューの識別子)。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="b0b2b-140">ProgramControlType には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="b0b2b-141">応答</span><span class="sxs-lookup"><span data-stu-id="b0b2b-141">Response</span></span>
<span data-ttu-id="b0b2b-142">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[programcontrol](../resources/programcontrol.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b0b2b-143">例</span><span class="sxs-lookup"><span data-stu-id="b0b2b-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0b2b-144">要求</span><span class="sxs-lookup"><span data-stu-id="b0b2b-144">Request</span></span>
<span data-ttu-id="b0b2b-145">要求本文で、 [Programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a><span data-ttu-id="b0b2b-146">応答</span><span class="sxs-lookup"><span data-stu-id="b0b2b-146">Response</span></span>
><span data-ttu-id="b0b2b-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0b2b-149">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b0b2b-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0b2b-150">C#</span><span class="sxs-lookup"><span data-stu-id="b0b2b-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_programControl_from_programControls-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0b2b-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0b2b-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_programControl_from_programControls-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b0b2b-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="b0b2b-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_programControl_from_programControls-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="b0b2b-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0b2b-153">See also</span></span>

| <span data-ttu-id="b0b2b-154">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0b2b-154">Method</span></span>           | <span data-ttu-id="b0b2b-155">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b0b2b-155">Return Type</span></span>    |<span data-ttu-id="b0b2b-156">説明</span><span class="sxs-lookup"><span data-stu-id="b0b2b-156">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0b2b-157">ProgramControlTypes のリスト</span><span class="sxs-lookup"><span data-stu-id="b0b2b-157">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="b0b2b-158">[Programcontroltype](../resources/programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b0b2b-158">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="b0b2b-159">プログラムコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b0b2b-159">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
