---
title: educationclass プロパティを更新する
description: クラスのプロパティを更新します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 96a016618cc9f2ed97b5da178612da7d7ee0af44
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370376"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="0adb6-103">educationclass プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="0adb6-103">Update educationclass properties</span></span>

<span data-ttu-id="0adb6-104">クラスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0adb6-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="0adb6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0adb6-105">Permissions</span></span>
<span data-ttu-id="0adb6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0adb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0adb6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0adb6-108">Permission type</span></span>      | <span data-ttu-id="0adb6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0adb6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0adb6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0adb6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0adb6-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0adb6-111">Not supported.</span></span>  |
|<span data-ttu-id="0adb6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0adb6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0adb6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0adb6-113">Not supported.</span></span>   |
|<span data-ttu-id="0adb6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0adb6-114">Application</span></span> | <span data-ttu-id="0adb6-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0adb6-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0adb6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0adb6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0adb6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0adb6-117">Request headers</span></span>
| <span data-ttu-id="0adb6-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0adb6-118">Header</span></span>       | <span data-ttu-id="0adb6-119">値</span><span class="sxs-lookup"><span data-stu-id="0adb6-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0adb6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0adb6-120">Authorization</span></span>  | <span data-ttu-id="0adb6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0adb6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0adb6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0adb6-123">Content-Type</span></span>  | <span data-ttu-id="0adb6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0adb6-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0adb6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0adb6-125">Request body</span></span>
<span data-ttu-id="0adb6-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0adb6-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0adb6-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="0adb6-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0adb6-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0adb6-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0adb6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0adb6-129">Property</span></span>     | <span data-ttu-id="0adb6-130">型</span><span class="sxs-lookup"><span data-stu-id="0adb6-130">Type</span></span>   |<span data-ttu-id="0adb6-131">説明</span><span class="sxs-lookup"><span data-stu-id="0adb6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0adb6-132">description</span><span class="sxs-lookup"><span data-stu-id="0adb6-132">description</span></span>|<span data-ttu-id="0adb6-133">String</span><span class="sxs-lookup"><span data-stu-id="0adb6-133">String</span></span>| <span data-ttu-id="0adb6-134">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="0adb6-134">Description of the class.</span></span>|
|<span data-ttu-id="0adb6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0adb6-135">displayName</span></span>|<span data-ttu-id="0adb6-136">文字列</span><span class="sxs-lookup"><span data-stu-id="0adb6-136">String</span></span>| <span data-ttu-id="0adb6-137">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="0adb6-137">Name of the class.</span></span>|
|<span data-ttu-id="0adb6-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0adb6-138">mailNickname</span></span>|<span data-ttu-id="0adb6-139">String</span><span class="sxs-lookup"><span data-stu-id="0adb6-139">String</span></span>| <span data-ttu-id="0adb6-140">機能が有効になっている場合に、すべてのユーザーに電子メールを送信する電子メールのエイリアス。</span><span class="sxs-lookup"><span data-stu-id="0adb6-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="0adb6-141">|classCode|String| 学校が使用するクラス コード。| |externalId|String| 同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="0adb6-141">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="0adb6-142">| |externalName|String|同期システム内のクラスの名前。| |externalSource|string| このクラスを作成した方法。</span><span class="sxs-lookup"><span data-stu-id="0adb6-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="0adb6-143">使用可能な値は`sis`、 `manual`、 `enum_sentinel`、. | です。</span><span class="sxs-lookup"><span data-stu-id="0adb6-143">The possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="0adb6-144">応答</span><span class="sxs-lookup"><span data-stu-id="0adb6-144">Response</span></span>
<span data-ttu-id="0adb6-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0adb6-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0adb6-146">例</span><span class="sxs-lookup"><span data-stu-id="0adb6-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0adb6-147">要求</span><span class="sxs-lookup"><span data-stu-id="0adb6-147">Request</span></span>
<span data-ttu-id="0adb6-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0adb6-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0adb6-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0adb6-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0adb6-150">C#</span><span class="sxs-lookup"><span data-stu-id="0adb6-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0adb6-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0adb6-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0adb6-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="0adb6-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0adb6-153">Java</span><span class="sxs-lookup"><span data-stu-id="0adb6-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0adb6-154">応答</span><span class="sxs-lookup"><span data-stu-id="0adb6-154">Response</span></span>
<span data-ttu-id="0adb6-155">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0adb6-155">The following is an example of the response.</span></span> 

><span data-ttu-id="0adb6-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0adb6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
