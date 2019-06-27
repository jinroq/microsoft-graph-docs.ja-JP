---
title: 'outlookUser: supportedTimeZones'
description: ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 087a79b1765033a68d429339a507d4833a0809b1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274292"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="9674d-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="9674d-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="9674d-104">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9674d-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="9674d-105">Windows のタイム ゾーン形式または [Internet Assigned Numbers Authority (IANA) のタイム ゾーン](https://www.iana.org/time-zones) (別称: Olson タイム ゾーン) 形式でタイム ゾーンが返されるよう、明示的に指定できます。</span><span class="sxs-lookup"><span data-stu-id="9674d-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="9674d-106">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="9674d-106">The Windows format is the default.</span></span>

<span data-ttu-id="9674d-107">Outlook クライアントを設定する際は、このサポートされているリストから、優先するタイム ゾーンを選択します。</span><span class="sxs-lookup"><span data-stu-id="9674d-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="9674d-108">これにより、[ユーザーのメールボックス設定を取得](user-get-mailboxsettings.md)することによって、優先タイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="9674d-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="9674d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9674d-109">Permissions</span></span>
<span data-ttu-id="9674d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9674d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9674d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9674d-112">Permission type</span></span>      | <span data-ttu-id="9674d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9674d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9674d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9674d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9674d-115">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="9674d-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="9674d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9674d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9674d-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="9674d-117">User.Read</span></span>    |
|<span data-ttu-id="9674d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9674d-118">Application</span></span> | <span data-ttu-id="9674d-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9674d-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9674d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9674d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="9674d-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="9674d-121">Function parameters</span></span>
| <span data-ttu-id="9674d-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9674d-122">Parameter</span></span>       | <span data-ttu-id="9674d-123">型</span><span class="sxs-lookup"><span data-stu-id="9674d-123">Type</span></span> | <span data-ttu-id="9674d-124">説明</span><span class="sxs-lookup"><span data-stu-id="9674d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9674d-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="9674d-125">TimeZoneStandard</span></span>  | <span data-ttu-id="9674d-126">timeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="9674d-126">timeZoneStandard</span></span>  | <span data-ttu-id="9674d-127">タイム ゾーンの形式。</span><span class="sxs-lookup"><span data-stu-id="9674d-127">A time zone format.</span></span> <span data-ttu-id="9674d-128">サポートされている値は `Windows` および `Iana` です。</span><span class="sxs-lookup"><span data-stu-id="9674d-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="9674d-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="9674d-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9674d-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9674d-130">Request headers</span></span>
| <span data-ttu-id="9674d-131">名前</span><span class="sxs-lookup"><span data-stu-id="9674d-131">Name</span></span>       | <span data-ttu-id="9674d-132">型</span><span class="sxs-lookup"><span data-stu-id="9674d-132">Type</span></span> | <span data-ttu-id="9674d-133">説明</span><span class="sxs-lookup"><span data-stu-id="9674d-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9674d-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="9674d-134">Authorization</span></span>  | <span data-ttu-id="9674d-135">string</span><span class="sxs-lookup"><span data-stu-id="9674d-135">string</span></span>  | <span data-ttu-id="9674d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9674d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9674d-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="9674d-138">Request body</span></span>
<span data-ttu-id="9674d-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9674d-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9674d-140">応答</span><span class="sxs-lookup"><span data-stu-id="9674d-140">Response</span></span>
<span data-ttu-id="9674d-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [timeZoneInformation](../resources/timezoneinformation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9674d-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9674d-142">例</span><span class="sxs-lookup"><span data-stu-id="9674d-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="9674d-143">要求 1</span><span class="sxs-lookup"><span data-stu-id="9674d-143">Request 1</span></span>
<span data-ttu-id="9674d-144">次の例では、`timeZoneStandard` パラメーターを指定せずに、Windows のタイム ゾーン形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9674d-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="9674d-145">応答 1</span><span class="sxs-lookup"><span data-stu-id="9674d-145">Response 1</span></span>
<span data-ttu-id="9674d-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9674d-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9674d-147">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9674d-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9674d-148">C#</span><span class="sxs-lookup"><span data-stu-id="9674d-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9674d-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="9674d-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9674d-150">目的-C</span><span class="sxs-lookup"><span data-stu-id="9674d-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="9674d-151">要求 2</span><span class="sxs-lookup"><span data-stu-id="9674d-151">Request 2</span></span>
<span data-ttu-id="9674d-152">次の例では、`TimeZoneStandard` パラメーターに `Iana` を指定して、IANA 形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9674d-152">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="9674d-153">応答 2</span><span class="sxs-lookup"><span data-stu-id="9674d-153">Response 2</span></span>
<span data-ttu-id="9674d-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9674d-154">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9674d-155">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9674d-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9674d-156">C#</span><span class="sxs-lookup"><span data-stu-id="9674d-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9674d-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="9674d-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9674d-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="9674d-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
