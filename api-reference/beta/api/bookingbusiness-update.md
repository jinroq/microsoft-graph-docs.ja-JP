---
title: Bookingbusiness の更新
description: BookingBusiness オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e841708eb41c6f12a7f38e0df2f1222fb3ad416e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439120"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="6b26c-103">Bookingbusiness の更新</span><span class="sxs-lookup"><span data-stu-id="6b26c-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b26c-104">[Bookingbusiness](../resources/bookingbusiness.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6b26c-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b26c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6b26c-105">Permissions</span></span>
<span data-ttu-id="6b26c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b26c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b26c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b26c-108">Permission type</span></span>      | <span data-ttu-id="6b26c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b26c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b26c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b26c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6b26c-111">予約します。すべての予約</span><span class="sxs-lookup"><span data-stu-id="6b26c-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6b26c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b26c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b26c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b26c-113">Not supported.</span></span>   |
|<span data-ttu-id="6b26c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b26c-114">Application</span></span> | <span data-ttu-id="6b26c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b26c-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6b26c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b26c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="6b26c-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b26c-117">Optional request headers</span></span>
| <span data-ttu-id="6b26c-118">名前</span><span class="sxs-lookup"><span data-stu-id="6b26c-118">Name</span></span>       | <span data-ttu-id="6b26c-119">説明</span><span class="sxs-lookup"><span data-stu-id="6b26c-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6b26c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b26c-120">Authorization</span></span>  | <span data-ttu-id="6b26c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6b26c-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b26c-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b26c-122">Request body</span></span>
<span data-ttu-id="6b26c-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6b26c-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6b26c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b26c-126">Property</span></span>     | <span data-ttu-id="6b26c-127">型</span><span class="sxs-lookup"><span data-stu-id="6b26c-127">Type</span></span>   |<span data-ttu-id="6b26c-128">説明</span><span class="sxs-lookup"><span data-stu-id="6b26c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b26c-129">address</span><span class="sxs-lookup"><span data-stu-id="6b26c-129">address</span></span>|[<span data-ttu-id="6b26c-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6b26c-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="6b26c-131">会社の住所。</span><span class="sxs-lookup"><span data-stu-id="6b26c-131">The street address of the business.</span></span>|
|<span data-ttu-id="6b26c-132">Microsoft.rtc.rgs.management.writablesettings.businesshours</span><span class="sxs-lookup"><span data-stu-id="6b26c-132">businessHours</span></span>|<span data-ttu-id="6b26c-133">[Bookingwork hours](../resources/bookingworkhours.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6b26c-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="6b26c-134">業務の運営時間。</span><span class="sxs-lookup"><span data-stu-id="6b26c-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="6b26c-135">businessType</span><span class="sxs-lookup"><span data-stu-id="6b26c-135">businessType</span></span>|<span data-ttu-id="6b26c-136">String</span><span class="sxs-lookup"><span data-stu-id="6b26c-136">String</span></span>|<span data-ttu-id="6b26c-137">業務の種類。</span><span class="sxs-lookup"><span data-stu-id="6b26c-137">The type of business.</span></span>|
|<span data-ttu-id="6b26c-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="6b26c-138">defaultCurrencyIso</span></span>|<span data-ttu-id="6b26c-139">String</span><span class="sxs-lookup"><span data-stu-id="6b26c-139">String</span></span>|<span data-ttu-id="6b26c-140">Microsoft の予約で勤務している通貨のコード。</span><span class="sxs-lookup"><span data-stu-id="6b26c-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="6b26c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6b26c-141">displayName</span></span>|<span data-ttu-id="6b26c-142">文字列</span><span class="sxs-lookup"><span data-stu-id="6b26c-142">String</span></span>|<span data-ttu-id="6b26c-143">顧客とのインターフェイスとなる企業の名前。</span><span class="sxs-lookup"><span data-stu-id="6b26c-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="6b26c-144">メール</span><span class="sxs-lookup"><span data-stu-id="6b26c-144">email</span></span>|<span data-ttu-id="6b26c-145">String</span><span class="sxs-lookup"><span data-stu-id="6b26c-145">String</span></span>|<span data-ttu-id="6b26c-146">ビジネスの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="6b26c-146">The email address for the business.</span></span>|
|<span data-ttu-id="6b26c-147">phone</span><span class="sxs-lookup"><span data-stu-id="6b26c-147">phone</span></span>|<span data-ttu-id="6b26c-148">String</span><span class="sxs-lookup"><span data-stu-id="6b26c-148">String</span></span>|<span data-ttu-id="6b26c-149">会社の電話番号。</span><span class="sxs-lookup"><span data-stu-id="6b26c-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="6b26c-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="6b26c-150">schedulingPolicy</span></span>|[<span data-ttu-id="6b26c-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="6b26c-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="6b26c-152">このビジネスに対して予約を作成する方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b26c-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="6b26c-153">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="6b26c-153">webSiteUrl</span></span>|<span data-ttu-id="6b26c-154">String</span><span class="sxs-lookup"><span data-stu-id="6b26c-154">String</span></span>|<span data-ttu-id="6b26c-155">ビジネス web サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="6b26c-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="6b26c-156">応答</span><span class="sxs-lookup"><span data-stu-id="6b26c-156">Response</span></span>
<span data-ttu-id="6b26c-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6b26c-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b26c-159">例</span><span class="sxs-lookup"><span data-stu-id="6b26c-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b26c-160">要求</span><span class="sxs-lookup"><span data-stu-id="6b26c-160">Request</span></span>
<span data-ttu-id="6b26c-161">次の例では、ビジネスの電子メールアドレスとスケジューリングポリシーを更新し、勤務先の既定の予約時間帯を1時間に変更してから30日以内に予約を進めます。</span><span class="sxs-lookup"><span data-stu-id="6b26c-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6b26c-162">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6b26c-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b26c-163">C#</span><span class="sxs-lookup"><span data-stu-id="6b26c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b26c-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="6b26c-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b26c-165">目的-C</span><span class="sxs-lookup"><span data-stu-id="6b26c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b26c-166">応答</span><span class="sxs-lookup"><span data-stu-id="6b26c-166">Response</span></span>
<span data-ttu-id="6b26c-167">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b26c-167">The following is an example of the response.</span></span> <span data-ttu-id="6b26c-168">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6b26c-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6b26c-169">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6b26c-169">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
