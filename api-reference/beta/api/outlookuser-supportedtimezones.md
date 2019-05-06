---
title: 'outlookUser: supportedTimeZones'
description: ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f76e92a6908246fe025022ae9839dfee81d2421c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596040"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="da3b2-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="da3b2-103">outlookUser: supportedTimeZones</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da3b2-104">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="da3b2-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="da3b2-105">Windows のタイム ゾーン形式または [Internet Assigned Numbers Authority (IANA) のタイム ゾーン](https://www.iana.org/time-zones) (別称: Olson タイム ゾーン) 形式でタイム ゾーンが返されるよう、明示的に指定できます。</span><span class="sxs-lookup"><span data-stu-id="da3b2-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="da3b2-106">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="da3b2-106">The Windows format is the default.</span></span>

<span data-ttu-id="da3b2-107">Outlook クライアントを設定する際は、このサポートされているリストから、優先するタイム ゾーンを選択します。</span><span class="sxs-lookup"><span data-stu-id="da3b2-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="da3b2-108">これにより、[ユーザーのメールボックス設定を取得](user-get-mailboxsettings.md)することによって、優先タイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="da3b2-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="da3b2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da3b2-109">Permissions</span></span>
<span data-ttu-id="da3b2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da3b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da3b2-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da3b2-112">Permission type</span></span>      | <span data-ttu-id="da3b2-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da3b2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da3b2-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da3b2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="da3b2-115">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="da3b2-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="da3b2-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da3b2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da3b2-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="da3b2-117">User.Read</span></span>    |
|<span data-ttu-id="da3b2-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da3b2-118">Application</span></span> | <span data-ttu-id="da3b2-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="da3b2-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da3b2-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da3b2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="da3b2-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="da3b2-121">Function parameters</span></span>
| <span data-ttu-id="da3b2-122">パラメーター</span><span class="sxs-lookup"><span data-stu-id="da3b2-122">Parameter</span></span>      | <span data-ttu-id="da3b2-123">型</span><span class="sxs-lookup"><span data-stu-id="da3b2-123">Type</span></span>    | <span data-ttu-id="da3b2-124">説明</span><span class="sxs-lookup"><span data-stu-id="da3b2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da3b2-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="da3b2-125">TimeZoneStandard</span></span>  | <span data-ttu-id="da3b2-126">String</span><span class="sxs-lookup"><span data-stu-id="da3b2-126">String</span></span>  | <span data-ttu-id="da3b2-127">タイム ゾーンの形式。</span><span class="sxs-lookup"><span data-stu-id="da3b2-127">A time zone format.</span></span> <span data-ttu-id="da3b2-128">サポートされている値は `Windows` および `Iana` です。</span><span class="sxs-lookup"><span data-stu-id="da3b2-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="da3b2-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="da3b2-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="da3b2-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da3b2-130">Request headers</span></span>
| <span data-ttu-id="da3b2-131">名前</span><span class="sxs-lookup"><span data-stu-id="da3b2-131">Name</span></span>       | <span data-ttu-id="da3b2-132">型</span><span class="sxs-lookup"><span data-stu-id="da3b2-132">Type</span></span> | <span data-ttu-id="da3b2-133">説明</span><span class="sxs-lookup"><span data-stu-id="da3b2-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da3b2-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="da3b2-134">Authorization</span></span>  | <span data-ttu-id="da3b2-135">string</span><span class="sxs-lookup"><span data-stu-id="da3b2-135">string</span></span>  | <span data-ttu-id="da3b2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="da3b2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da3b2-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="da3b2-138">Request body</span></span>
<span data-ttu-id="da3b2-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="da3b2-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da3b2-140">応答</span><span class="sxs-lookup"><span data-stu-id="da3b2-140">Response</span></span>
<span data-ttu-id="da3b2-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [timeZoneInformation](../resources/timezoneinformation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="da3b2-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da3b2-142">例</span><span class="sxs-lookup"><span data-stu-id="da3b2-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="da3b2-143">要求 1</span><span class="sxs-lookup"><span data-stu-id="da3b2-143">Request 1</span></span>
<span data-ttu-id="da3b2-144">次の例では、`timeZoneStandard` パラメーターを指定せずに、Windows のタイム ゾーン形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="da3b2-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="da3b2-145">応答 1</span><span class="sxs-lookup"><span data-stu-id="da3b2-145">Response 1</span></span>
<span data-ttu-id="da3b2-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="da3b2-146">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="da3b2-147">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="da3b2-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="da3b2-148">Visual</span><span class="sxs-lookup"><span data-stu-id="da3b2-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da3b2-149">Java</span><span class="sxs-lookup"><span data-stu-id="da3b2-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="da3b2-150">要求 2</span><span class="sxs-lookup"><span data-stu-id="da3b2-150">Request 2</span></span>
<span data-ttu-id="da3b2-151">次の例では、`TimeZoneStandard` パラメーターに `Iana` を指定して、IANA 形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="da3b2-151">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="da3b2-152">応答 2</span><span class="sxs-lookup"><span data-stu-id="da3b2-152">Response 2</span></span>
<span data-ttu-id="da3b2-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="da3b2-153">Here is an example of the response.</span></span> 

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="da3b2-154">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="da3b2-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="da3b2-155">Visual</span><span class="sxs-lookup"><span data-stu-id="da3b2-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da3b2-156">Java</span><span class="sxs-lookup"><span data-stu-id="da3b2-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
