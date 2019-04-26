---
title: programcontrol を作成する
description: Azure AD access レビュー機能で、新しい programcontrol オブジェクトを作成します。  これにより、アクセスレビューがプログラムにリンクされます。
localization_priority: Normal
ms.openlocfilehash: d7a48b45049c2268856a3ec238114cfa9bf834f5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332044"
---
# <a name="create-programcontrol"></a><span data-ttu-id="42f27-104">programcontrol を作成する</span><span class="sxs-lookup"><span data-stu-id="42f27-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42f27-105">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[programcontrol](../resources/programcontrol.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="42f27-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="42f27-106">これにより、アクセスレビューがプログラムにリンクされます。</span><span class="sxs-lookup"><span data-stu-id="42f27-106">This links an access review to a program.</span></span>

<span data-ttu-id="42f27-107">この要求を行う前に、発信者が以前に</span><span class="sxs-lookup"><span data-stu-id="42f27-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="42f27-108">の`programId`値を要求に含めるには、[プログラムを作成](program-create.md)するか、[プログラムを取得](program-list.md)しました。</span><span class="sxs-lookup"><span data-stu-id="42f27-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="42f27-109">の`controlId`値を要求に含めるために、[アクセスレビューを作成](accessreview-create.md)するか、[アクセスレビューを取得](accessreview-get.md)しました。</span><span class="sxs-lookup"><span data-stu-id="42f27-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="42f27-110">の`controlTypeId`値を要求に含めるために、[プログラムコントロールの種類の一覧を取得](programcontroltype-list.md)しました。</span><span class="sxs-lookup"><span data-stu-id="42f27-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="42f27-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42f27-111">Permissions</span></span>
<span data-ttu-id="42f27-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42f27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f27-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42f27-114">Permission type</span></span>                        | <span data-ttu-id="42f27-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42f27-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="42f27-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42f27-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="42f27-117">programcontrol</span><span class="sxs-lookup"><span data-stu-id="42f27-117">ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="42f27-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42f27-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42f27-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42f27-119">Not supported.</span></span> |
|<span data-ttu-id="42f27-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42f27-120">Application</span></span>                            |  <span data-ttu-id="42f27-121">programcontrol</span><span class="sxs-lookup"><span data-stu-id="42f27-121">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="42f27-122">また、サインインしているユーザーは、 **programcontrol**を作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="42f27-122">The signed in user must also be in a directory role that permits them to create a **programControl**.</span></span> 

## <a name="http-request"></a><span data-ttu-id="42f27-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42f27-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="42f27-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42f27-124">Request headers</span></span>
| <span data-ttu-id="42f27-125">名前</span><span class="sxs-lookup"><span data-stu-id="42f27-125">Name</span></span>         | <span data-ttu-id="42f27-126">型</span><span class="sxs-lookup"><span data-stu-id="42f27-126">Type</span></span>        | <span data-ttu-id="42f27-127">説明</span><span class="sxs-lookup"><span data-stu-id="42f27-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="42f27-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="42f27-128">Authorization</span></span> | <span data-ttu-id="42f27-129">string</span><span class="sxs-lookup"><span data-stu-id="42f27-129">string</span></span> | <span data-ttu-id="42f27-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="42f27-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42f27-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="42f27-132">Request body</span></span>
<span data-ttu-id="42f27-133">要求本文で、 [programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42f27-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="42f27-134">次の表に、プログラムコントロールの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="42f27-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="42f27-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42f27-135">Property</span></span>     | <span data-ttu-id="42f27-136">型</span><span class="sxs-lookup"><span data-stu-id="42f27-136">Type</span></span>        | <span data-ttu-id="42f27-137">説明</span><span class="sxs-lookup"><span data-stu-id="42f27-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="42f27-138">このコントロールが一部になるプログラムの programid。</span><span class="sxs-lookup"><span data-stu-id="42f27-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="42f27-139">コントロールの controlId (特にアクセスレビューの識別子)。</span><span class="sxs-lookup"><span data-stu-id="42f27-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="42f27-140">programcontroltype には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。</span><span class="sxs-lookup"><span data-stu-id="42f27-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="42f27-141">応答</span><span class="sxs-lookup"><span data-stu-id="42f27-141">Response</span></span>
<span data-ttu-id="42f27-142">成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[programcontrol](../resources/programcontrol.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="42f27-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="42f27-143">例</span><span class="sxs-lookup"><span data-stu-id="42f27-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42f27-144">要求</span><span class="sxs-lookup"><span data-stu-id="42f27-144">Request</span></span>
<span data-ttu-id="42f27-145">要求本文で、 [programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42f27-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="42f27-146">応答</span><span class="sxs-lookup"><span data-stu-id="42f27-146">Response</span></span>
><span data-ttu-id="42f27-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="42f27-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="42f27-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="42f27-149">See also</span></span>

| <span data-ttu-id="42f27-150">メソッド</span><span class="sxs-lookup"><span data-stu-id="42f27-150">Method</span></span>           | <span data-ttu-id="42f27-151">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="42f27-151">Return Type</span></span>    |<span data-ttu-id="42f27-152">説明</span><span class="sxs-lookup"><span data-stu-id="42f27-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42f27-153">programcontroltypes のリスト</span><span class="sxs-lookup"><span data-stu-id="42f27-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="42f27-154">[programcontroltype](../resources/programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="42f27-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="42f27-155">プログラムコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="42f27-155">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
