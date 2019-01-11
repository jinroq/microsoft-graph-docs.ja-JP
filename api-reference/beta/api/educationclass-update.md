---
title: educationclass プロパティを更新する
description: クラスのプロパティを更新します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 1c011a19371490bb8d00a7048a9809cc8a58beee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813994"
---
# <a name="update-educationclass-properties"></a><span data-ttu-id="4a235-103">educationclass プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="4a235-103">Update educationclass properties</span></span>

> <span data-ttu-id="4a235-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a235-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a235-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a235-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a235-106">クラスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4a235-106">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a235-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a235-107">Permissions</span></span>
<span data-ttu-id="4a235-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a235-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a235-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a235-110">Permission type</span></span>      | <span data-ttu-id="4a235-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a235-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a235-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a235-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a235-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a235-113">Not supported.</span></span>  |
|<span data-ttu-id="4a235-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a235-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a235-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a235-115">Not supported.</span></span>   |
|<span data-ttu-id="4a235-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a235-116">Application</span></span> | <span data-ttu-id="4a235-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a235-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4a235-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a235-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4a235-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a235-119">Request headers</span></span>
| <span data-ttu-id="4a235-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a235-120">Header</span></span>       | <span data-ttu-id="4a235-121">値</span><span class="sxs-lookup"><span data-stu-id="4a235-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a235-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a235-122">Authorization</span></span>  | <span data-ttu-id="4a235-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a235-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4a235-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a235-125">Content-Type</span></span>  | <span data-ttu-id="4a235-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a235-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a235-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a235-127">Request body</span></span>
<span data-ttu-id="4a235-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a235-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4a235-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="4a235-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4a235-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4a235-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4a235-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a235-131">Property</span></span>     | <span data-ttu-id="4a235-132">種類</span><span class="sxs-lookup"><span data-stu-id="4a235-132">Type</span></span>   |<span data-ttu-id="4a235-133">説明</span><span class="sxs-lookup"><span data-stu-id="4a235-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a235-134">説明</span><span class="sxs-lookup"><span data-stu-id="4a235-134">description</span></span>|<span data-ttu-id="4a235-135">String</span><span class="sxs-lookup"><span data-stu-id="4a235-135">String</span></span>| <span data-ttu-id="4a235-136">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="4a235-136">Description of the class.</span></span>|
|<span data-ttu-id="4a235-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4a235-137">displayName</span></span>|<span data-ttu-id="4a235-138">String</span><span class="sxs-lookup"><span data-stu-id="4a235-138">String</span></span>| <span data-ttu-id="4a235-139">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="4a235-139">Name of the class.</span></span>|
|<span data-ttu-id="4a235-140">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4a235-140">mailNickname</span></span>|<span data-ttu-id="4a235-141">String</span><span class="sxs-lookup"><span data-stu-id="4a235-141">String</span></span>| <span data-ttu-id="4a235-142">機能が有効になっている場合に、すべてのユーザーに電子メールを送信する電子メールのエイリアス。</span><span class="sxs-lookup"><span data-stu-id="4a235-142">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="4a235-143"><!-- Please verify the revised description here. -->| classCode |文字列 |クラスの学校で使用されるコードです |。| externalId |文字列 |同期中のシステムからのクラスの ID です。</span><span class="sxs-lookup"><span data-stu-id="4a235-143"><!-- Please verify the revised description here. --> |classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="4a235-144">| |externalName|String|同期システム内のクラスの名前。| |externalSource|string| このクラスを作成した方法。</span><span class="sxs-lookup"><span data-stu-id="4a235-144">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="4a235-145">使用可能な値: `sis`、`manual`、`enum_sentinel`.|</span><span class="sxs-lookup"><span data-stu-id="4a235-145">Possible values are: `sis`, `manual`, `enum_sentinel`.|</span></span>

## <a name="response"></a><span data-ttu-id="4a235-146">応答</span><span class="sxs-lookup"><span data-stu-id="4a235-146">Response</span></span>
<span data-ttu-id="4a235-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4a235-147">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a235-148">例</span><span class="sxs-lookup"><span data-stu-id="4a235-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a235-149">要求</span><span class="sxs-lookup"><span data-stu-id="4a235-149">Request</span></span>
<span data-ttu-id="4a235-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a235-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="4a235-151">応答</span><span class="sxs-lookup"><span data-stu-id="4a235-151">Response</span></span>
<span data-ttu-id="4a235-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a235-152">The following is an example of the response.</span></span> 

><span data-ttu-id="4a235-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4a235-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
