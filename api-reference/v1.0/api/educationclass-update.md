---
title: educationclass プロパティを更新する
description: クラスのプロパティを更新します。
author: mmast-msft
ms.openlocfilehash: 9a11ae5e1a2139df4ade3417c940d00dea2d1888
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358710"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="4c1df-103">educationclass プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="4c1df-103">Update educationclass properties</span></span>

<span data-ttu-id="4c1df-104">クラスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c1df-104">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c1df-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c1df-105">Permissions</span></span>
<span data-ttu-id="4c1df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c1df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c1df-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c1df-108">Permission type</span></span>      | <span data-ttu-id="4c1df-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c1df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c1df-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c1df-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c1df-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c1df-111">Not supported.</span></span>  |
|<span data-ttu-id="4c1df-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c1df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c1df-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c1df-113">Not supported.</span></span>   |
|<span data-ttu-id="4c1df-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c1df-114">Application</span></span> | <span data-ttu-id="4c1df-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c1df-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c1df-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c1df-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4c1df-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c1df-117">Request headers</span></span>
| <span data-ttu-id="4c1df-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c1df-118">Header</span></span>       | <span data-ttu-id="4c1df-119">値</span><span class="sxs-lookup"><span data-stu-id="4c1df-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c1df-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c1df-120">Authorization</span></span>  | <span data-ttu-id="4c1df-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c1df-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4c1df-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c1df-123">Content-Type</span></span>  | <span data-ttu-id="4c1df-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c1df-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c1df-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c1df-125">Request body</span></span>
<span data-ttu-id="4c1df-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c1df-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4c1df-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="4c1df-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4c1df-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4c1df-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c1df-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c1df-129">Property</span></span>     | <span data-ttu-id="4c1df-130">種類</span><span class="sxs-lookup"><span data-stu-id="4c1df-130">Type</span></span>   |<span data-ttu-id="4c1df-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c1df-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c1df-132">説明</span><span class="sxs-lookup"><span data-stu-id="4c1df-132">description</span></span>|<span data-ttu-id="4c1df-133">String</span><span class="sxs-lookup"><span data-stu-id="4c1df-133">String</span></span>| <span data-ttu-id="4c1df-134">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="4c1df-134">Description of the class.</span></span>|
|<span data-ttu-id="4c1df-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4c1df-135">displayName</span></span>|<span data-ttu-id="4c1df-136">String</span><span class="sxs-lookup"><span data-stu-id="4c1df-136">String</span></span>| <span data-ttu-id="4c1df-137">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="4c1df-137">Name of the class.</span></span>|
|<span data-ttu-id="4c1df-138">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4c1df-138">mailNickname</span></span>|<span data-ttu-id="4c1df-139">String</span><span class="sxs-lookup"><span data-stu-id="4c1df-139">String</span></span>| <span data-ttu-id="4c1df-140">機能が有効になっている場合に、すべてのユーザーに電子メールを送信する電子メールのエイリアス。</span><span class="sxs-lookup"><span data-stu-id="4c1df-140">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="4c1df-141"><!-- Please verify the revised description here. -->| classCode |文字列 |クラスの学校で使用されるコードです |。| externalId |文字列 |同期中のシステムからのクラスの ID です。</span><span class="sxs-lookup"><span data-stu-id="4c1df-141"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="4c1df-142">| |externalName|String|同期システム内のクラスの名前。| |externalSource|string| このクラスを作成した方法。</span><span class="sxs-lookup"><span data-stu-id="4c1df-142">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="4c1df-143">可能な値: `sis`、 `manual`、 `enum_sentinel`. |</span><span class="sxs-lookup"><span data-stu-id="4c1df-143">The possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="4c1df-144">応答</span><span class="sxs-lookup"><span data-stu-id="4c1df-144">Response</span></span>
<span data-ttu-id="4c1df-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c1df-145">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c1df-146">例</span><span class="sxs-lookup"><span data-stu-id="4c1df-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c1df-147">要求</span><span class="sxs-lookup"><span data-stu-id="4c1df-147">Request</span></span>
<span data-ttu-id="4c1df-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c1df-148">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4c1df-149">応答</span><span class="sxs-lookup"><span data-stu-id="4c1df-149">Response</span></span>
<span data-ttu-id="4c1df-150">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c1df-150">The following is an example of the response.</span></span> 

><span data-ttu-id="4c1df-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4c1df-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->