---
title: デバッギングを作成します。
description: Azure AD のレビュー機能にアクセス、デバッギング オブジェクトを新規作成します。  アクセス確認をプログラムにリンクします。
ms.openlocfilehash: fa6a93b13391fd4b9e3c5816bb2a27259e730c0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072034"
---
# <a name="create-programcontrol"></a><span data-ttu-id="a567d-104">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="a567d-104">Create programControl</span></span>

> <span data-ttu-id="a567d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a567d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a567d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a567d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a567d-107">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[デバッギング](../resources/programcontrol.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a567d-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="a567d-108">アクセス確認をプログラムにリンクします。</span><span class="sxs-lookup"><span data-stu-id="a567d-108">This links an access review to a program.</span></span>

<span data-ttu-id="a567d-109">この要求を行う前に呼び出し元には以前</span><span class="sxs-lookup"><span data-stu-id="a567d-109">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="a567d-110">[プログラムを作成](program-create.md)または[プログラムを取得する](program-list.md)の値を設定する`programId`、要求に含める</span><span class="sxs-lookup"><span data-stu-id="a567d-110">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="a567d-111">[アクセス確認を作成](accessreview-create.md)または[、アクセス確認を取得する](accessreview-get.md)の値を設定する`controlId`、要求に含めると</span><span class="sxs-lookup"><span data-stu-id="a567d-111">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="a567d-112">[コントロールの種類のプログラムの一覧を取得](programcontroltype-list.md)の値を設定する`controlTypeId`要求に含める。</span><span class="sxs-lookup"><span data-stu-id="a567d-112">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="a567d-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a567d-113">Permissions</span></span>
<span data-ttu-id="a567d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a567d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a567d-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a567d-116">Permission type</span></span>                        | <span data-ttu-id="a567d-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a567d-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a567d-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a567d-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="a567d-119">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a567d-119"></span></span>  <span data-ttu-id="a567d-120">サインインしているユーザーは、ディレクトリの役割を可能にして、デバッギングを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a567d-120">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="a567d-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a567d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a567d-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a567d-122">Not supported.</span></span> |
|<span data-ttu-id="a567d-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a567d-123">Application</span></span>                            | <span data-ttu-id="a567d-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a567d-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a567d-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a567d-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="a567d-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a567d-126">Request headers</span></span>
| <span data-ttu-id="a567d-127">名前</span><span class="sxs-lookup"><span data-stu-id="a567d-127">Name</span></span>         | <span data-ttu-id="a567d-128">型</span><span class="sxs-lookup"><span data-stu-id="a567d-128">Type</span></span>        | <span data-ttu-id="a567d-129">説明</span><span class="sxs-lookup"><span data-stu-id="a567d-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a567d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a567d-130">Authorization</span></span> | <span data-ttu-id="a567d-131">string</span><span class="sxs-lookup"><span data-stu-id="a567d-131">string</span></span> | <span data-ttu-id="a567d-132">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="a567d-132">Bearer \{token\}.</span></span> <span data-ttu-id="a567d-133">必須。</span><span class="sxs-lookup"><span data-stu-id="a567d-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a567d-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="a567d-134">Request body</span></span>
<span data-ttu-id="a567d-135">要求の本文には、[デバッギング](../resources/programcontrol.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a567d-135">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="a567d-136">プログラムのコントロールを作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a567d-136">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="a567d-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a567d-137">Property</span></span>     | <span data-ttu-id="a567d-138">型</span><span class="sxs-lookup"><span data-stu-id="a567d-138">Type</span></span>        | <span data-ttu-id="a567d-139">説明</span><span class="sxs-lookup"><span data-stu-id="a567d-139">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="a567d-140">プログラムの programId コントロールしようの一部になります。</span><span class="sxs-lookup"><span data-stu-id="a567d-140">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="a567d-141">コントロールの処理、特にアクセスの id を確認します。</span><span class="sxs-lookup"><span data-stu-id="a567d-141">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="a567d-142">ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。</span><span class="sxs-lookup"><span data-stu-id="a567d-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="a567d-143">応答</span><span class="sxs-lookup"><span data-stu-id="a567d-143">Response</span></span>
<span data-ttu-id="a567d-144">かどうかは成功すると、このメソッドが返されます、`201, Created`応答コードおよび応答の本文の[デバッギング](../resources/programcontrol.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a567d-144">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="a567d-145">例</span><span class="sxs-lookup"><span data-stu-id="a567d-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a567d-146">要求</span><span class="sxs-lookup"><span data-stu-id="a567d-146">Request</span></span>
<span data-ttu-id="a567d-147">要求の本文には、[デバッギング](../resources/programcontrol.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a567d-147">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="a567d-148">応答</span><span class="sxs-lookup"><span data-stu-id="a567d-148">Response</span></span>
><span data-ttu-id="a567d-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a567d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a567d-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="a567d-151">See also</span></span>

| <span data-ttu-id="a567d-152">メソッド</span><span class="sxs-lookup"><span data-stu-id="a567d-152">Method</span></span>           | <span data-ttu-id="a567d-153">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a567d-153">Return Type</span></span>    |<span data-ttu-id="a567d-154">説明</span><span class="sxs-lookup"><span data-stu-id="a567d-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a567d-155">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="a567d-155">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="a567d-156">[programControlType](../resources/programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a567d-156">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="a567d-157">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a567d-157">List program control types.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
