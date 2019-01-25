---
title: デバッギングを作成します。
description: Azure AD のレビュー機能にアクセス、デバッギング オブジェクトを新規作成します。  アクセス確認をプログラムにリンクします。
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511115"
---
# <a name="create-programcontrol"></a><span data-ttu-id="6af68-104">デバッギングを作成します。</span><span class="sxs-lookup"><span data-stu-id="6af68-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af68-105">機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[デバッギング](../resources/programcontrol.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6af68-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="6af68-106">アクセス確認をプログラムにリンクします。</span><span class="sxs-lookup"><span data-stu-id="6af68-106">This links an access review to a program.</span></span>

<span data-ttu-id="6af68-107">この要求を行う前に呼び出し元には以前</span><span class="sxs-lookup"><span data-stu-id="6af68-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="6af68-108">[プログラムを作成](program-create.md)または[プログラムを取得する](program-list.md)の値を設定する`programId`、要求に含める</span><span class="sxs-lookup"><span data-stu-id="6af68-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="6af68-109">[アクセス確認を作成](accessreview-create.md)または[、アクセス確認を取得する](accessreview-get.md)の値を設定する`controlId`、要求に含めると</span><span class="sxs-lookup"><span data-stu-id="6af68-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="6af68-110">[コントロールの種類のプログラムの一覧を取得](programcontroltype-list.md)の値を設定する`controlTypeId`要求に含める。</span><span class="sxs-lookup"><span data-stu-id="6af68-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="6af68-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6af68-111">Permissions</span></span>
<span data-ttu-id="6af68-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6af68-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af68-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6af68-114">Permission type</span></span>                        | <span data-ttu-id="6af68-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6af68-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6af68-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6af68-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6af68-117">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="6af68-117"></span></span>  <span data-ttu-id="6af68-118">サインインしているユーザーは、ディレクトリの役割を可能にして、デバッギングを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6af68-118">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="6af68-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6af68-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6af68-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6af68-120">Not supported.</span></span> |
|<span data-ttu-id="6af68-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6af68-121">Application</span></span>                            | <span data-ttu-id="6af68-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6af68-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6af68-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6af68-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="6af68-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6af68-124">Request headers</span></span>
| <span data-ttu-id="6af68-125">名前</span><span class="sxs-lookup"><span data-stu-id="6af68-125">Name</span></span>         | <span data-ttu-id="6af68-126">型</span><span class="sxs-lookup"><span data-stu-id="6af68-126">Type</span></span>        | <span data-ttu-id="6af68-127">説明</span><span class="sxs-lookup"><span data-stu-id="6af68-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6af68-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6af68-128">Authorization</span></span> | <span data-ttu-id="6af68-129">string</span><span class="sxs-lookup"><span data-stu-id="6af68-129">string</span></span> | <span data-ttu-id="6af68-130">ベアラー トークン</span><span class="sxs-lookup"><span data-stu-id="6af68-130">Bearer \{token\}.</span></span> <span data-ttu-id="6af68-131">必須です。</span><span class="sxs-lookup"><span data-stu-id="6af68-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6af68-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="6af68-132">Request body</span></span>
<span data-ttu-id="6af68-133">要求の本文には、[デバッギング](../resources/programcontrol.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6af68-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="6af68-134">プログラムのコントロールを作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="6af68-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="6af68-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6af68-135">Property</span></span>     | <span data-ttu-id="6af68-136">型</span><span class="sxs-lookup"><span data-stu-id="6af68-136">Type</span></span>        | <span data-ttu-id="6af68-137">説明</span><span class="sxs-lookup"><span data-stu-id="6af68-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="6af68-138">プログラムの programId コントロールしようの一部になります。</span><span class="sxs-lookup"><span data-stu-id="6af68-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="6af68-139">コントロールの処理、特にアクセスの id を確認します。</span><span class="sxs-lookup"><span data-stu-id="6af68-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="6af68-140">ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。</span><span class="sxs-lookup"><span data-stu-id="6af68-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="6af68-141">応答</span><span class="sxs-lookup"><span data-stu-id="6af68-141">Response</span></span>
<span data-ttu-id="6af68-142">かどうかは成功すると、このメソッドが返されます、`201, Created`応答コードおよび応答の本文の[デバッギング](../resources/programcontrol.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6af68-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="6af68-143">例</span><span class="sxs-lookup"><span data-stu-id="6af68-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6af68-144">要求</span><span class="sxs-lookup"><span data-stu-id="6af68-144">Request</span></span>
<span data-ttu-id="6af68-145">要求の本文には、[デバッギング](../resources/programcontrol.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6af68-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="6af68-146">応答</span><span class="sxs-lookup"><span data-stu-id="6af68-146">Response</span></span>
><span data-ttu-id="6af68-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6af68-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6af68-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="6af68-149">See also</span></span>

| <span data-ttu-id="6af68-150">メソッド</span><span class="sxs-lookup"><span data-stu-id="6af68-150">Method</span></span>           | <span data-ttu-id="6af68-151">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6af68-151">Return Type</span></span>    |<span data-ttu-id="6af68-152">説明</span><span class="sxs-lookup"><span data-stu-id="6af68-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6af68-153">リスト programControlTypes</span><span class="sxs-lookup"><span data-stu-id="6af68-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="6af68-154">[programControlType](../resources/programcontroltype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6af68-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="6af68-155">プログラムのコントロールの種類を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6af68-155">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
