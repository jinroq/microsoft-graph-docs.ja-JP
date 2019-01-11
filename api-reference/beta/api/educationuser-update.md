---
title: educationUser プロパティを更新する
description: '**educationuser** オブジェクトのプロパティを更新します。'
localization_priority: Normal
ms.openlocfilehash: a6479095abbb1884acf98377e8fef9d115d4a6c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843513"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="024d9-103">educationUser プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="024d9-103">Update educationUser properties</span></span>

> <span data-ttu-id="024d9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="024d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="024d9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="024d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="024d9-106">**educationuser** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="024d9-106">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="024d9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="024d9-107">Permissions</span></span>
<span data-ttu-id="024d9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="024d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="024d9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="024d9-110">Permission type</span></span>      | <span data-ttu-id="024d9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="024d9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="024d9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="024d9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="024d9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="024d9-113">Not supported.</span></span>  |
|<span data-ttu-id="024d9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="024d9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="024d9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="024d9-115">Not supported.</span></span>  |
|<span data-ttu-id="024d9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="024d9-116">Application</span></span> | <span data-ttu-id="024d9-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="024d9-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="024d9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="024d9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="024d9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="024d9-119">Request headers</span></span>
| <span data-ttu-id="024d9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="024d9-120">Header</span></span>       | <span data-ttu-id="024d9-121">値</span><span class="sxs-lookup"><span data-stu-id="024d9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="024d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="024d9-122">Authorization</span></span>  | <span data-ttu-id="024d9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="024d9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="024d9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="024d9-125">Content-Type</span></span>  | <span data-ttu-id="024d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="024d9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="024d9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="024d9-127">Request body</span></span>
<span data-ttu-id="024d9-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="024d9-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="024d9-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="024d9-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="024d9-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="024d9-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="024d9-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="024d9-131">Property</span></span>     | <span data-ttu-id="024d9-132">種類</span><span class="sxs-lookup"><span data-stu-id="024d9-132">Type</span></span>   |<span data-ttu-id="024d9-133">説明</span><span class="sxs-lookup"><span data-stu-id="024d9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="024d9-134">displayName</span><span class="sxs-lookup"><span data-stu-id="024d9-134">displayName</span></span>| <span data-ttu-id="024d9-135">String</span><span class="sxs-lookup"><span data-stu-id="024d9-135">String</span></span>| <span data-ttu-id="024d9-136">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="024d9-136">Display Name of User</span></span>|
|<span data-ttu-id="024d9-137">givenName</span><span class="sxs-lookup"><span data-stu-id="024d9-137">givenName</span></span>| <span data-ttu-id="024d9-138">String</span><span class="sxs-lookup"><span data-stu-id="024d9-138">String</span></span> | <span data-ttu-id="024d9-139">名</span><span class="sxs-lookup"><span data-stu-id="024d9-139">First Name</span></span> |
|<span data-ttu-id="024d9-140">middleName</span><span class="sxs-lookup"><span data-stu-id="024d9-140">middleName</span></span>| <span data-ttu-id="024d9-141">String</span><span class="sxs-lookup"><span data-stu-id="024d9-141">String</span></span> | <span data-ttu-id="024d9-142">ユーザーのミドル ネーム</span><span class="sxs-lookup"><span data-stu-id="024d9-142">Middle Name of user</span></span>|
|<span data-ttu-id="024d9-143">surname</span><span class="sxs-lookup"><span data-stu-id="024d9-143">surname</span></span>| <span data-ttu-id="024d9-144">String</span><span class="sxs-lookup"><span data-stu-id="024d9-144">String</span></span> | <span data-ttu-id="024d9-145">ユーザーの姓</span><span class="sxs-lookup"><span data-stu-id="024d9-145">Surname of user</span></span>|
|<span data-ttu-id="024d9-146">mail</span><span class="sxs-lookup"><span data-stu-id="024d9-146">mail</span></span>| <span data-ttu-id="024d9-147">String</span><span class="sxs-lookup"><span data-stu-id="024d9-147">String</span></span>| <span data-ttu-id="024d9-148">メール アドレス</span><span class="sxs-lookup"><span data-stu-id="024d9-148">email address</span></span>|
|<span data-ttu-id="024d9-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="024d9-149">mobilePhone</span></span>| <span data-ttu-id="024d9-150">String</span><span class="sxs-lookup"><span data-stu-id="024d9-150">String</span></span> | <span data-ttu-id="024d9-151">ユーザーの携帯電話番号</span><span class="sxs-lookup"><span data-stu-id="024d9-151">Mobile number of user</span></span> |
|<span data-ttu-id="024d9-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="024d9-152">externalSource</span></span>|<span data-ttu-id="024d9-153">文字列</span><span class="sxs-lookup"><span data-stu-id="024d9-153">string</span></span>| <span data-ttu-id="024d9-154">使用可能な値: `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="024d9-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="024d9-155">externalSource</span><span class="sxs-lookup"><span data-stu-id="024d9-155">externalSource</span></span>|<span data-ttu-id="024d9-156">文字列</span><span class="sxs-lookup"><span data-stu-id="024d9-156">string</span></span>| <span data-ttu-id="024d9-157">このユーザーが作成された場所。</span><span class="sxs-lookup"><span data-stu-id="024d9-157">Where this user was created from.</span></span>  <span data-ttu-id="024d9-158">使用可能な値: `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="024d9-158">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="024d9-159">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="024d9-159">mailingAddress</span></span>|[<span data-ttu-id="024d9-160">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="024d9-160">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="024d9-161">ユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="024d9-161">Mail address of user.</span></span>|
|<span data-ttu-id="024d9-162">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="024d9-162">residenceAddress</span></span>|[<span data-ttu-id="024d9-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="024d9-163">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="024d9-164">ユーザーが在住している場所のアドレス。</span><span class="sxs-lookup"><span data-stu-id="024d9-164">Address where user lives.</span></span>|
|<span data-ttu-id="024d9-165">primaryRole</span><span class="sxs-lookup"><span data-stu-id="024d9-165">primaryRole</span></span>|<span data-ttu-id="024d9-166">文字列</span><span class="sxs-lookup"><span data-stu-id="024d9-166">string</span></span>| <span data-ttu-id="024d9-167">ユーザーの既定のロール。</span><span class="sxs-lookup"><span data-stu-id="024d9-167">Default Role for a user.</span></span>  <span data-ttu-id="024d9-168">ユーザーのロールは、個々のクラスで異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="024d9-168">The user's role might be different in an individual class.</span></span> <span data-ttu-id="024d9-169">使用可能な値: `student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="024d9-169">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="024d9-170">student</span><span class="sxs-lookup"><span data-stu-id="024d9-170">student</span></span>|[<span data-ttu-id="024d9-171">educationStudent</span><span class="sxs-lookup"><span data-stu-id="024d9-171">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="024d9-172">プライマリ ロールが学生の場合、このブロックには学生固有のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="024d9-172">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="024d9-173">teacher</span><span class="sxs-lookup"><span data-stu-id="024d9-173">teacher</span></span>|[<span data-ttu-id="024d9-174">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="024d9-174">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="024d9-175">プライマリ ロールが教師の場合、このブロックには教師固有のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="024d9-175">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="024d9-176">応答</span><span class="sxs-lookup"><span data-stu-id="024d9-176">Response</span></span>
<span data-ttu-id="024d9-177">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationUser](../resources/educationuser.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="024d9-177">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="024d9-178">例</span><span class="sxs-lookup"><span data-stu-id="024d9-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="024d9-179">要求</span><span class="sxs-lookup"><span data-stu-id="024d9-179">Request</span></span>
<span data-ttu-id="024d9-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="024d9-180">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a><span data-ttu-id="024d9-181">応答</span><span class="sxs-lookup"><span data-stu-id="024d9-181">Response</span></span>
<span data-ttu-id="024d9-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="024d9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
